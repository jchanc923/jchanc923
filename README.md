# Sistemas Operativos

## Johan Chan Chinchilla

Universidad Latinoamericana de Ciencia y Tecnología

ULACIT

2022


### Comandos Linux

* ./ VBox Linux Adittion.run
* sudo reboot       Reiniciar 

Ver procesos
* ps-aux       Ver procesos de Usuario con más información 
* top
* htop
* pstree

* sudo apt install htop 

* ps   / man ps    Reporte de procesos

* ps e        Todo
* kill -93    Matar proceso 
* ctrl + c    Salir ...

**** 7/6
* man         Ver información o manual acerca del comando 

* interrumpe proceso / mata terminal
* |   (Pipe)        Concatenar / unir comandos
* ls          Listar datos carpeta
* /bin   /(nombrecarpeta)    Específica carpeta 
* Greg         Búsqueda texto 

ps -aux | grep "firefox"
Ver procesos de mi usuario |concatena| busca el texto ("firefox") en los procesos de mi usuario
 
|       concatenar / unir comandos

ls /bin -l
ls -l    en lista
mkdir JohanCarpeta   Crear carpeta
pwd      cual es la ruta
cd       "Nombre carpeta"    abrir 
cd       devolverse
cd ..    a Home
sudo add user "test"      Agregar new Usuario
sudo passwd test          Cambiar contraseña
sudo userdel test         Eliminar usuario 
su test                   Cambiar de usuario
su                        Iniciar sección en terminal/ Cambiar usuario
WHOAMI

nano                      Abrir txt
sudo su                   Iniciar usuario root

nano archivo.txt          Crear
cat                       Solo mostrar, solo imprimir




Comandos instalación Manjaro ArchLinux
sudo pacman -Syy 
descarga forzada, para ello utilizaremos el gestor de paquetes pacman, para instalar Guest Addition

sudo -i
Ingresar como root

sudo pacman-key  - - refresh-keys
Actualizar los certificados de las firmas PGP de los paquetes pacman

sudo pacman-key  - - populate archlinux
Verificar que las claves maestras se hayan actualizado correctamente

sudo pacman -Scc
Purgar borrando los paquetes guardados y limpiando los repositorios que no se usan

sudo pacman -Syyu
Forzar actualización paquetes ArchLinux

sudo reboot
Reiniciar

sudo pacman -Sy virtualbox-guest-utils 
Descargar paquetes Guest Addition si el otro no funcionó  

sudo systemctl reboot
Reiniciar sistema versión ctl

lsmod
Muestra información de los módulo

grep -i     ¨            ¨
Es utilizado para búsqueda de texto

lsmod | grep -i vbox 
Concatenamos los dos comandos, colocamos vbox para corroborar que tengamos vboxguest.

sudo pacman -S unrar zip unzip p7zip gzip bzip2
Instalar los paquetes que comprimen y descomprimen archivos con Zip.

sudo pacman -S yay
Instalar el repositorio AUR (Arch User Repository)

sudo yay -S --needed base-devel
Actualizar los paquetes del repositorio previamente de instalado

yay -S google-chrome
Instalar paquetes yay para instalar google-chrome 

sudo pacman -S apache.
Instalar, configurar y ejecutar Apache

sudo systemctl enable httpd
Iniciar el servicio en el arranque

sudo systemctl restart httpd
Reiniciar servicio

sudo systemctl status httpd
Verificamos el estado finalmente del servicio

sudo nano /srv/http/index.html
Modificar el archivo html que se acaba de crear, lo encontramos en la ubicación /srv/http/index.html 

nano
Abrir el archivo en archivo de texto y modificarlo
sudo pacman -S neofetch

Instalar Neofetch no servirá para visualizar de forma gráfica en consola información de la distribución

uname -a
Ver la versión o el nombre del kernel que está utilizando mi maquina o disponemos
sudo useradd -m ¨nombreusario¨ -G wheel -p  ¨contraseña¨  

Crear nuevo usuario, -G es para asignarle grupo y -p para asignarle contraseña en el mismo comando 

cd /home/sistemasoperativos
Cambiar al repositorio de otro usuario

nano archivo5.txt
Crear archivo .txt vacío con el nombre de archivo 

ls / (directorios: /, home, nombreusuario, documentos)
Listar carpetas del directorio usado en el comando

sudo mkdir diruno
Crear carpeta con el nombre diruno, en la ubicación prevista

ls
Listar archivos en carpeta seleccionada

rm /(ruta y nombre de usuario: /home/johanc923/dirdos/archivo.sh)
Borrar archivo especificado en ruta

ls/bin > archivo1.txt
Guardamos la salida del comando en un txt llamado archivo1.txt usando el símbolo de mayor

cp/etc/profile | HOME/dir003/dircuatro/ > archivo3.txt
##ERROR## Quería concatenar los dos comandos y guardarlos en el archivo3.txt, para 
guardar la salida, pero no me funcionó


