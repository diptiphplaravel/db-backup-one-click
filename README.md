# db-backup-one-click

1. Install Composer and xxamp on your machine and clone the project in xxamp's htdocs directory

2. Grant RW permission to Bootstrap and Storage folders

3. Then update the composer with "composer update" command.

4. Set below values in .env
Create database and give details as per below
DB_HOST=<DB_HOST>
DB_PORT=<DB_PORT>
DB_DATABASE=<DB_DATABASE>
DB_USERNAME=<DB_USERNAME>
DB_PASSWORD=<DB_PASSWORD>

MYSQLDUMP_PATH=<PATH_To_MYSQLDUMP>

5. That's it! Run the artisan command from the Terminal to see the new backup commands.
	php artisan
	
6. After this command you can see that command is added to list as  backup
		backup:mysql-dump     Dump your Mysql database to a file
		backup:mysql-restore  Restore your Mysql database from a file
		
7. To back up database hit the URL : http://localhost/db-backup-one-click/public/
		
8. You can also take backup of database using below command
		php artisan backup:mysql-dump
