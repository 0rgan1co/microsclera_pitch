# MICROSCLERA — Landing de pitch

Landing one-page (HTML autocontenido) para la presentación de **MICROSCLERA**, la nueva generación de bioinsecticidas basada en microesclerocios.

## Estructura

- `index.html` — Landing completa, single-file (CSS + JS inline, Google Fonts vía CDN).

## Cómo verla localmente

Abrir `index.html` en cualquier navegador moderno. No requiere build.

```bash
open index.html
```

## Cómo publicarla

### Opción 1: GitHub Pages (gratis)

1. Subir el repo a GitHub (este repo).
2. Settings → Pages → Source: `main` branch, folder: `/ (root)`.
3. La URL pública será: `https://0rgan1co.github.io/microsclera_pitch/`.

### Opción 2: Surge.sh

```bash
npx surge index.html microsclera.surge.sh
```

### Opción 3: Netlify / Vercel

Drag & drop de la carpeta en sus dashboards.

## Pendientes (REEMPLAZAR)

Buscar la cadena `[REEMPLAZAR` en `index.html` para encontrar los puntos pendientes de completar:

- Etapa de la empresa (Pre-seed / Seed)
- Fuentes de las stats (FAO, CABI, etc.)
- Datos de costo por hectárea
- Citas normativas específicas
- Papers publicados, patentes en trámite
- Hectáreas / partners de field-trials
- Nombres y credenciales del equipo (3 personas más)
- Logos institucionales (CONICET, universidad, INTA, GRIDX)
- Métrica de impacto escalado
- Emails de contacto

## Decisiones de diseño

Bio-tech sobrio: paleta verdes/tierra (off-white papel, verde bosque, soil/tierra), tipografía Fraunces (serif moderna) para titulares + Inter para cuerpo. Estructura basada en el 3-Minute Pitch Template (Hero → Problema broader → Problema limitation → ¿Por qué ahora? → Solución → Ventaja técnica → Equipo → Cierre).

---

© Microsclera · 2026
