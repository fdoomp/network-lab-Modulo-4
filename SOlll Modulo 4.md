# network-lab-Modulo-4

Laboratorios del modulo IV Practica 1

su

apt install apache2

cd /var/www/html

ls 

mkdir prueba

cd prueba/

nano index.html

**<center>**

**<h1>Hola Mundo</h1>**

**</center>**

nano /etc/apache2/conf/apache2.conf

**<VirtualHost \*:80>**

**Servername prueba.localhost**

**DocumentRoot /var/www/html/prueba**

**ServerAdmin root@localhost**

**</VirtualHost>**

systemctl restart apache2

ifconfig O ip a 

mkdir credenciales

cd credenciales/
nano index.html

**<center>**

**<h2>Fernando Matos, Matricula: 20242332, Materia: Sistema Operativos III<h2>**

**</center>**

nano /etc/apache/conf/apache2.conf 

**Listen 8080**

**<VirtualHost \*:8080>**

**Servername credenciales.localhost**

**DocumentRoot /var/www/html/credenciales**

**ServerAdmin root@localhost**

**</VirtualHost>**

**systemctl restart apache2**

mi-ip-que-tenga:8080

-------------------------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------------------------

Laboratorios del modulo IV Practica 2
