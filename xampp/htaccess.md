# How to using htaccess

## VirtualHost

Path `D:\xampp\apache\conf\extra\httpd-vhosts.conf`

```bash
...
# NameVirtualHost *:8080
<VirtualHost *:8080>
    DocumentRoot "D:/xampp/htdocs"
    ServerName localhost:8080
    <Directory "D:/xampp/htdocs">
    </Directory>
</VirtualHost>

<VirtualHost *:8080>
    DocumentRoot "D:/xampp/htdocs/project"
    ServerName yii2.local:8080
    <Directory "D:/xampp/htdocs/project">
        Options -Indexes +FollowSymLinks +MultiViews
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>
```
