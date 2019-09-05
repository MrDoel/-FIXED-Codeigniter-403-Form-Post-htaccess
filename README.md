# -FIXED-Codeigniter-403-Form-Post-htaccess

RewriteEngine on
 
SecFilterEngine Off
SecFilterScanPOST Off
 
RewriteCond $1 !^(index\.php|assets|css|js|plugin)
 
RewriteRule ^(.*)$ index.php/$1 [L]
