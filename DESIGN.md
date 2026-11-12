---
name: Avante Consultores — Sistema de Archivo Físico
description: Identidad y lenguaje de diseño para custodia contable y auditoría física
colors:
  primary: "#090F1B"
  primary-container: "#10192A"
  accent-gold: "#DFB15B"
  accent-gold-deep: "#B38622"
  neutral-bg: "#FAF8F5"
  surface: "#FFFFFF"
  surface-warm: "#F3EFE7"
  ink-primary: "#0D1627"
  ink-secondary: "#334155"
  ink-tertiary: "#475569"
  rule-fine: "#E6DFD3"
  rule-medium: "#D5CBBC"
  kraft-box: "#C29B38"
typography:
  display:
    fontFamily: "Newsreader, Iowan Old Style, Apple Garamond, Georgia, serif"
    fontSize: "1.75rem"
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: "-0.015em"
  title:
    fontFamily: "Newsreader, Iowan Old Style, Apple Garamond, Georgia, serif"
    fontSize: "1.25rem"
    fontWeight: 600
    lineHeight: 1.3
    letterSpacing: "0em"
  body:
    fontFamily: "Plus Jakarta Sans, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "0.85rem"
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: "0em"
  data-num:
    fontFamily: "Newsreader, Georgia, serif"
    fontSize: "1.85rem"
    fontWeight: 500
    lineHeight: 1
    letterSpacing: "-0.02em"
rounded:
  sm: "4px"
  md: "8px"
  lg: "12px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
components:
  button-primary:
    backgroundColor: "{colors.accent-gold}"
    textColor: "{colors.primary}"
    rounded: "{rounded.sm}"
    padding: "8px 16px"
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.ink-secondary}"
    rounded: "{rounded.sm}"
    padding: "8px 16px"
  card-spine:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.sm}"
    padding: "20px"
---

# Design System: Avante Consultores — Archivo Físico

## Overview

El sistema visual de **Avante Consultores — Registro & Custodia Documental** está diseñado para el modo **Operate**: una herramienta de trabajo intensivo para contadores y auditores. Evita por completo la estética genérica de tarjetas flotantes grises de SaaS y los degradados de marketing, sustituyéndolos por la dignidad material del archivo físico contable: vinilo martillado, filetes de libro mayor, papel actuario libre de ácido y el oro bruñido del sello institucional de la firma.

## Colors

La paleta se deriva de la insignia corporativa de Avante Consultores:

- **Azul Noche Obsidiana (`#090F1B`, `#10192A`)**: Base estructural en modo nocturno, color del panel lateral y del vinilo de los archivadores.
- **Oro Bruñido Contable (`#DFB15B`, `#B38622`, `#C59B27`)**: Acentos de prestigio, sello notarial, monograma "A" y confirmación de acciones principales.
- **Papel Actuario Marfil (`#FAF8F5`, `#F3EFE7`)**: Lienzo diurno de lectura prolongada libre de fatiga visual; no es blanco hospitalario ni crema saturado de IA.
- **Tinta Tipográfica de Alta Densidad (`#0D1627`, `#334155`)**: Contraste estricto WCAG AA (>5.5:1) para cifras y datos contables.
- **Cartón Kraft Corrugado (`#C29B38`, `#8C6527`)**: Tono distintivo para las cajas de depósito de archivo muerto.

## Typography

Se utiliza una combinación dual con propósito funcional estricto:

- **Newsreader (Serif Display Editorial)**: Aporta la autoridad solemne de un acta notarial o libro de balances. Utilizada en títulos, cabecera institucional y cifras de balance.
- **Plus Jakarta Sans (Grotesca de Cifras Tabulares)**: Optimizada con `font-variant-numeric: tabular-nums` y `font-feature-settings: "tnum"`. Garantiza que todos los números de folios, años (2023–2026), bancos y cajas compartan exactamente el mismo ancho de columna.

## Layout

- **Estructura de Panel Dual**:
  - **Barra Lateral de Navegación Física (`aside.app-sidebar`)**: Búsqueda en tiempo real, filtro por estanterías (*Izquierda*, *Derecha*, *Encima*, *Almacén* con selector de cajas *C1, C2*), tipos contables (*Compras y Bancos*, *Impuestos SUNAT*, *Ventas*) y selector multi-empresa con contadores en vivo.
  - **Lienzo de Registro (`main.app-main`)**: Cabecera institucional con métricas continuas de balance y conmutador de tres ópticas (*Tabla Contable*, *Fichas de Lomo*, *Cajas de Almacén*).
- **Rhythm & Grid**: Espaciado consistente basado en múltiplos de 8px (8, 16, 24, 32). Ancho de lectura nunca superior a 80 caracteres en notas.

## Elevation & Depth

- **Planitud Actuaria**: La jerarquía se expresa principalmente a través de bordes y filetes finos de encuadernación (`1px solid var(--rule-fine)`), no mediante sombras difusas decorativas.
- **Elevación funcional**:
  - `box-shadow: 0 4px 16px rgba(0, 0, 0, 0.25)` reservada para capas flotantes (barra de acciones masivas, modales y avisos toast).
  - Efectos `:hover` discretos de 2px de elevación para elementos interactivos.

## Shapes

- **Radios sutiles**: Radios de curvatura contenidos de 4px (`--radius-sm`) para botones y celdas, 8px (`--radius-md`) para contenedores principales y modales. Se prohíben las esquinas exageradamente redondeadas de plantillas de IA.
- **Detalle Físico de Lomo**: Cada tarjeta de archivador incluye un ojal metálico inferior de extracción (`.spine-card::after`) y un filete lateral con el código de color de la empresa.

## Components

- **Botón Primario**: Oro bruñido (`#DFB15B`) con texto en tinta azul noche (`#090F1B`) y retroalimentación táctil de pulsación (`transform: scale(0.97)` en `:active`).
- **Botón Secundario**: Fondo transparente o pergamino suave con borde fino y texto en azul pizarra.
- **Barra Flotante de Acciones en Lote**: Emerge desde la base al seleccionar archivadores para traslados masivos instantáneos.
- **Avisos Toast**: Notificaciones efímeras con entrada y salida simétricas aceleradas por GPU.

## Do's and Don'ts

### Do's
- Mantener siempre la alineación de cifras tabulares (`tabular-nums`) en años, folios y bancos.
- Utilizar vocabulario formal de auditoría peruana: "Folio", "Compras y Bancos", "SUNAT", "Custodia".
- Garantizar que cada acción en lote muestre el conteo exacto de archivadores afectados.
- Respetar la dualidad de modo diurno (papel marfil) y modo nocturno (obsidiana con oro).

### Don'ts
- **No** usar tarjetas grises flotantes idénticas ni degradados en títulos.
- **No** colocar flechitas decorativas (`➔`, `→`) al final de resúmenes.
- **No** usar textos en mayúsculas sostenidas para etiquetas informativas.
- **No** usar sombras coloreadas difusas sin desplazamiento físico.
- **No** inventar registros ni romper el enlace de los 120 archivadores originales.
