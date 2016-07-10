﻿# ACRA-Simplest-Backend-With-Alterations



# Setup:

You need a PHP MySQL server. Because of the simplicify of all this you can use webhosts like one.com. We're using that and we cannot use any other backends because of the complexity(of the other backends). (NOTE: No SQL database is needed. Do not use index.php or tosql.php in errors/ if you do not have a database)

Once you have the requirements above, simply add the files to your website. Nothing else is required except:
Change the .htpasswd file in the "errors" folder to fit your requirements. Setting up the password: http://one-docs.com/tools/basic-auth

If you are not using one.com, do not use the long link, in .htaccess instead say(if it is in the same folder): .htpasswd

# Using it:

Link to the file called "report.php" in the first directory in your java file.
Edit the file with your email(if you want to recieve emails) and set the boolean to "true".

You will only recieve mails if the directory is empty. Which means you will only be informed about new crashes since you emptied the logs folder.
!!SQL REQUIRED FOR THIS!!

When you are on your computer open crash/tosql.php. This file will transfer all .txt files in logs to the SQL database.

Remember, for 100% functionality, name the table 'exceptions'. 

In index.php and tosql.php, remember to add:
* Database name
* Database host
* Database username
* Database password

Some places the table is set fixed to 'exceptions', for an instance in the tosql file there is a method that converts all the strings to SQL insert command.

# Features:

* Simple setup
* Easy to use
* You can manually transfer all .txt files into an sql database
* You can view all the entries in the SQL database.
* You can view all .txt files without entering them into the SQL database(very important if your server does not support MySQL.
* If your website does not have databases, remove the database dependant files in errors/


# Notes:

No .htaccess or .htpasswd is created. Create them yourself.

A good idea is to **not** password protect 'submit.php' as that would require you to add password and username in the Java code. Java code 
isn't really that save, even inside the APK. There are multiple ways to break into the APK source code and see it and then your password 
and username would be out in the open. And passwords and username can be exploited.


This project is licenced under Creative Commons 4.0 Attribution Licence.
Feel free to support the project by adding design or improving the PHP code. Keep the links in a simple format so they don't screw up the code.

So this is the simplest PHP SQL backend there is. We can say that on accounts of the few lines of code, the simple install(which really is just to add the files to your website.

ENJOY!
Gamers Cave
