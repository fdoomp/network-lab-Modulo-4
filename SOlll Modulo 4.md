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

sudo apt install postfix -y

sudo apt install mailutils -y

sudo dpkg-reconfigure postfix

$myhostname, localhost.$mydomain, localhost

sudo nano /etc/postfix/sasl/sasl_passwd 

[smtp.gmail.com]:587 micorreo]

sudo postmap /etc/postfix/sasl/sasl_passwd

ls

ls /etc/postfix/sasl/sasl_passwd

sudo chmod 600 /etc/postfix/sasl/sasl_passwd

sudo chmod 600 /etc/postfix/sasl/sasl_passwd.db

ls /etc/postfix/sasl/

sudo nano /etc/postfix/main.cf

relayhost = [smtp.gmail.com]:587

smtp_use_tls = yes
smtp_tls_note_starttls_offer = yes
smtp_sasl_auth_enable = yes
smtp_sasl_password_maps = hash:/etc/postfix/sasl/sasl_passwd
smtp_sasl_security_options = noanonymous
smtp_tls_CAfile = /etc/ssl/certs/ca-certificates.crt

sudo systemctl restart postfix

sudo systemctl status postfix

echo "Fernando Matos\nMatricula: 20242332" | mail -s "MambruSeFueALaGuerra" correodeprueba


echo "Fernando Matos\nMatricula: 20242332" | mail -s "MambruSeFueALaGuerra" correodelprofesor


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Laboratorios del modulo IV Practica 3


sudo apt install cups

sudo systemctl status cups 

sudo apt install epel-release -y 

sudo apt install cups-pdf 

localhost:631/

cups-pdf (virtual pdf printer)

Make: Generic 

Model: Generic CUPS-PDF Printer (w/options) (en)

192.168.1.11:651


