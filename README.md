# Pizza Deprizza — Plataforma de Gestión Operativa

Prototipo de la plataforma en un solo archivo HTML autocontenido, publicado como sitio web estático. Siete módulos en tres grupos: Operaciones (Inventarios y Compras, Procesos, Recursos Humanos), Administración (Ventas, Reportes y Proyecciones; Franquicias y Cumplimiento) y Estratégico (Módulo Financiero, Analytics y Dashboard Ejecutivo).

## Estructura

| Archivo | Uso |
|---|---|
| `index.html` | Plataforma de Gestión Operativa (página principal del sitio) |
| `404.html` | Redirige cualquier ruta desconocida a la página principal |
| `.nojekyll` | Indica a GitHub Pages que sirva los archivos tal cual |
| `UX Specs/` | Especificaciones de diseño para Power Apps (DPZ-UX) |
| `deprizza-iconos.zip` | Iconografía de la marca |

## Especificaciones de diseño

| Documento | Archivo | Estado |
|---|---|---|
| DPZ-UX-01 · Menú principal | `UX Specs/Menú principal.html` | v1.1 |
| DPZ-UX-02 · Inventarios y Compras | `UX Specs/Inventarios y Compras.html` | Borrador v1.0 |
| DPZ-UX-05 · Ventas, Reportes y Proyecciones | `UX Specs/Ventas, Reportes y Proyecciones.html` | Borrador v1.0 |

## Estado del prototipo

- **Ventas** abre una portada con tres reportes: Pulso del día, Proyecciones de venta y Cortes de caja. Usa datos reales de la serie RBG (1 jul – 8 oct 2026).
- **Analytics y Financiero** toman sus cifras de ventas del módulo Ventas (mes de referencia: septiembre 2026).
- Toda la plataforma usa la paleta `Tema.*` de DPZ-UX-01, fuente Segoe UI y radios de 8, 12 y 16 px. No tiene modo oscuro.
- Los demás módulos usan datos de ejemplo. Cada uno se regenerará desde su especificación DPZ-UX.
- Los datos de referencia son los del punto de venta Soft Restaurant (`softrestaurant10`), según su diccionario de datos del 9 oct 2026.

## Publicar con GitHub Pages

1. En el repositorio: **Settings → Pages**.
2. En *Build and deployment*, elige **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guarda.
3. El sitio queda disponible en `https://antpathservices-svg.github.io/pizzas/`.

## Ver en local

Abre `index.html` directamente en el navegador; no requiere servidor.
