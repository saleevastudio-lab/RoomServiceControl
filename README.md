# Room Service Control · Kimpton Los Monteros

Panel operativo de room service: comandas en tiempo real, estados de cocina y recogidas.

## Despliegue

Sitio estático (GitHub Pages). No requiere build.

- `index.html` — aplicación completa
- `manifest.json` + `icons/icon.svg` — instalable como app (PWA)
- `sw.js` — service worker (network-first)

## Backend

Se conecta al Cloudflare Worker `roomservice-operations-api` (Google Apps Script + Google Sheets).
Acciones usadas: `dashboardLite`, `order`, `startCooking`, `selectDeliveryType`, `pickupOnWay`, `completePickup`.
