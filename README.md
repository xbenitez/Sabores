# Pasaporte Sabores del Mundo · Extreme Challenge Flavor

Pasaporte virtual de sellos con QR. Es un solo archivo (`index.html`) y no necesita servidor ni base de datos.

## Publicar en GitHub Pages
1. Crea un repositorio, por ejemplo `sabores-del-mundo`, y sube `index.html`.
2. Ve a Settings → Pages → Source: "Deploy from a branch" → rama `main`, carpeta `/ (root)` → Save.
3. Espera 1 o 2 minutos. La página queda en `https://TU-USUARIO.github.io/sabores-del-mundo/`

## Imprimir los QR de los puestos
Abre `https://TU-USUARIO.github.io/sabores-del-mundo/?qr` → "Imprimir / Guardar PDF" (A4, márgenes: ninguno, con gráficos de fondo).
Cada QR apunta automáticamente a la dirección donde está publicada la página.
No compartas el enlace `?qr` con el público.

## Aduana
Botón "Aduana (solo personal)" al final del pasaporte. PIN: `2026`.
Para cambiarlo, busca `const ADUANA_PIN` en `index.html`.

## Reiniciar un pasaporte
Desde la Aduana (con PIN) → "Reiniciar pasaporte". Se borran el nombre y los sellos.
El número de pasaporte (SDM-XXXXX) y los premios ya entregados se conservan:
aunque se vuelvan a ganar, no se pueden canjear otra vez en ese celular.
La Aduana también muestra cuántas veces se reinició.

## Notas
- Los sellos se guardan en el navegador de cada celular (localStorage).
- Si cambias los códigos en `const TOKENS`, vuelve a imprimir los QR.
