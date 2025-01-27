i have searched for installing suite crm in cpanel without softaculous in cli . But there is no document available . so i have created this document by manually installing suite crm by myself.

First create a Cpanel account in WHM.
WHM -> MultiPHPManager -> User domain settings -> select the domain -> PHP 8.1
Login to the cpanel account -> MultiPHP INI Editor -> increase the memory_limit : 50M & upload_max_filesize to 20M

Now login in to the server.
switch as the cpanel user and go to the home path of the user.
now move to \public_html folder and wget the software.
wget https://suitecrm.com/download/148/suite87/564667/suitecrm-8-7-1.zip

unzip suitecrm-8–7–1.zip
chown -R user:user .
chmod -R 755 .
Postinstallation:

Create a Database and user in cpanel .
Give the user full privileges
http://domain/public/install.php
cd /home/user/public_html/public/legacy
chmod -R 775 cache custom modules themes data upload
When you type the base url in the browser you will get the index, folders page , it will work only when you type this http://domain/public/install.php
To redirect it to this URL use cpanel built in redirects tool and paste this url http://domain/public/install.php .
Troubleshooting:

If the route checks gets failed in the installation process:

Remove the files in the public_html directory and also delete the hidden files too. (note: the hidden files will not be deleted even if you use rm -rf *)
Do the installation part again
If you get module errors on installation process ,go to whm and download the required apache modules

If you have any questions related to the installation iam happy to help you feel free to contact me

Gmail: rocksn425@gmail.com
