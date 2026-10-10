# PALOMITASX

Sitio de una sola página creado con Astro para mostrar sabores, precios de referencia, paquetes y cotización por WhatsApp.

## Requisitos

- Node.js 22.12 o superior
- npm 9.6.5 o superior

## Arranque

```sh
npm install
npm run dev
```

Para generar la versión de producción:

```sh
npm run build
npm run preview
```

## Estructura

- `src/pages/index.astro`: página, menú, precios, carrito y acciones de WhatsApp.
- `src/layouts/Layout.astro`: estructura HTML y metadatos globales.
- `src/styles/global.css`: estilos ordenados y puntos de adaptación para móvil, tableta y escritorio.
- `public/favicon.svg`: icono del sitio.
- `astro.config.mjs`, `tsconfig.json`, `package.json` y `package-lock.json`: configuración e instalación reproducible.

## Personalización

- Los sabores y precios se editan al inicio de `src/pages/index.astro` en los arreglos `savory` y `sweet`.
- La lista refleja los tamaños CH, MD, G y XL del catálogo. Los sabores que no aparecen ahí y los paquetes son propuestas editables.
- Los iconos actuales son ilustraciones provisionales. Reemplaza los emojis de cada sabor por imágenes propias en `public/` cuando estén listas.
- Actualiza `waNumber` dentro del script de la página con el número de WhatsApp del negocio, en formato internacional sin `+` ni espacios.

Los precios del PDF se conservaron como referencia; confirma los precios actuales antes de publicar.
