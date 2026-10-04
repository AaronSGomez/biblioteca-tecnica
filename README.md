# Biblioteca técnica PI5SERVER

Portfolio público de documentación y páginas interactivas creadas durante el
desarrollo y la experimentación con un servidor Raspberry Pi 5.

## Contenido

- Arquitectura y despliegue de Spring Boot para VeriFactu.
- Investigación de SOAP, XML, WS-Security y librerías Dart.
- Contenedorización de Odoo y PostgreSQL.
- Apache como proxy inverso, DuckDNS y certificados Let's Encrypt.
- Aislamiento con Nginx, rate limiting y trazabilidad de peticiones.
- CrowdSec y Firewall Bouncer para defensa perimetral.

La portada está en [`index.html`](./index.html) y las páginas individuales en
[`docs/`](./docs/).

## Ver el sitio

El proyecto es HTML/CSS/JavaScript estático y puede publicarse con GitHub Pages.
No requiere PHP ni un servidor activo. Las páginas cargan algunas librerías
visuales desde CDN cuando el navegador tiene conexión a Internet.

## Seguridad y privacidad

Este repositorio no debe contener:

- tokens de DuckDNS ni claves de API;
- contraseñas, certificados, claves privadas o archivos `.env`;
- logs con direcciones IP públicas o datos de usuarios;
- configuraciones reales que permitan acceder a servicios.

Los valores incluidos en la documentación son ejemplos y placeholders. La
Raspberry Pi está apagada y fuera de uso; aun así, cualquier credencial que
haya sido utilizada históricamente debe revocarse y regenerarse antes de hacer
público el repositorio.

## Licencia

El contenido se publica como portfolio y material educativo. Añade una licencia
explícita si quieres permitir su reutilización.
