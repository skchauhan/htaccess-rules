# htaccess-rules



RewriteEngine On
RewriteRule ^test?$ test.php
RewriteRule ^test/([0-9]+)/([0-9a-z]+)$ test.php?id=$1&ip=$2

Remove php extension
RewriteRule ^([^\.]+)$ $1.php [NC,L]


Remove HTML extension
RewriteRule ^([^\.]+)$ $1.html [NC,L]


Change PHP extension to HTML extension
RewriteRule ^(.*)\.html$ $1.php [L] 
