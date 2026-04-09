# Dicremex Website

Sitio web estático de presentación para Dicremex, una empresa de servicios de software, consultoría e inteligencia artificial en México con experiencia local e internacional.

## Qué incluye

- Landing page responsiva en HTML y CSS.
- Presentación de servicios de software, consultoría, IA y herramientas productivas.
- Portafolio con dos soluciones destacadas:
  - Bot de finanzas personales.
  - Directorio de proveedores para residenciales.
- Sección de quiénes somos.
- Redes y contacto.
- Formulario temporal de contacto hacia `dresendi@gmail.com`.
- Aviso de privacidad.
- Configuración básica para despliegue en Vercel.

## Estructura

- `index.html`: contenido principal del sitio.
- `styles.css`: estilos visuales y responsive.
- `vercel.json`: configuración de despliegue y headers en Vercel.

## Desarrollo local

Como es un sitio estático, puedes abrir `index.html` directamente en el navegador o servirlo con cualquier servidor estático.

Ejemplo con PowerShell y Python:

```bash
python -m http.server 8000
```

Luego abre:

```text
http://localhost:8000
```

## Formulario de contacto

El formulario actual usa `formsubmit.co` para enviar mensajes de forma temporal a:

```text
dresendi@gmail.com
```

Esto permite recibir contactos sin backend propio. Más adelante se puede reemplazar por una integración más robusta con Vercel Functions, Resend, un CRM o un servicio de automatización.

## Despliegue en Vercel

Este proyecto está preparado para funcionar como sitio estático en Vercel.

Buenas prácticas aplicadas:

- `cleanUrls` habilitado.
- `trailingSlash: false`.
- Headers básicos de seguridad.
- Cache agresivo para `styles.css`.

Pasos típicos:

1. Importar el repositorio en Vercel.
2. Mantener la rama `main` como producción.
3. Verificar que el dominio, metadata y enlaces de contacto estén correctos.
4. Hacer una prueba manual del formulario después del primer deploy.

## Siguientes mejoras sugeridas

- Sustituir enlaces temporales de WhatsApp, LinkedIn e Instagram por los reales.
- Agregar favicon e imagen Open Graph.
- Mover la tipografía a assets locales si se quiere depender menos de Google Fonts.
- Reemplazar el correo temporal por un flujo propio con dominio y analítica de leads.
