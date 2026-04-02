# 📊 Rastreador de Hábitos 30 Días — PWA

PWA para rastrear 10 hábitos diarios durante 30 días. Funciona offline, se instala en Android y Windows.

## 🚀 Desplegar en GitHub Pages (3 pasos)

### 1. Crear repositorio en GitHub
- Crea un repo nuevo, por ejemplo: `habit-tracker`
- Puede ser público o privado (GitHub Pages gratis solo en públicos)

### 2. Subir los archivos
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/habit-tracker.git
git push -u origin main
```

### 3. Activar GitHub Pages
- Ve a tu repo → **Settings** → **Pages**
- En *Source* selecciona **Deploy from a branch**
- Rama: `main`, carpeta: `/ (root)`
- Guarda → en 1-2 minutos tu app estará en:
  `https://TU-USUARIO.github.io/habit-tracker/`

> **Importante:** Si el repo NO es la raíz del usuario (`TU-USUARIO.github.io`), el SW y el manifest usan rutas relativas, así que funcionan en cualquier subruta.

---

## 📱 Instalar como app

### Android (Chrome)
1. Abre la URL en Chrome
2. Toca el banner "Añadir a pantalla de inicio" o menú ⋮ → "Instalar app"

### Windows (Edge / Chrome)
1. Abre la URL en Edge o Chrome
2. Haz clic en el ícono de instalación (⊕) en la barra de direcciones
3. O menú → "Instalar Rastreador de Hábitos"

---

## 📁 Archivos

| Archivo        | Función |
|----------------|---------|
| `index.html`   | App completa (todo en un archivo, sin build) |
| `manifest.json`| Configuración PWA |
| `sw.js`        | Service worker para modo offline |
| `icon-192.png` | Ícono app (copia del original) |
| `icon-512.png` | Ícono splash screen (copia del original) |

## ✨ Características

- ✅ Sin build, sin Node.js, sin dependencias locales
- ✅ Funciona offline gracias al Service Worker
- ✅ Datos en `localStorage` — sin backend
- ✅ Dark mode
- ✅ Exportar backup JSON
- ✅ Optimizado para Android y Windows
- ✅ Gráfico de progreso diario + torta de días
- ✅ Barras de progreso por hábito
