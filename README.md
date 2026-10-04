# Biblioteca Técnica PI5SERVER

Biblioteca de documentos técnicos útiles para la programación, arquitectura, infraestructura, seguridad perimetral, microservicios y facturación electrónica (VeriFactu / NovaPay), desarrollada a partir de la experimentación en servidores caseros con **Raspberry Pi 5**.

El proyecto presenta un diseño unificado de manual técnico interactivo, responsivo y enriquecido con diagramas, simuladores y explicaciones detalladas sin perder rigor técnico.

---

## 📚 Estructura y Contenidos

El repositorio consta de un portal de inicio en [`index.html`](./index.html) y siete manuales técnicos interactivos en el directorio [`docs/`](./docs/):

1. **🏛️ [VeriFactu INFO](./docs/verifactu.html)**  
   Guía interactiva sobre integración con la Agencia Tributaria (AEAT), arquitectura del sobre SOAP/XML, firma digital X.509, encadenamiento SHA-256 de registros de facturación y exploración de librerías en Dart/Flutter.

2. **⚙️ [Informe Backend NovaPay](./docs/springbootAPI.html)**  
   Arquitectura REST del núcleo fiscal NovaPay, controlador de enrutamiento regional (Bizkaia/Batuz, Araba/TicketBAI, Gipuzkoa y AEAT), gestión de colas de reintento con Exponential Backoff y persistencia en SQL.

3. **☕ [Arquitectura Spring Boot](./docs/springboot.html)**  
   Diseño del middleware intermedio en Java 17 / Spring Boot para la traducción transparente de JSON a sobres XML/SOAP firmados mediante compilación WSDL-to-POJO (`jaxb2-maven-plugin`).

4. **📦 [Odoo Dockerizado](./docs/dokerizacion.html)**  
   Despliegue ERP Odoo 16 en contenedores Docker, volúmenes de persistencia para PostgreSQL (`pgdata` y `odoo-web-data`), redes aisladas en Docker Compose y configuración de proxy inverso Apache.

5. **🌐 [Multi-dominio y SSL](./docs/duckdnsyssl.html)**  
   Infraestructura de dominios dinámicos con DuckDNS, automatización de scripts de actualización de IP pública, directiva VirtualHost en Apache y renovación de certificados TLS con Certbot / Let's Encrypt.

6. **🛡️ [Búnker Nginx](./docs/nginx.html)**  
   Proxy inverso perimetral con modelo de seguridad Zero Trust, límite de peticiones (`limit_req_zone`), ajuste de timeouts (`client_body_timeout`), prevención de buffer overflow y cabeceras de hardening (HSTS, CSP, X-Frame-Options).

7. **🔒 [CrowdSec y Firewall Bouncer](./docs/securefirewall.html)**  
   Sistema de Prevención de Intrusiones (IPS) adaptativo basado en análisis de logs en tiempo real, comunicación con CrowdSec LAPI y bouncer `cs-firewall-bouncer` para descarte directo de amenazas a nivel de kernel mediante `iptables`.

---

## 🎨 Características de Diseño

- **Estética de Manual Guía**: Formato de documentación limpia, estructurada y visualmente coherente en todos los módulos.
- **Layout Optimizado**: Reestructuración a contenedor ancho (`1140px`) para maximizar la legibilidad en pantallas de escritorio y portátiles.
- **Navegación Fluida**: Barras de retorno rápido al índice (`← Volver al índice`), enlaces al pie de página (`↑ Volver arriba`) y controles flotantes adaptados para dispositivos móviles.
- **Componentes Interactivos**: Gráficos dinámicos con Chart.js, exploradores de código/scaffolding y simuladores de validación de firma y sobres SOAP.
- **Pie de Página Unificado**: Pie compartido en una sola línea en todo el sitio:
  `Biblioteca técnica de AaronSGomez / Github © 2026`

---

## 💻 Despliegue y Visualización

El proyecto está construido completamente con **HTML5, CSS3 y JavaScript ES6+ (Vanilla)**.
- Puede alojarse directamente en **GitHub Pages**, Nginx, Apache o cualquier servidor web estático.
- No requiere dependencias de backend en ejecución (PHP, Node.js ni bases de datos activas).
- Las librerías de soporte (como Chart.js) se cargan desde CDNs oficiales mediante HTTPS.

---

## 🔒 Seguridad y Privacidad

- **Estado del Servidor**: La Raspberry Pi 5 utilizada en la fase experimental se encuentra **apagada y fuera de servicio**.
- **Credenciales y Datos**: Todos los nombres de dominio, tokens de DuckDNS, direcciones IP, certificados digitalizados, archivos `.env` y claves privadas mostrados en los ejemplos son **placeholders ficticios** y no representan secretos reales.

---

## 👤 Autor

**AaronSGomez**  
- Web: [aaronsgomez.es](https://aaronsgomez.es)  
- GitHub: [github.com/AaronSGomez](https://github.com/AaronSGomez)  

© 2026 AaronSGomez. Biblioteca técnica de documentación.
