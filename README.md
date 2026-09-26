# Sitio web EntrePelos

Página de EntrePelos (peluquería canina y felina en La Florida) con panel de administración.

## Qué hay en esta carpeta

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La página. No hace falta tocarla. |
| `data/sitio.json` | Todo lo que se puede cambiar: colores, fuentes, textos, precios, fotos, horario y preguntas. |
| `images/` | Las fotos. Las que vienen son de ejemplo y dicen "Reemplaza esta foto". |
| `.pages.yml` | Configuración del panel de administración (Pages CMS). |

## 1. Subir el sitio a GitHub

1. Entra a github.com y crea un repositorio nuevo, por ejemplo `entrepelos`.
2. En el repositorio, pulsa **Add file → Upload files**, arrastra **todo el contenido** de esta carpeta (no la carpeta en sí) y pulsa **Commit changes**.
   - El archivo `.pages.yml` empieza con punto y algunos computadores lo esconden. Si no aparece al arrastrar, créalo en GitHub con **Add file → Create new file**, nómbralo `.pages.yml` y pega su contenido.

## 2. Publicarlo en internet (gratis)

1. En el repositorio: **Settings → Pages**.
2. En "Branch", elige `main` y la carpeta `/ (root)`, y pulsa **Save**.
3. En uno o dos minutos el sitio queda en `https://TU-USUARIO.github.io/entrepelos/`.

> Si el repositorio es privado, GitHub Pages requiere una cuenta de pago. Con repositorio público es gratis (lo que se ve público es el contenido de la página, que igual es pública).

## 3. Entrar al panel de administración

1. Ve a **https://app.pagescms.org** y entra con tu cuenta de GitHub.
2. Autoriza el acceso al repositorio `entrepelos`.
3. Verás **Sitio web EntrePelos** con estas secciones:
   - **Colores y tipografía**: color principal, oscuro, fondo y acento (códigos tipo `#C92A62`) y la fuente de títulos y de texto.
   - **Datos del negocio**: nombre, logo, WhatsApp, Instagram, dirección, nota de Google.
   - **Portada**: título, texto y las dos fotos.
   - **Servicios y precios**: precio por tamaño de cada servicio (ahora dicen `[PRECIO]`).
   - **Galería de fotos**, **Foto de la fachada**, **Horario**, **Preguntas frecuentes**.
4. Cambia lo que quieras y pulsa **Save**. En uno o dos minutos se ve en el sitio.

Solo las personas con acceso a tu repositorio de GitHub pueden entrar al panel.

## Probarlo en tu computador

La página lee `data/sitio.json`, así que abrir `index.html` con doble clic no carga el contenido. Para probar en tu computador, abre una terminal en esta carpeta y ejecuta `python3 -m http.server`, y luego visita `http://localhost:8000`.
