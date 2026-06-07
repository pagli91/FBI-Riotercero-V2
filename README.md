# FBI Torneos — Tiro Federal Río Tercero

Aplicación web progresiva (PWA) para gestión de puntajes en torneos **FBI 15m** y **FBI Minirifle / PCC** del Tiro Federal Río Tercero.

## 📱 Características

- Gestión completa de tiradores, series y puntajes
- Disciplinas: FBI 15m (Pistola/Revólver) y FBI Minirifle (Minirifle/PCC/Kit Roni)
- Modos de puntuación: 8 series individuales o 4 bloques agrupados
- Tabla de resultados con podio y clasificación por división
- Exportación de resultados como imagen JPG
- **Funciona sin internet** una vez cargada (PWA offline)
- **Instalable** en iPhone y Android como app nativa

---

## 🚀 Deploy en GitHub Pages

### 1. Crear el repositorio

```bash
git init
git add .
git commit -m "FBI Torneos TFRT - versión inicial"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/TU_REPO.git
git push -u origin main
```

### 2. Activar GitHub Pages

1. Ir a **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` / `/ (root)`
4. Guardar → en unos minutos la app estará en:
   `https://TU_USUARIO.github.io/TU_REPO/`

---

## 📲 Instalar en el celular

### iPhone / Safari
1. Abrir la URL en Safari
2. Tocar el ícono de **Compartir** (cuadrado con flecha)
3. Seleccionar **"Agregar a pantalla de inicio"**
4. Confirmar → aparece el ícono del club en el home

### Android / Chrome
1. Abrir la URL en Chrome
2. Tocar el menú (⋮) → **"Agregar a pantalla de inicio"**  
   *O bien: aparece automáticamente un banner "Instalar aplicación"*
3. Confirmar → aparece el ícono del club en el home

---

## 📁 Archivos del proyecto

```
├── index.html            # Aplicación principal
├── manifest.json         # Configuración PWA
├── sw.js                 # Service Worker (offline)
├── icon-192.png          # Ícono Android (192×192)
├── icon-512.png          # Ícono Android HD (512×512)
├── apple-touch-icon.png  # Ícono iOS (180×180)
├── favicon.png           # Favicon navegador (32×32)
└── README.md             # Este archivo
```

---

## 🔄 Actualizar la app

Cada vez que subas cambios al repo, los usuarios verán la nueva versión
automáticamente la próxima vez que abran la app con internet.

Para forzar una actualización del cache, cambiar el número de versión
en `sw.js` línea 2:
```js
const CACHE_NAME = 'fbi-tfrt-v2'; // incrementar versión
```

---

*Desarrollado para el Tiro Federal Río Tercero · FeCoTir*
