# Bitácora — La Bodega de LLantas

## Sesión: 2026-07-02

### Hallazgos

1. **Dominio**: `labodegadellantas.com` — apuntando al VPS2 (74.208.13.120) con Plesk.
2. **Servidor**: Ubuntu, Apache, Plesk. Directorio raíz: `/var/www/vhosts/labodegadellantas.com/httpdocs/`
3. **Estado inicial**: Página default de Plesk ("Domain Default page").
4. **Crawler Facebook**: Devolvía 403 por falta de `robots.txt` y contenido real.

### Acciones realizadas

- Subida de imagen "Sitio en Construcción" (`sitio-en-construccion.jpg`)
- Reemplazo de `index.html` con página minimalista + Open Graph tags (og:title, og:description, og:image)
- Creación de `robots.txt` permitiendo `facebookexternalhit` y `Twitterbot`
- Creación de `favicon.svg` (ícono de llanta)
- Corrección de ownership de archivos (`labodegadellantas.co_fbz9xzojqw8:psacln`)

### Pendientes

- [ ] Reemplazar "Sitio en Construcción" con el sitio final
- [ ] Agregar SSL/HTTPS si no está configurado
- [ ] Crear contenido real del negocio (catálogo de llantas)
