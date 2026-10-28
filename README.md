# Pixlet Toys · Catálogo

Coleccionables geek impresos en 3D, capa por capa. Catálogo público: https://pixlettoys.github.io · Instagram [@pixlet.toys](https://instagram.com/pixlet.toys)

Página estática (GitHub Pages). Los clientes arman su pedido en un carrito y lo envían por WhatsApp.

## Editar productos (sin código)
Abre **https://pixlettoys.github.io/admin.html**, entra con tu llave de GitHub y desde ahí
agrega, edita, ordena o quita productos, fotos, banners de la portada y categorías. Al tocar
**Publicar**, todo se guarda en un solo cambio en este repositorio y el catálogo se actualiza en 1 o 2 minutos.

- Pantallas: **Productos**, el editor de cada producto, **Portada** (banners), **Categorías** y
  **Publicar** (lista de cambios con *Deshacer* antes de subirlos).
- Los productos, categorías y banners viven en `productos.json`; las fotos en `img/`.
- Los cambios sin publicar se guardan en el propio dispositivo y se recuperan si la app se cierra.
- La llave es un *fine-grained token* de GitHub solo para este repositorio, con permiso
  **Contents: Read and write**. Se guarda únicamente en tu dispositivo.

## Identidad
Morado noche `#2B1B4D`, lila claro `#F4F0FF` y lima capa `#C6F432` (un solo acento).
Títulos en Bagel Fat One, textos en Figtree (Google Fonts).

## Seguridad
- El catálogo no usa bases de datos ni servicios externos: solo lee `productos.json` de este mismo
  sitio y las fuentes de Google. La administración solo habla con la API de GitHub.
- Todo el texto de `productos.json` se muestra escapado y se valida al cargar.
