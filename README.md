# Pizza Deprizza — Plataforma de Gestión Operativa

Prototipo de la plataforma en un solo archivo HTML autocontenido, publicado como sitio web estático. Cuatro módulos en tres grupos: Operaciones (Inventarios y Compras), Administración (Ventas, Reportes y Proyecciones; Franquicias y Cumplimiento) y Estratégico (Análisis ejecutivo, con tres accesos: Resumen ejecutivo, Costos y márgenes, Ventas y mezcla).

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

- Los cuatro módulos están regenerados con el estándar DPZ-UX y se abren a pantalla completa desde el menú.
- Cada módulo tiene un selector de rol y sucursal que ajusta lo que se muestra.
- **Inventarios y Compras** incluye Monitoreo de Insumos, Control de masa con registro de mezclas, ajuste de rendimiento de harina y registro de mermas.
- **Ventas** abre una portada con tres reportes: Pulso del día, Proyecciones de venta y Cortes de caja. Usa datos reales de la serie RBG (1 jul – 8 oct 2026).
- **Franquicias y Cumplimiento** permite registrar compromisos con responsable y fecha.
- **Análisis ejecutivo** muestra resumen del mes, recetas y costo teórico por producto, productos más vendidos, venta por estación y la proyección al cierre (RN-22).
- Toda la plataforma usa la paleta `Tema.*` de DPZ-UX-01, fuente Segoe UI y radios de 8, 12 y 16 px. No tiene modo oscuro.
- El contenido de `index.html` es el mismo que el artefacto publicado en claude.ai.
- Los datos de referencia son los del punto de venta Soft Restaurant (`softrestaurant10`), según su diccionario de datos del 9 oct 2026.

## Publicar con GitHub Pages

1. En el repositorio: **Settings → Pages**.
2. En *Build and deployment*, elige **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guarda.
3. El sitio queda disponible en `https://antpathservices-svg.github.io/pizzas/`.

## Ver en local

Abre `index.html` directamente en el navegador; no requiere servidor.
