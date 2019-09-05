# FIXED Codeigniter 403 Form Post htaccess

```
RewriteEngine On

SecFilterEngine Off
SecFilterScanPOST Off


RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteRule ^(.*)$ index.php/$1 [L]
```
