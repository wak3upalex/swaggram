# swaggram

## Steps to launch
1. Launch Postgres Database
2. Check connection to the DB
```shell
psql -h 127.0.0.1 -U your_db_user -d your_db_name
```
3. If your database is empty, then create default tables
```shell
php artisan migrate
```
Laravel expects certain tables to exist, especially if you’re using database-based caching, sessions, or queues.

This will create default Laravel tables, such as:
-	users → if you’re using authentication.
-	password_resets → for password recovery.
-	failed_jobs → if you’re using queues.
-	migrations → Laravel’s migration tracking table.

