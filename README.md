# 🐇 Pure-on-Chip — Pitch Deck

> *"Beyond the cell"* — La CRO de **Organ-on-Chip** especializada en cosmética ética.
> Seguridad humana demostrada, cero daño animal.

Presentación (pitch deck) construida como sitio estático con [reveal.js](https://revealjs.com/).
Sin build, sin dependencias locales: un único `index.html` que GitHub Pages sirve directo.

---

## 👀 Ver en local

```bash
# server local (recomendado — reveal.js usa el hash de la URL)
python3 -m http.server 8000
# → http://localhost:8000
```

**Navegación:** `←` / `→` o `Espacio` avanzar · `↓` sub-slides · `Esc` vista general ·
`S` modo presentador (notas) · `F` pantalla completa.

---

## 📄 Exportar a PDF

1. Abrí con `?print-pdf`: `http://localhost:8000/?print-pdf`
2. `Cmd/Ctrl + P` → **Guardar como PDF** → Márgenes **Ninguno** → Fondos **activados**.

---

## 🎨 Personalización

El tema vive en el bloque `<style>` de `index.html`, en las variables `:root`
(paleta tomada del logo: teal `--teal`, verde `--green`, azul `--blue`).
Cada `<section>` es un slide; los `<section>` anidados crean sub-slides verticales.

Imágenes de marca: `logo.png` (portada, cierre y marca de agua) y `certificado.png`
(sello "Tested on Synthetic Human Biology" en la sección de modelo de negocio).

---

## 📑 Estructura del deck

1. Portada
2. Quiénes somos → Visión · Misión · Valores
3. El problema
4. La solución (Skin / Lung / Multi-órgano / IA)
5. El mercado
6. **Modelo de negocio** → Tesis B2B2C · Propuesta de valor dual · El sello · Portafolio ·
   Unit economics · Go-to-Market · Moats · Business Model Canvas
7. Clientes
8. Benchmarking (líderes + nuestra ventaja)
9. Equipo
10. Proyecto a 5 años (roadmap)
11. Financiación (cuánto / para qué) → cierre

---

## 🚀 Deploy

Publicado con GitHub Pages desde la rama `main` (carpeta raíz).
El archivo `.nojekyll` hace que Pages sirva el estático sin procesarlo con Jekyll.
