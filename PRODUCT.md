# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Contadores públicos colegiados, auditores tributarios, asistentes contables y archivistas del despacho contable Avante Consultores (Perú).
Su situación: gestión diaria de expedientes físicos, respuesta inmediata a fiscalizaciones y requerimientos de SUNAT, auditorías financieras de fin de mes y transferencias periódicas de expedientes activos a cajas de depósito definitivo.

## Product Purpose

Sistema de control, registro, búsqueda y custodia física de archivadores contables de palanca y cajas de almacén muerto para múltiples empresas clientes.
El éxito significa localizar cualquier documento o archivador en menos de 30 segundos, mantener actualizada la trazabilidad física por estanterías ("Izquierda", "Derecha", "Encima") o cajas de almacén ("C1", "C2", etc.), y permitir traslados masivos y exportación fidedigna de padrones.

## Positioning

Frente a gestores de tareas digitales genéricos o hojas de cálculo propensas a errores, es una herramienta de inventario físico especializada en la materialidad del acervo documental peruano: archivadores de palanca de 8 cm lomo ancho, discriminación automática de Compras y Bancos (CyB), liquidaciones SUNAT, detracciones y empaque en cajas numeradas de cartón kraft.

## Operating Context

- Despacho contable en Lima, Perú.
- Estanterías metálicas de consulta activa y depósito de archivo muerto.
- Documentación física probatoria: facturas, boletas, comprobantes de pago, extractos de cuentas bancarias (BCP, BBVA, Scotiabank, Interbank), constancias de detracción y expedientes de importación.
- Dispositivos de uso: PCs de escritorio y laptops en oficina, y teléfonos móviles / tablets para cotejo in situ frente al estante o en almacén.

## Capabilities and Constraints

- Inventario base de 120 archivadores categorizados por Empresa, Mes, Año, Banco, Tipo contable y Ubicación.
- Traducción automática del término contable "CyB" a "Compras y Bancos".
- Vistas operativas triples: Tabla Contable (Libro Mayor), Lomos de Archivador (con código de color y ojal de tiro), y Cajas de Almacén (con cubicaje por caja C1, C2).
- Traslados masivos de ubicación física para lotes filtrados o seleccionados manualmente.
- Generación asistida de descripciones estandarizadas con libertad de edición manual.
- Exportación a CSV con codificación UTF-8 con BOM para visualización perfecta en Excel sin errores de tildes ni la letra "ñ".
- Almacenamiento local autónomo en el navegador (`localStorage`) con opción de restablecimiento al dataset original.
- Funcionamiento 100% offline y compatible para incrustación directa en Google Sites.

## Brand Commitments

- Identidad: "Avante Consultores".
- Logotipo oficial: Monograma geométrico en letra "A" con tipografía serif romana de alta alcurnia y acabado en oro bruñido texturizado sobre azul noche obsidiana.
- Paleta obligatoria: Azul Noche Obsidiana (`#090F1B`, `#0C1424`), Oro Cepillado (`#DFB15B`, `#C59B27`, `#B38622`), Papel Actuario Marfil (`#FAF8F5`, `#F3EFE7`) para evitar saturación y descansar la vista.

## Evidence on Hand

- 120 registros contables reales verificados de empresas como Ssoma, Alcaba, Amasc, Global, JamDermo, Evaneabel, Freddy Estrada, Diana, MJC, Olmos, Henriod, Johana Dreyfus, María Torres, Sea Lilly, Milly.
- Fotografías reales del archivo físico con archivadores ARPERU y OF con rótulos membretados.
- Logotipo oficial vectorizado/renderizado de Avante Consultores.

## Product Principles

1. **Rigor y fidelidad física**: Cada registro en pantalla representa un objeto tangible en la estantería o en una caja de almacén.
2. **Inmediatez a cero fricción**: Filtros instantáneos en cliente, búsqueda en vivo y cifras tabulares alineadas matemáticamente.
3. **Respeto a la identidad institucional**: Sobriedad legal y elegancia contable sin artificios de marketing SaaS ni elementos genéricos de IA.

## Accessibility & Inclusion

- Cumplimiento de ratio de contraste WCAG AA (mínimo 4.5:1 en textos de lectura).
- Objetivos táctiles mínimos de 44px en entornos móviles.
- Navegación por teclado completa con `:focus-visible` definido y soporte para `prefers-reduced-motion`.
