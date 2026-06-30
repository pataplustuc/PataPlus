# PataPlus Partner - App Android

App nativa Android que carga https://pata-plus-partner.netlify.app/

---

## ⚡ OPCIÓN MÁS FÁCIL: Obtener el APK en 5 minutos con GitHub Actions

### Paso 1 — Crear cuenta en GitHub (gratis)
Ve a https://github.com/signup y creá una cuenta gratuita.

### Paso 2 — Crear repositorio nuevo
1. Hacé clic en **"New repository"** (botón verde)
2. Nombre: `pataplus-app`
3. Dejá todo lo demás por defecto
4. Clic en **"Create repository"**

### Paso 3 — Subir los archivos
1. En la página del repositorio nuevo, clic en **"uploading an existing file"**
2. Arrastrá TODOS los archivos y carpetas de este ZIP
3. Clic en **"Commit changes"**

### Paso 4 — GitHub compila el APK automáticamente
1. Hacé clic en la pestaña **"Actions"** del repositorio
2. Vas a ver el workflow **"Build PataPlus APK"** ejecutándose (tarda ~3-5 min)
3. Cuando termine (✅ verde), hacé clic en el workflow
4. Bajá hasta **"Artifacts"** y descargá **"PataPlus-debug-APK"**

### Paso 5 — Instalar en tu teléfono
1. Descomprimí el ZIP descargado → tenés el archivo `app-debug.apk`
2. Mandátelo a tu teléfono (WhatsApp, email, cable USB, etc.)
3. Abrí el APK en tu teléfono → tocá **"Instalar"**
4. Si aparece "fuentes desconocidas": Configuración → Seguridad → activar "Instalar apps desconocidas"

---

## Características de la app
- Splash screen con logo PataPlus al abrir
- WebView a pantalla completa cargando la web
- Barra de progreso verde durante la carga
- Pull-to-refresh (deslizar hacia abajo para recargar)
- Botón Atrás navega el historial web
- Compatible con Android 5.0+

## Estructura
```
├── app/src/main/
│   ├── java/com/pataplus/app/
│   │   ├── SplashActivity.java   ← Pantalla de inicio con logo
│   │   └── MainActivity.java     ← WebView principal
│   ├── res/
│   │   ├── drawable/logo.png     ← Logo PataPlus
│   │   ├── mipmap-*/             ← Íconos del launcher
│   │   └── layout/               ← Layouts
│   └── AndroidManifest.xml
├── .github/workflows/build.yml   ← Compilación automática en GitHub
└── build.gradle
```
