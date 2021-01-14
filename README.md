# Multi-User To-Do application
 
version: v1.0.1
 
Multi-User To-Do application (Aplicación multiusuario de tareas pendientes) (Se utiliza la implementación Laravel Jetstream para añadir la funcionalidad de autenticación)
 
### SET UP
* Requirements (Already covered with Docker deployment)
	1. Apache/2.4.27 or greater.
	2. MySQL 5.7 or greater.
	3. PHP/7.2.24 or greater.
  
* App Configuration
    1. Add host `multiuser-todo.localhost`,
        	see [Edit hosts](https://dinahosting.com/ayuda/como-modificar-el-fichero-hosts).        	
    2. Create `.env` file from `.env.example` and set it.
	3. Give Folder permissions:	
	    ```
	    sudo chown -R $USER:www-data storage;
        chmod -R 775 storage;
        sudo chown -R $USER:www-data bootstrap/cache;
        chmod -R 775 bootstrap/cache;
	    ```
    4. Set `APP_KEY=base64:8jv5dNpL4Dn9hHdzTNosZS/xAiuGPRtKiKRWvD2K/y8=` at `.env`.
    5. Set `DB_DATABASE=root_multiuser_todo` at `.env`.     	
	6. Run `composer install`.
	7. Run `php artisan storage:link`. 
	8. Run `php artisan migrate`. 	

* Browse at [multiuser-todo.localhost](http://http://multiuser-todo.localhost).
 
* Login at [multiuser-todo.localhost/login](http://http://multiuser-todo.localhost/login).

* Register at [multiuser-todo.localhost/register](http://http://multiuser-todo.localhost/register).
 
### CONTRIBUTION: Guidelines & Documentation
 
* Git :
    [Gitflow](http://nvie.com/posts/a-successful-git-branching-model).
* Back End:
    [Laravel 8.21](https://laravel.com/docs/8.x),
* Front End:
    [Tailwind CSS 2.0.1](https://tailwindcss.com/docs),
 
***
 
2021 [Samuel Ramirez](https://github.com/Samvel24/)