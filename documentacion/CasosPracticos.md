<img src="../imagenes/MI-LICENCIA88x31.png" style="float: left; margin-right: 10px;" />

# Primeros Pasos
<!-- NGINX -T -->
## Instalación

*Si tenemos instalado apache2 tendremos que desabilitarlo...*

```bash
systemctl stop apache2.service 
systemctl disable apache2.service 
```

```bash
apt update
apt-get install nginx -y
systemctl status nginx.service
```

## Versión de Nginx instalado.

```bash
nginx -v
```

## Servicio asociado.

```bash
systemctl status nginx.service
```

## Ficheros de configuración.

```bash
ls /usr/share/nginx/

```

## Configuraciones Avanzadas

### [Página web por defecto](CasosPracticosApartados/paginaWebDefecto.md)
### [Virtual Hosting](CasosPracticosApartados/VirtualHosting.md)
### [Autentificación, Autorización y Control de acceso](CasosPracticosApartados/autenAutoContAcc.md)
### [Seguridad](CasosPracticosApartados/seguridad.md)
________________________________________
*[Volver al índice...](../README.md)*