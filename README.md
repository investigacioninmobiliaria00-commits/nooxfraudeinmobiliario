# Noox Fraude — Landing Page de Interés Público

Una página de alerta ciudadana sobre construcciones irregulares de Noox (Grupo Mypsa S.A. de C.V.) en la Ciudad de México.

## Archivos incluidos

- **index.html** — Página completa, autocontenida (HTML + CSS inline, sin dependencias externas)
- **CNAME** — Configuración del dominio personalizado para GitHub Pages
- **README.md** — Este archivo

## Despliegue en GitHub Pages

### Paso 1: Crear un repositorio en GitHub

1. Ve a [github.com](https://github.com) e inicia sesión en tu cuenta.
2. Haz clic en el icono **+** en la esquina superior derecha y selecciona **New repository**.
3. Nombra el repositorio: `nooxfraudeinmobiliario.com` (o el nombre que prefieras).
4. Selecciona **Public** para que sea visible.
5. Haz clic en **Create repository**.

### Paso 2: Subir los archivos

Opción A: Usando Git desde la línea de comandos

```bash
git clone https://github.com/TU_USUARIO/nooxfraudeinmobiliario.com.git
cd nooxfraudeinmobiliario.com
cp index.html .
cp CNAME .
cp README.md .
git add .
git commit -m "Initial commit: landing page"
git push origin main
```

Opción B: Subir archivos directamente en GitHub

1. En tu repositorio, haz clic en **Add file** → **Upload files**.
2. Arrastra y suelta `index.html`, `CNAME` y `README.md`.
3. Haz clic en **Commit changes**.

### Paso 3: Configurar GitHub Pages

1. Ve a **Settings** en tu repositorio.
2. En el menú izquierdo, selecciona **Pages**.
3. Bajo "Source", selecciona la rama **main** (o **master**, según tu configuración).
4. Haz clic en **Save**.

GitHub Pages ahora desplegará automáticamente tu sitio en `https://TU_USUARIO.github.io/nooxfraudeinmobiliario.com`.

### Paso 4: Conectar el dominio personalizado `nooxfraudeinmobiliario.com`

#### 4.1 Configurar el dominio en GitHub Pages

1. Ve a **Settings** → **Pages** en tu repositorio.
2. Bajo "Custom domain", ingresa `nooxfraudeinmobiliario.com`.
3. Haz clic en **Save**.

GitHub Pages verificará automáticamente que el archivo `CNAME` esté presente (ya lo incluimos).

#### 4.2 Configurar los registros DNS en tu registrador de dominio

Debes apuntar tu dominio `nooxfraudeinmobiliario.com` a los servidores de GitHub Pages. Sigue estos pasos en tu registrador (GoDaddy, Namecheap, etc.):

**Opción A: Usar registros A (recomendado)**

Añade estos cuatro registros A en tu DNS:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

Todos deben apuntar a `nooxfraudeinmobiliario.com`.

**Opción B: Usar registro CNAME (alternativa)**

Si prefieres, puedes crear un registro CNAME:

```
www.nooxfraudeinmobiliario.com  CNAME  TU_USUARIO.github.io
```

Y luego un registro A para el apex:

```
nooxfraudeinmobiliario.com  A  185.199.108.153
```

(Repite con los otros tres IPs de GitHub Pages si es posible).

#### 4.3 Esperar a la propagación DNS

Los cambios DNS pueden tardar entre 15 minutos y 48 horas en propagarse globalmente. Puedes verificar el estado en:

- [whatsmydns.net](https://whatsmydns.net) — ingresa `nooxfraudeinmobiliario.com` y selecciona "A record"

#### 4.4 Habilitar HTTPS

Una vez que el dominio esté configurado correctamente:

1. Regresa a **Settings** → **Pages**.
2. Marca la casilla **Enforce HTTPS**.

GitHub Pages emitirá automáticamente un certificado SSL gratuito (Let's Encrypt).

## Verificación

Una vez completados todos los pasos:

1. Abre `https://nooxfraudeinmobiliario.com` en tu navegador.
2. Verifica que la página se carga correctamente.
3. Comprueba que el certificado SSL es válido (icono de candado verde).

## Estructura del archivo HTML

El archivo `index.html` es completamente autocontenido:

- **HTML5 semántico** con estructura clara
- **CSS inline** — todo el estilo está dentro de la etiqueta `<style>`
- **Sin imágenes externas** — el sitio no depende de recursos externos
- **SEO optimizado** — meta tags, Open Graph, Twitter Cards, JSON-LD (Article, FAQPage, BreadcrumbList)
- **Responsive** — se adapta a móvil, tablet y desktop
- **Accesible** — ARIA labels, jerarquía de encabezados, contraste de colores

## Personalización

Si deseas hacer cambios:

1. Abre `index.html` en un editor de texto (VS Code, Sublime Text, etc.).
2. Busca y reemplaza el contenido que necesites.
3. Guarda los cambios.
4. Sube el archivo actualizado a GitHub (o usa `git push` si trabajas con Git).

GitHub Pages actualizará el sitio automáticamente en unos segundos.

## Aviso legal

Esta página es una publicación anónima de interés público basada en documentos oficiales y resoluciones de autoridades de la Ciudad de México. Véase el aviso legal completo en la página misma.

## Contacto y derecho de réplica

Cualquier persona o empresa aludida en esta página puede ejercer su derecho de réplica. Para ello, contacta a través de los canales que establezca el publicador.

---

**Última actualización:** Julio 2026
