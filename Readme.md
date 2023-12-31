# Segunda Práctica Integradora

## Consigna

Continuar sobre el proyecto que has trabajado para tu ecommerce y configurar los siguientes elementos:

1. Crear un modelo `User` el cual contará con los siguientes campos:
   - `first_name`: String
   - `last_name`: String
   - `email`: String (único)
   - `age`: Number
   - `password`: String (Hash)
   - `cart`: Id con referencia a Carts
   - `role`: String (default: 'user')

2. Desarrollar las estrategias de Passport para que funcionen con este modelo de usuarios.

3. Modificar el sistema de login del usuario para poder trabajar con session o con JWT (a tu elección).

4. (Sólo para JWT) Desarrollar una estrategia "current" para extraer la cookie que contiene el token para obtener el usuario asociado a dicho token. En caso de tener el token, devolver al usuario asociado al token; en caso contrario, devolver un error de Passport. Utilizar un extractor de cookie.

5. Agregar al router `/api/sessions/` la ruta `/current`, la cual utilizará el modelo de sesión que estés utilizando para poder devolver en una respuesta el usuario actual.
