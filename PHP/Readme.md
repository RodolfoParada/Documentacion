- [Volver al Inicio](../README.md)

<aside>
</aside>

**Como instalar PHP**
```instalar PHP
sudo apt install php
```


**Como crear un proyecto en laravel**
```
composer create-project --prefer-dist laravel/laravel nombre-del-proyecto
```
**Configuraciones**
```configuracion en consola
sudo chown -R www-data:www-data .
```
```configuracion en consola
sudo chmod -R 755 storage/
```

**deforma Global se intala**
```
sudo apt install gedit
```

**Luego tambien de forma global los siguietes comandos se debe abrir un archivo**
```configuracion en consola
sudo chown -R www-data:www-data .
```
```configuracion en consola
sudo chmod -R 755 storage/
```

**Una vez que se abre el archivo se debe copiar lo siguiete**
```copiar 
<VirtualHost *:80>
ServeName @localhost
DocumentRoot /var/www/html/nombre-del-projecto/public

<Directory /var/www/html/nombre-del-projecto>
AllowOverride All
</Directory>

ErrorLog ${APACHE_LOG_DIR}/error.log
CustomLog ${APACHE_LOG_DIR}/access.log combined

</VirtualHost>

```


**se levanta xampp con este comando**
```
sudo /opt/lampp/lampp start
```



