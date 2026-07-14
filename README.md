# 🗺️ GeoRuta: Contador de Provincias

**App PWA para rastrear tu progreso de Geocaching en España y Portugal.**

Una aplicación web progresiva 100% offline diseñada para llevar el conteo de provincias/distritos visitados durante un road trip de geocaching por la Península Ibérica.

---

## ✨ Características principales

- **Selección de ubicación**:
  - Países: España 🇪🇸 y Portugal 🇵🇹
  - Provincias/Distritos completos (52 de España + Ceuta y Melilla + 20 de Portugal incluyendo Azores y Madeira)

- **Registro de caches**:
  - Entrada de códigos GC con validación automática (GC + alfanumérico)
  - Conversión automática a mayúsculas

- **Dashboard de progreso**:
  - Contador de provincias visitadas vs. totales
  - Total de caches encontradas
  - Barra de progreso visual

- **Historial**:
  - Lista filtrable y buscable
  - Etiquetas de códigos GC clicables → enlaces directos a `coord.info`
  - Acciones para añadir o eliminar códigos por provincia

- **Sincronización y portabilidad**:
  - Copiar datos en formato compacto (ideal para WhatsApp)
  - Exportar JSON completo
  - Importar datos con fusión o sobrescritura (con confirmación)

- **PWA completa**:
  - Funciona **100% offline**
  - Instalación como app nativa en móvil
  - Icono SVG personalizado (pin de mapa + caja de geocache)

---

## 🛠️ Stack técnico

- **100% estático**: HTML5 + CSS3 + Vanilla JavaScript
- Sin frameworks ni dependencias externas
- Diseñado para **GitHub Pages**
- Persistencia en `localStorage`
- Service Worker + manifest.json
- **Cache busting** con timestamps (evita problemas de caché en móviles)

---

## 📱 Uso

1. Abre `index.html` en cualquier navegador.
2. Selecciona país → provincia.
3. Introduce un código GC (ej: `GC8F2KX`) y pulsa **Añadir Visita**.
4. Todo se guarda automáticamente.

**Para compartir tu progreso**:
- Pulsa **Copiar Datos** → pega directamente en WhatsApp.
- El receptor puede importarlo con **Importar Datos**.

---

## 🚀 Despliegue (GitHub Pages)

1. Sube los archivos:
   - `index.html`
   - `manifest.json`
   - `service-worker.js`
   - `icon.svg`
   - `README.md`

2. En GitHub → Settings → Pages → Source: **Deploy from a branch** → `/ (root)`

3. La app estará disponible en `https://tuusuario.github.io/tu-repo`

---

## 📌 Notas importantes

- La aplicación **no requiere backend** ni conexión una vez instalada.
- El **cache busting** implementado asegura que las actualizaciones se carguen correctamente en dispositivos móviles.
- Los datos se guardan solo en el dispositivo (no se suben a ningún servidor).

---

## 🎨 Estilo

Diseño inspirado en el branding oficial de Geocaching:
- Verde bosque: `#02874d`
- Marrón tierra: `#5f452a`
- Fondos claros y tarjetas redondeadas

---

**¡Buen camino y muchas caches!** 🧭

Proyecto creado como herramienta personal para un road trip de geocaching por España y Portugal.
