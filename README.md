Template Name: Personal
Kit de herramientas de AWS para Visual Studio:
https://aws.amazon.com/es/visualstudio/
```
https://aws.amazon.com/es/visualstudio/
```
asegurate de tener la version de visual studio requerida por el sdk aws

luego puedes verificar la version con:

```
aws --version
```
te saldra algo como:
aws-cli/2.15.6 Python/3.11.6 Windows/10 exe/AMD64 prompt/off

luego será necesario verificar el contenido del archivo de configuración de las credenciales de AWS.
el comando 
```
 cat ~/.aws/credentials
```
Este archivo suele contener información como el ID de clave de acceso, la clave de acceso secreta y la región de AWS.
Se verá similar a esto:
[default]
aws_access_key_id = XXXX...

Si es asi, entonces deberás crear un USUARIO en tu cuenta de amazon con las aws_access_key_id = TU_ACCESS_KEY_ID
aws_secret_access_key = TU_SECRET_ACCESS_KEY y darles permisos de programador

El servicio de AWS IAM provee de esta configuracion  
Una vez esté listo, podras continuar con el uso de tu entorno Visual studio con .NET
