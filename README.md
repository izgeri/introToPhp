# introToPhp

This repo contains some example projects that start out with just plain a HTML form, cover using HTML / PHP / JS, and start to build a basic CMS.

The main project is in cms.zip. To run it, you're going to need to install Apache, MySQL, and PHP - depending on your computer's operating system, that means you'll need MAMP (Mac), WAMP (Windows), or LAMP (Linux). Your best bet is to do a web search for "how to install [m/w/l]amp" for instructions. You'll also need to:

- Copy the cms code (in cms.zip) to the www directory for your webserver. You can find this path in the [m|w|l]amp application settings.
- Check the port in conn.php and make sure it matches the port you selected for MySQL when you set it up
- Add a mysql user. This user should match what is specified in conn.php. Open phpMyAdmin (installed with the [m|w|l]amp software) and click on the users tab. Click the "Add User" link and create the user "demo". Generate the SHA1 hashed password with http://localhost/cms/generatePasswordHash.php Also, check "global privileges".
- Create a new database. In the left column of phpMyAdmin, click "new" and enter "cms" into the database name field.
- Load the tables required for the CMS. Download the cms.sql file attached to this email. You can use the import tab in phpMyAdmin to load the tables into the database with the cms.sql file. Or you can run the import in a terminal:
  - mysql -u adminUser -h localhost -p cms < cms.sql
- You may also want to download one of the available open source software for editing computer code, like the Sublime text editor. Once you've done that, you should be ready to start editing the CMS!

Here are some good resources for continuing to learn about this stuff:

- Take online courses at codecademy.com
- Actually download these files and try to play with them on your own!
- If you're working on this and you get stuck, it really does help to Google around for help. You can get useful information from questions other people have asked on stackoverflow.com and from php.net and dev.mysql.com.
