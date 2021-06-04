# ansible-http-authentication
Configure HTTP Authentication
-----------------------------


step 1 : install httpd package

step 2 : copy web page

step 3 : conf httpd : configure auth  /var/www/html
         go to file /etc/httpd/conf/httpd.conf
         in "httpd.conf", in < Director     /var/www/html >
         replace "AllowOverride None"  with  "AllowOveride AuthConfig" using
         "replace" module

step 4 : cd /var/www/html
         create file ".htaccess"

{
step 5 : install package "python36"

step 6 : install module "passlib" with "pip" module
}        [we install "python" on T.N to use "pip" for installing "passlib", ignore
          installing "python" if it is already present there]

step 7 : user/passwd  DB  uding "htpasswd"
         for enabling the http authentication and creating the file "/etc/www.passwd"
         as a database(DB) for storing login details of users.

step 8 : start httpd serices

step 9 : enable firewall for port 80 on T.N

