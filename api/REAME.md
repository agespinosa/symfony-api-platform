composer create-project symfony/skeleton project ^5.1.0
mv project/* .
http://localhost:250/
composer validate
composer update
composer require monolog doctrine phpunit
composer require --dev browser-kit maker
composer require api
composer require symfony/security-core symfony/uid
# Para autenticacion con jwt
https://github.com/lexik/LexikJWTAuthenticationBundle
composer require "lexik/jwt-authentication-bundle"
copiar el valor de la clave JWT_PASSPHRASE= dentro de .env
pegarlo en la tarea generate-ssh-keys atributo pass:
ejecutar cmd generate-ssh-keys
probar la configuracion
php bin/console lexik:jwt:check-config