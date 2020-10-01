composer create-project symfony/skeleton project ^5.1.0
mv project/* .
http://localhost:250/
composer validate
composer update
composer require monolog doctrine phpunit
composer require --dev browser-kit maker
composer require api