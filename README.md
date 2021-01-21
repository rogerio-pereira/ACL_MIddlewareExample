git clone git@github.com:rogerio-pereira/ACL_MIddlewareExample.git  
cd ACL_MIddlewareExample  
touch database/database.sqlite  
cp .env.example .env  
php artisan key:generate  
composer update  
npm install  
npm run dev  
php artisan migrate --seed  
php artisan serve  

