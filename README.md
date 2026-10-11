# Cocina del Mundo

Recetas de almuerzo y cena de 19 países. App web instalable (PWA): porciones que recalculan los ingredientes, cronómetro por paso, filtros y modo sin internet.

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La app (diseño y funciones) |
| `recetas.json` | Todas las recetas y países. Acá se agregan las recetas nuevas |
| `manifest.json` | Nombre, colores e íconos para instalarla en el celular |
| `sw.js` | Guarda la app y las recetas para usarla sin internet |
| `icon-*.png`, `apple-touch-icon.png` | Íconos de la app |

## Publicar en GitHub Pages

1. Creá un repositorio nuevo en GitHub (por ejemplo `cocina-del-mundo`).
2. Subí **todos los archivos sueltos, en la raíz del repositorio** (Add file, Upload files).
3. En Settings, Pages: Source "Deploy from a branch", rama `main`, carpeta `/ (root)`. Guardá.
4. Esperá un minuto. El enlace queda así: `https://TU-USUARIO.github.io/cocina-del-mundo/`

## Instalar en el celular

- **Android (Chrome):** abrí el enlace y tocá el botón amarillo de instalar, o el menú y «Instalar app».
- **iPhone (Safari):** Compartir y «Agregar a pantalla de inicio».

## Agregar recetas

Cada receta nueva se completa en `recetas.json` (ingredientes, pasos y tiempos de cada timer) y marcando `"desarrollada": true`. No hace falta tocar `index.html` ni `sw.js`. Al abrir la app con internet, las recetas nuevas se descargan solas.

## Probar en la computadora

No abras `index.html` con doble clic: el navegador bloquea la lectura de `recetas.json`. Usá el enlace de GitHub Pages o, en la carpeta del proyecto, `python3 -m http.server` y entrá a `http://localhost:8000`.
