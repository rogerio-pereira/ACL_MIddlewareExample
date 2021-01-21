# Instalation
git clone git@github.com:rogerio-pereira/ACL_MIddlewareExample.git  
cd ACL_MIddlewareExample  
composer update  
npm install  
npm run dev  
cp .env.example .env  
touch database/database.sqlite  
php artisan key:generate  
php artisan migrate --seed  
php artisan serve  

# Users
admin@test.com
user@test.com
Both passwords are "password"

# Usage
Login with admin, navigate to http://localhost:8000/admin. I'll see will be allowed.
Login with user, navigate to http://localhost:8000/admin. I'll see will be redirected to dashboard, because user isn't allowed to access.
The middleware will check, User's role attibute, and redirect it if not allowed.

# Important Files
app\Http\Middleware\ChechRole
app\Http\Kernel - Line 66
app\Models\User
routes\web - Last block
