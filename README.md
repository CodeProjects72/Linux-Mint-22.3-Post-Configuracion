# Linux Mint - Post-Configuración

Configuración básica y programas esenciales para una instalación nueva de Linux Mint / Ubuntu.

---

## Actualizar el sistema

> Actualiza la lista de paquetes y todos los programas instalados.

```bash
sudo apt update && sudo apt upgrade
```

---

## Códecs, Tipografías y Utilidades 

> Instalación de códecs multimedia, fuentes de Microsoft, GDebi, Synaptic, compresores/descompresores y drivers de impresora.

Ejecuta el siguiente comando:

```bash
sudo apt-get install -y ubuntu-restricted-extras mint-meta-codecs curl nano wget git ffmpeg ttf-mscorefonts-installer gdebi gdebi-core synaptic p7zip-full p7zip-rar rar unrar printer-driver-all
```

---

## Programas y utilidades

> Aplicaciones de uso diario: multimedia, edición de video, terminal, monitores del sistema y gestor de discos.

```bash
sudo apt install -y cmatrix btop htop mousepad evince eog obs-studio kdenlive qbittorrent vlc tilix gparted
```

### Iconos y Cursores

```bash
sudo apt install -y papirus-icon-theme bibata-cursor-themes
```

---

## Activar el cortafuegos (Firewall)

> Activa y verifica `ufw`, el firewall sencillo de Linux.

Activar:

```bash
sudo ufw enable
```

Ver estado:

```bash
sudo ufw status
```

---

## Limpiar paquetes innecesarios

> Elimina dependencias que ya no se usan y limpia la caché de APT.

```bash
sudo apt autoremove && sudo apt autoclean
```

---

## Listo
