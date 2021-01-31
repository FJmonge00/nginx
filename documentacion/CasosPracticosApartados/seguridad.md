<img src="../../imagenes/MI-LICENCIA88x31.png" style="float: left; margin-right: 10px;" />

# Seguridad (BETA)

Se recomienda encarecidamente que el tráfico cifrado utilice solo protocolos TLS más nuevos, en lugar de SSL. Ambas versiones de SSL ampliamente disponibles en la actualidad (SSLv2 y SSLv3) tienen fallas de seguridad graves y nunca deben usarse en entornos de producción.

Dejo una pequeña tabla con tipos de cifrados:

TABLA

```nginx
server {
    listen 443 ssl;

    ssl_certificate     /etc/ssl/foo.example.com.crt;
    ssl_certificate_key /etc/ssl/foo.example.com.key;

    ssl_verify_client       on;
    ssl_trusted_certificate /etc/ssl/cachain.pem;
    ssl_ocsp                on; # Enable OCSP validation
```
```nginx
server {
    http {
    ssl_session_cache   shared:SSL:10m;
    ssl_session_timeout 10m;

    server {
        listen              443 ssl;
        server_name         www.example.com;
        keepalive_timeout   70;

        ssl_certificate     www.example.com.crt;
        ssl_certificate_key www.example.com.key;
        ssl_protocols       TLSv1 TLSv1.1 TLSv1.2;
        ssl_ciphers         HIGH:!aNULL:!MD5;
    }
```
https://docs.nginx.com/nginx/admin-guide/security-controls/terminating-ssl-http/
________________________________________
*[Volver atrás...](../CasosPracticos.md)*