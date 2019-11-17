# App - MVC framework



#### PHP project with MVC framework

```text
public
    index.php
    css
    js
    images
app
    libraries
        core.php
        database.php
        controller.php
    models
    views
    controllers
    helpers
    config : database configuration
    .htaccess 
    bootstrap.php: will require all files we need (like a build)
```

`bootstrap.php` will load php files from library folder \(libraries/Core.php \) which will get the url and reroute it the right controller to display the page `Core.php will` will get the url through GET\['url'\] _.htaccess_

```text
Options -Indexes: hide directory contents when the path is written in the browser.
Ex.
www.yourdomain/css

Options +Indexes : show the folders.
```

_.htaccess inside public folder_ :Configure a php module to reroute any unknown page to index.php

```ruby
<IfModule mod_rewrite.c>
  Options -Multiviews
  RewriteEngine On
  RewriteBase /traversymvc/public
  RewriteCond %{REQUEST_FILENAME} !-d
  RewriteCond %{REQUEST_FILENAME} !-f
  RewriteRule  ^(.+)$ index.php?url=$1 [QSA,L]
</IfModule>
```

_.htaccess inside root folder_ :Configure a php module to reroute any unknown page to public folder

```ruby
<IfModule mod_rewrite.c>
  Options -Multiviews
  RewriteEngine On
  RewriteBase /traversymvc/public
  RewriteCond %{REQUEST_FILENAME} !-d
  RewriteCond %{REQUEST_FILENAME} !-f
  RewriteRule  ^(.+)$ index.php?url=$1 [QSA,L]
</IfModule>
```



