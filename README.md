# 🍓 Fresa Solidaria Barragán — PWA

App web progresiva para la venta directa de fresa fresca de una familia campesina de **Barragán, Valle (2.900 msnm)**, dentro del *Reto Fresa Solidaria — Salvemos la Cosecha*.

## ¿Qué hace?

- 🧺 **Catálogo con carrito** — cajas de 1, 2 y 5 kg + pedido mayorista para negocios.
- 📊 **Contador de meta semanal** — barra de progreso hacia los 1.800 kg.
- 📍 **Geolocalización GPS** — el cliente comparte su ubicación para la entrega.
- 📲 **Envío de pedido por WhatsApp** — mensaje formateado automáticamente.
- 🏅 **Botón "Aliado Fresa Solidaria"** — para restaurantes, heladerías, panaderías y jugueras.
- 🕐 **Reloj de Colombia (UTC-5)** y campaña con vigencia.
- 🌄 **Sección de historia** de la familia productora.
- ✅ **PWA completa** — manifest, service worker, soporte offline, Open Graph para preview en WhatsApp.
- 🔒 **Aviso Habeas Data** (Ley 1581/2012) en el formulario.

## Archivos

| Archivo | Descripción |
|---|---|
| `index.html` | App principal (todo en un solo archivo) |
| `manifest.json` | Configuración PWA (instalable) |
| `sw.js` | Service worker (offline) |
| `README.md` | Este archivo |

## Configuración rápida

En `index.html`, dentro de `<script>`, edita la sección `CONFIG`:

```js
const WHATSAPP = "573188312581"; // Cristina Arango (con código país, sin +)
const META_KG  = 1800;            // Meta de kilos de la semana
```

**Precios:** edita el arreglo `PRODUCTS` para cambiar valores, cajas y descripciones.

**Contador de meta:** la línea `setGoal(420)` define cuántos kg se han vendido. Cámbiala manualmente cada vez que avancen las ventas, o conéctala a una fuente de datos real más adelante.

**Imágenes (og:image e iconos):** actualmente usan un placeholder. Reemplaza las URLs por una foto real del cultivo/fresa para mejorar el preview en WhatsApp y el ícono instalable.

## Despliegue

1. Sube los 4 archivos a un repositorio en GitHub.
2. Activa **GitHub Pages** (o despliega en **Netlify**) sobre la raíz.
3. Comparte el enlace en el flyer y en redes.

> ⚠️ La PWA es 100% estática y no requiere servidor ni API. Funciona en GitHub Pages sin restricciones.

---

Desarrollada por **Vibras Positivas HM** — Derechos de Autor Reservados
📧 haroldco45@gmail.com · 📱 3117700431
