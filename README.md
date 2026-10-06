# 🧬 [NOMBRE EMPRESA] — Pitch Deck

Presentación (pitch deck) de la CRO de **Organ-on-Chip para cosmética**, construida como
sitio estático con [reveal.js](https://revealjs.com/). Sin build, sin dependencias locales:
un único `index.html` que GitHub Pages sirve directo.

---

## ✏️ Antes de nada: poné el nombre real

El nombre está marcado como placeholder. Buscá y reemplazá **`[NOMBRE EMPRESA]`** en `index.html`
(aparece en la portada y en el cierre). Mismo criterio con `contacto@[empresa].com` y `www.[empresa].com`.

> Tip: en tu editor, "Reemplazar todo" sobre `[NOMBRE EMPRESA]`.

---

## 👀 Ver en local

No necesitás servidor, pero reveal.js usa el hash de la URL, así que lo ideal es un server estático:

```bash
# opción 1 — abrir directo
open index.html

# opción 2 — server local (recomendado)
python3 -m http.server 8000
# → http://localhost:8000
```

**Navegación:** `←` / `→` o `Espacio` para avanzar · `Esc` para vista general ·
`S` modo presentador (notas) · `F` pantalla completa.

---

## 🚀 Deploy en GitHub Pages

### 1. Subí el repo a GitHub

```bash
git init
git add .
git commit -m "feat: pitch deck organ-on-chip CRO"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/TU_REPO.git
git push -u origin main
```

### 2. Activá Pages

En el repo de GitHub → **Settings** → **Pages**:

- **Source:** `Deploy from a branch`
- **Branch:** `main` · carpeta `/ (root)`
- Guardá.

En ~1 minuto queda publicado en:

```
https://TU_USUARIO.github.io/TU_REPO/
```

> El archivo `.nojekyll` ya está incluido para que Pages sirva el estático sin procesarlo con Jekyll.

---

## 📄 Exportar a PDF

reveal.js exporta a PDF nativo desde Chrome:

1. Abrí la presentación con `?print-pdf` al final de la URL:
   `http://localhost:8000/?print-pdf`
2. `Cmd/Ctrl + P` → Destino **Guardar como PDF** → Márgenes **Ninguno** → Fondos **activados**.

---

## 🎨 Personalización rápida

Todo el tema vive en el bloque `<style>` de `index.html`, en las variables `:root`:

| Variable | Qué controla |
|----------|--------------|
| `--teal` / `--cyan` / `--violet` | Colores de acento y gradientes |
| `--bg` / `--bg-2` | Fondo de la presentación |
| `--ink` / `--ink-soft` | Texto principal / secundario |

Las slides son HTML plano dentro de `<section>`. Cada `<section>` es un slide;
los `<section>` anidados crean sub-slides verticales (navegás con `↓`).

---

## 📑 Estructura del deck

1. Portada
2. Quiénes somos → Visión · Misión · Valores
3. El problema
4. La solución
5. El mercado
6. Modelo de negocio
7. Clientes
8. Benchmarking (competencia)
9. Equipo
10. Proyecto a 5 años (roadmap)
11. Financiación (cuánto / para qué) → cierre
