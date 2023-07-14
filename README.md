Customización v1 BountyHacker
 
# CREANDO UN NUEVO USUARIO (aplicable cuando usamos una vm)

```bash 
sudo su
useradd -m <tu_nombre_de_usuario>
passwd <tu_nombre_de_usuario>
<aca_tu_contraseña>
<repetir_contraseña>
usermod -a -G sudo <tu_nombre_de_usuario>
chsh -s /bin/bash <tu_nombre_de_usuario>
exit
sudo reboot
```

# Luego nos logueamos con nuestras nuevas credenciales

```bash
whoami # Deberia aparecernos nuestro nuevo username
```

# Clonar el repositorio de github

```bash 
git clone https://github.com/emersontech/KaliBspwm
```
Instrucciones bàsicas para utilizar la configuraciòn:

```bash
"""
===========================================================================================================
  ____   _____ _______          ____  __    _____ _                _             _       
 |  _ \ / ____|  __ \ \        / /  \/  |  / ____| |              | |           | |      
 | |_) | (___ | |__) \ \  /\  / /| \  / | | (___ | |__   ___  _ __| |_ ___ _   _| |_ ___ 
 |  _ < \___ \|  ___/ \ \/  \/ / | |\/| |  \___ \| '_ \ / _ \| '__| __/ __| | | | __/ __|
 | |_) |____) | |      \  /\  /  | |  | |  ____) | | | | (_) | |  | || (__| |_| | |_\__ \
 |____/|_____/|_|       \/  \/   |_|  |_| |_____/|_| |_|\___/|_|   \__\___|\__,_|\__|___/
                                                                                         
===========================================================================================================
windows + enter abre terminal 
windows + w cierra terminal
windows + d abre el buscador de aplicaciones
windows hold mover libremente la ventana
windows clic derecho reescalar libremente la ventana
windows + alt + flechas escalar ventana
windows + ctl + flechas mover ventana
control + shift + t abre pestaña en terminal
control shift alt t renombrar pestaña de terminal
control shift w cerrar pestaña de terminal
windows + "1,2,3,4,5,6,7,8,9,0" cambiar de escritorio
windows + shift + "1,2,3,4,5,6,7,8,9,0" cambiar de escritorio la ventana actual al escritorio seleccionado
============================================================================================================
```
 
# Los dot files los puedes modificar en las siguientes rutas.
Para aplicar los cambios de las configuraciones más abajo: WINDOWS + ALT + R

```bash
~/.config/bspwm/bspwmrc <- Aqui se cambian los wallpapers
~/.config/polybar/
~/.config/picom/picom.conf
~/.config/sxhkd/sxhkdrc <- Aqui se cambian los comandos
```
 
# Instalar complementos y programas extras

```bash
sudo apt install htop # Administrador de tareas
sudo apt install gnome-control-center # Para hacer uso de configuraciones
sudo apt install flameshot # Para fotocapturas
sudo apt install redshift # Para filtro de luz azul
sudo apt install seclists
sudo apt install alien # Conversor de archivos TAR.GZ y RPM a .DEB
# Install docker on linux (debian based)
sudo apt install -y docker.io
sudo systemctl enable docker --now
docker
```

# Cambiar el keyboard layout desde la terminal

```bash
setxkbmap es
```
