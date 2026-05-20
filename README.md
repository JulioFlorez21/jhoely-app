# Jhoely · Asistente Personal de IA

## Archivos del proyecto
```
jhoely-app/
├── index.html      ← La app completa
├── manifest.json   ← Configuración PWA
├── sw.js           ← Service worker (funciona offline)
├── icons/
│   ├── icon-192.png   ← Ícono (debes crearlo)
│   └── icon-512.png   ← Ícono grande (debes crearlo)
└── README.md
```

---

## PASO 1 — Crear los íconos

Necesitas dos imágenes PNG:
- `icons/icon-192.png` (192x192 px)
- `icons/icon-512.png` (512x512 px)

Puedes crear un ícono simple en canva.com o usar cualquier imagen cuadrada.
Si no tienes íconos, la app funciona igual pero sin ícono personalizado en la pantalla de inicio.

---

## PASO 2 — Subir a GitHub

1. Ve a github.com y crea una cuenta (gratis)
2. Clic en "New repository"
3. Nombre: `jhoely-app`
4. Selecciona "Public"
5. Clic en "Create repository"
6. Sube los archivos arrastrándolos o usando el botón "Upload files"
7. Sube TODOS los archivos: index.html, manifest.json, sw.js, y la carpeta icons/

---

## PASO 3 — Desplegar en Netlify

1. Ve a netlify.com y crea una cuenta gratis (puedes entrar con tu cuenta de GitHub)
2. Clic en "Add new site" → "Import an existing project"
3. Conecta con GitHub y selecciona el repositorio `jhoely-app`
4. En la configuración:
   - Build command: (dejar vacío)
   - Publish directory: / (o dejar vacío)
5. Clic en "Deploy site"
6. En 1-2 minutos tendrás una URL como: `jhoely-tuNombre.netlify.app`
7. Puedes personalizar el nombre del sitio en Site settings → General

---

## PASO 4 — Obtener tu API Key de Anthropic

1. Ve a console.anthropic.com
2. Crea una cuenta o inicia sesión
3. Ve a "API Keys" → "Create Key"
4. Copia la key (empieza con sk-ant-...)
5. En la app Jhoely, ve a CONFIG y pégala ahí
6. La key se guarda localmente en tu celular

---

## PASO 5 — Instalar en tu celular

### Android (Chrome):
1. Abre tu URL en Chrome
2. Menú (⋮) → "Agregar a pantalla de inicio"
3. Confirma → ¡Ya tienes el ícono de Jhoely!

### iPhone/iPad (Safari):
1. Abre tu URL en Safari (NO en Chrome)
2. Botón compartir (cuadrito con flecha hacia arriba)
3. "Agregar a pantalla de inicio"
4. Confirma → ¡Lista!

---

## PASO 6 — Para alarmas en segundo plano (Android)

La app como PWA no puede sonar con la pantalla apagada.
Para alarmas reales en segundo plano, instala **Tasker** ($3.5 USD en Play Store):

1. Abre Tasker → Perfiles → + → Tiempo
2. Configura la hora de tu alarma
3. Crea una tarea que abra tu URL de Jhoely en Chrome
4. Opcional: usa AutoVoice para el comando "Ok Jhoely"

---

## Funcionalidades

✅ Alarma con saludo personalizado y briefing matutino
✅ Clima en tiempo real (requiere permiso de ubicación)
✅ Noticias del día (requiere API Key)
✅ Lista de tareas persistente
✅ Recordatorios
✅ Chat por texto y voz
✅ Respuestas de IA (requiere API Key)
✅ Funciona offline (clima y noticias requieren internet)
✅ Se instala como app nativa

## Próximamente

⬜ Integración con Notion
⬜ Notificaciones push
⬜ Alarmas en segundo plano nativas
