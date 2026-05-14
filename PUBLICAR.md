# Cómo publicar la landing — Guía rápida

El repo local ya está inicializado y con el primer commit hecho. Solo falta el push y activar GitHub Pages.

## 1. Crear el repo en GitHub (si no existe)

Andá a https://github.com/new y creá un repo con estos parámetros:

- **Owner:** `0rgan1co`
- **Repository name:** `microsclera_pitch`
- **Visibility:** Public (necesario para GitHub Pages gratuito) o Private (requiere plan pago para Pages)
- **NO inicializar** con README, .gitignore ni licencia (porque ya los tenemos local)

## 2. Push desde tu terminal

Abrí Terminal en la carpeta del proyecto:

```bash
cd "/Users/roldanjorgex/claudecowork/microsclerapitch/Microsclera Pitch"
git push -u origin main
```

Si te pide credenciales, usá:
- **Username:** `0rgan1co`
- **Password:** un Personal Access Token (no la contraseña real). Generar en https://github.com/settings/tokens — permisos: `repo` (read/write).

Alternativa más simple si tenés [GitHub CLI](https://cli.github.com/) instalado:

```bash
gh auth login              # solo la primera vez
git push -u origin main
```

## 3. Activar GitHub Pages

1. Andá a https://github.com/0rgan1co/microsclera_pitch/settings/pages
2. En **Build and deployment → Source:** elegir `Deploy from a branch`
3. En **Branch:** elegir `main` y carpeta `/ (root)`
4. Click **Save**
5. Esperar 1-2 minutos. La URL pública será:

   👉 **https://0rgan1co.github.io/microsclera_pitch/**

## 4. Actualizaciones futuras

Cuando quieras cambiar la landing, hacer en Terminal:

```bash
cd "/Users/roldanjorgex/claudecowork/microsclerapitch/Microsclera Pitch"
git add .
git commit -m "Update: [describir cambio]"
git push
```

GitHub Pages se actualiza automáticamente en ~1 minuto.

## 5. Custom domain (opcional)

Si tenés dominio propio (ej: `microsclera.com`):

1. En el dashboard de tu proveedor de DNS agregar un `CNAME` apuntando a `0rgan1co.github.io`
2. En Settings → Pages → Custom domain: poner tu dominio y guardar
3. Tildar **Enforce HTTPS**

---

## Estado actual del repo local

- ✅ Git inicializado en branch `main`
- ✅ Remote configurado: `https://github.com/0rgan1co/microsclera_pitch.git`
- ✅ Commit inicial hecho: `425f1a7 Initial commit: landing v1`
- ⏳ Pendiente: push (requiere auth en tu Mac)
- ⏳ Pendiente: activar Pages desde la UI de GitHub
