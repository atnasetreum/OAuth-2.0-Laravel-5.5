### Crear Usuario DB

CREATE USER 'homestead'@'localhost' IDENTIFIED BY 'secret';
GRANT ALL PRIVILEGES ON * . * TO 'homestead'@'localhost';
FLUSH PRIVILEGES;

### Instalar dependencias laravel
composer update

### Instalar dependencias npm
npm install

### Compilar
npm run dev

### Correr Migraciones
php artisan migrate

### Crear clientes pasport
php artisan passport:install

### Ejecutar proyecto
php artisan serve

### Registro
Registrar un nuevo usuario

### postman
En los headers de la peticion GET http://127.0.0.1:8000/api/user
Accept = application/json
Authorization = Bearer (Personal Access Tokens)
