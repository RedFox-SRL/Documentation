# Apis Documentación
## Authentication
### **`POST`/Register**
<p>Permite registrar un nuevo usuario en el sistema.</p>

##### Parámetro de solicitud Registro {collapsible="true"}

---

| Parámetro    | Tipo   | Descripción                                                      | Requerido |
|--------------|--------|------------------------------------------------------------------|-----------|
| `name`       | string | Nombre del usuario. Longitud máxima de 255 caracteres.           | Sí        |
| `last_name`  | string | Apellido del usuario. Longitud máxima de 255 caracteres.         | Sí        |
| `email`      | string | Correo electrónico del usuario. Debe estar en formato válido.    | Sí        |
| `password`   | string | Contraseña del usuario. Longitud mínima de 8 caracteres.         | Sí        |
| `role`       | string | Rol del usuario (`student` o `teacher`).                         | Sí        |

---

###
<procedure title="Respuestas" >
<step>
    <tabs>
    <tab title="✅200 ">
        <p>Cuando el registro es exitoso, el API retorna un token de autenticación y el rol del usuario.</p>

```json
{
  "token": "your_token",
  "access_type": "bearer",
  "expires_in": 3600,
  "role": "student"
} 
```
</tab>
    <tab title="401">
        <p>Si las credenciales son inválidas o faltan parámetros requeridos.</p>

```json
{
  "code": 251,
  "message": "Invalid email or password."
} 
```
</tab>
<tab title="422">
        <p>Si las credenciales son inválidas o faltan parámetros requeridos.</p>

```json
{
  "code": 422,
  "message": "The email has already been taken."
} 
```
</tab>
</tabs>
</step>
</procedure>

### **`POST`/Login**

<p>Permite a un usuario iniciar sesión.</p>

##### Parámetro de solicitud Login {collapsible="true"}

---

| Parámetro  | Tipo   | Descripción                     | Requerido |
|------------|--------|---------------------------------|-----------|
| `email`    | string | Correo electrónico del usuario. | Sí        |
| `password` | string | Contraseña del usuario.         | Sí        |

---


### 

<procedure title="Respuestas" >

<step>
    <tabs>
    <tab title="✅200 ">
        <p>Cuando las credenciales son válida.</p>

```json
{
  "token": "your_token",
  "access_type": "bearer",
  "expires_in": 3600,
  "role": "user_role"
}
```
</tab>
    <tab title="401">
        <p>Si las credenciales proporcionadas no son válidas.</p>

```json
{
  "code": 251,
  "message": "Invalid email or password."
} 
```
</tab>
</tabs>
</step>
</procedure>

### **`POST`/Logout**

<p>Permite a un usuario cerrar sesión.</p>

##### Parámetro de solicitud Logout {collapsible="true"}

| Parámetro | Tipo   | Descripción                                         | Requerido |
|-----------|--------|-----------------------------------------------------|-----------|
|Authorization| String | Debe incluir el token en el formato `Bearer<token>` | Sí        |

###

<procedure title="Respuestas" >

<step>
    <tabs>
    <tab title="✅200 ">
        <p>Cuando el cierre de sesión es exitoso.</p>
    
```json
{
  "token": "your_token",
  "access_type": "bearer",
  "expires_in": 3600,
  "role": "user_role"
}
```
</tab>
</tabs>
</step>
</procedure>

### **`POST`/Refresh Token**
<p>Este endpoint permite refrescar el token de autenticación de un usuario.</p>

##### Parámetro de solicitud Refresh Token {collapsible="true"}

| Parámetro | Tipo   | Descripción                                           | Requerido |
|-----------|--------|-------------------------------------------------------|-----------|
|Authorization| String | El token de auntenticación en formato `Bearer<token>` | Sí        |

### 
<procedure title="Respuestas" >

<step>
    <tabs>
    <tab title="✅200 ">
        <p> Si el token es válido, el servidor devuelve un nuevo token junto con el tiempo de expiración.</p>

```json
{
  "token": "new_token",
  "access_type": "bearer",
  "expires_in": 3600
}
```
</tab>
</tabs>
</step>
</procedure>

### **`GET`/User Info**
<p>Este endpoint devuelve la información del usuario autenticado.</p>

##### Parámetro de solicitud User Info {collapsible="true"}

| Parámetro | Tipo   | Descripción                                         | Requerido |
|-----------|--------|-----------------------------------------------------|-----------|
|Authorization| String | Debe incluir el token en el formato `Bearer<token>` | Sí        |

### 
<procedure title="Respuestas" >

<step>
    <tabs>
    <tab title="✅200">
        <p>Cuando la solicitud es exitosa, el servidor devuelve los datos del usuario.</p>

```json
{
  "id": 1,
  "name": "John Doe",
  "email": "john.doe@example.com",
  "role": "user_role"
}
```
</tab>
</tabs>
</step>
</procedure>

### **`PUT`/Update Profile**
<p>Este endpoint permite al usuario autenticado actualizar su información de perfil.</p>

##### Parámetro de solicitud Update Profile {collapsible="true"}

---
| Parámetro    | Tipo   | Descripción                                              | Requerido |
|--------------|--------|----------------------------------------------------------|-----------|
| `name`       | string | El nuevo nombre del usuario.                             | Sí        |
| `last_name`  | string | El nuevo apellido del usuario.                           | Sí        |
| `email`      | string | El nuevo Correo electrónico del usuario.                 | Sí        |
| `_method`   | string | Este campo debe tener el valor `PUT` para realizar laactualización.  | Sí        |

---
###
<procedure title="Respuestas" >

<step>
    <tabs>
    <tab title="✅200">
        <p>Si la actualización es exitosa, el servidor devuelve los datos actualizados del usuario junto con un mensaje de éxito.</p>

```json
{
  "user": {
    "id": 1,
    "name": "John",
    "last_name": "Doe",
    "email": "john.doe@example.com",
    "created_at": "2024-10-17T00:00:00.000Z",
    "updated_at": "2024-10-17T12:00:00.000Z",
    "role": "user_role"
  },
  "message": "Profile updated successfully."
}
```
</tab>
    <tab title="401">
        <p>Si el token de autenticación no es válido o está ausente.</p>

```json
{
  "code": 251,
  "message": "Invalid email or password."
}
```
</tab>
</tabs>
</step>
</procedure>

### **`GET`/Verify Email**

<p> Este endpoint permite verificar el correo electrónico de un usuario utilizando un ID de verificación.</p>

##### Parámetro de solicitud Verify Email {collapsible="true"}

---
| Parámetro | Tipo   | Descripción                                                 | Requerido |
|-----------|--------|-------------------------------------------------------------|-----------|
| `id`      | string | El `ID` de verificación que se envió al correo del usuario. | Sí        |

---
###
<procedure title="Respuestas" >

<step>
    <tabs>
    <tab title="✅302">
        <p>Cuando la verificación es exitosa, el servidor redirige al usuario a la página de inicio.</p>
</tab>
    <tab title="403">
        <p>Si la URL de verificación no es válida o ha expirado.</p>

```json
{
  "code": 253,
  "message": "Invalid/Expired url provider."
}
```
</tab>
</tabs>
</step>
</procedure>

### **`GET`/Resend Verification Email**

<p> Este endpoint permite reenviar el correo de verificación a un usuario autenticado.</p>

##### Parámetro de solicitud Resent Verify Email {collapsible="true"}
---
| Parámetro       | Tipo   | Descripción                                           | Requerido |
|-----------------|--------|-------------------------------------------------------|-----------|
| `Authorization` | string | El token de autenticación en formato `Bearer<token>`. | Sí        |

---
###
<procedure title="Respuestas" >

<step>
    <tabs>
    <tab title="✅200">
        <p>Si el correo de verificación se reenvía correctamente, el servidor devuelve un mensaje de éxito.</p>

```json
{
    "message": "Email verification link sent on your email id"
}
```
</tab>
    <tab title="400">
        <p> Si el correo ya ha sido verificado.</p>

```json
{
  "code": 254,
  "message": "Email already verified."
}
```
</tab>
    <tab title="403">
        <p>Si las credenciales no son válidas (token inválido o faltante).</p>

```json
{
  "code": 251,
  "message": "Invalid email or password."
}
```
</tab>
</tabs>
</step>
</procedure>

### **`POST`/Forgot Password**

<p>  Este endpoint permite solicitar un enlace para restablecer la contraseña de un usuario.</p>

##### Parámetro de solicitud Forgot Password {collapsible="true"}
---
| Parámetro | Tipo   | Descripción                                    | Requerido |
|-----------|--------|------------------------------------------------|-----------|
| `email`   | string | El correo electrónico del usuario registrado`. | Sí        |

---
###
<procedure title="Respuestas" >

<step>
    <tabs>
    <tab title="✅200">
        <p>Si el correo electrónico se encuentra en la base de datos, el servidor enviará un enlace para
 restablecer la contraseña a la dirección de correo proporcionada.</p>

```json
{
  "message": "Reset password link sent on your email id."
}
```
</tab>
    <tab title="400">
        <p>Si el correo electrónico no está registrado en el sistema.</p>

```json
{
  "code": 272,
  "message": "Email not found."
}
```
</tab>
    <tab title="400">
        <p>Si ocurre un error de validación, por ejemplo, si el campo de correo está vacío o no tiene el formato correcto.</p>

```json
{
  "code": 252,
  "message": "Validation error."
}
```
</tab>
</tabs>
</step>
</procedure>

### **`POST`/Reset Password**

<p>Este endpoint permite restablecer la contraseña de un usuario utilizando un token de restablecimiento.</p>

##### Parámetro de solicitud Reset Password {collapsible="true"}
---
| Parámetro  | Tipo   | Descripción                                   | Requerido |
|------------|--------|-----------------------------------------------|-----------|
| `email`    | string | El correo electrónico del usuario registrado. | Sí        |
| `token`    | string | El token de restablecimiento de contraseña recibido.| Sí        |
| `password` | string | La nueva contraseña que desea establecer el usuario.| Sí        |
| `password_confirmation`| string | Confirmación de la nueva contraseña.          | Sí        |

---
###
<procedure title="Respuestas" >

<step>
    <tabs>
    <tab title=" ✅200">
        <p>Si el restablecimiento de la contraseña es exitoso, el servidor devuelve un mensaje de confirmación.</p>

```json
{
  "message": "Password successfully changed"
}
```
</tab>
    <tab title="400">
        <p>Si el token proporcionado no es válido o ha expirado.</p>

```json
{
  "code": 255,
  "message": "Invalid token provided"
}
```
</tab>
    <tab title="400">
        <p>Si ocurre un error de validación, por ejemplo, si las contraseñas no coinciden o no cumplen con los criterios de seguridad.</p>

```json
{
  "code": 252,
  "message": "Validation error."
}
```
</tab>
</tabs>
</step>
</procedure>

## Management


Start typing here...