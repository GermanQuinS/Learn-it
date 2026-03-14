# 📚 Learn it

![Status](https://img.shields.io/badge/status-active-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![GitHub Pages](https://img.shields.io/badge/hosted%20on-GitHub%20Pages-222?logo=github)
![Vanilla JS](https://img.shields.io/badge/built%20with-Vanilla%20JS-f7df1e?logo=javascript)

> **Organiza tus estudios, sigue tu progreso, domina el contenido con flashcards.**

Learn it es una plataforma de aprendizaje personal construida con HTML, CSS y JavaScript puro. Diseñada para ser genuinamente útil como herramienta de estudio y como proyecto de portafolio sólido.

---

## ✨ Features

| Feature | Descripción |
|---|---|
| ⏱️ **Temporizador Pomodoro** | Modos Pomodoro y personalizado con notificación sonora al completar |
| 📈 **Seguimiento semanal** | Velocímetro de horas con meta configurable y racha de días |
| 📊 **Estadísticas** | Sesiones de hoy, promedio diario, total de horas y racha actual |
| 📝 **Gestión de exámenes** | Agenda exámenes con cuenta atrás y nivel de urgencia |
| ✅ **Gestión de tareas** | Prioridades, materias asociadas y fechas de entrega |
| 📖 **Materias** | Crea y colorea tus materias para organizar tu contenido |
| 🃏 **Flashcards con SM-2** | Repetición espaciada (algoritmo SM-2, igual que Anki) con barajas manuales o generadas por IA |
| 🤖 **Generación con IA** | Genera flashcards desde un PDF o texto usando Gemini AI |
| 🎭 **Modo demo** | Al entrar como invitado se precargan datos de ejemplo realistas |
| 👤 **Perfil editable** | Nombre, carrera, centro educativo, con soporte de modo invitado |
| 📥 **Exportar estadísticas** | Descarga un resumen JSON con todas tus estadísticas de estudio |
| 🌐 **Multiidioma** | Soporte completo para ES, EN, GL, FR y DE |
| 🎨 **Tema claro/oscuro** | Toggle con bombilla animada, preferencia persistente |
| 🔔 **Notificaciones** | Sistema de notificaciones en tiempo real vía Firebase |
| 🐛 **Reporte de bugs** | Los usuarios pueden reportar bugs directamente desde la app |
| 🛡️ **Panel de administración** | Estadísticas, envío de notificaciones y gestión de reportes |

---

## 🖼️ Vista previa

> *Capturas del dashboard en acción:*

```
[Dashboard principal]          [Flashcards SM-2]
┌─────────────────────────┐   ┌─────────────────────────┐
│  ⏱️ Temporizador         │   │  🃏 Matemáticas           │
│      25:00               │   │  ┌───────────────────┐   │
│  [▶ Iniciar] [⏹ Detener] │   │  │ ¿Qué es una       │   │
├─────────────────────────┤   │  │ derivada?          │   │
│  📈 Horas semanales      │   │  └───────────────────┘   │
│     7.3h / 25h  (29%)   │   │  [✗ Mal][~ Difícil]       │
└─────────────────────────┘   │  [✓ Bien][⚡ Fácil]       │
                               └─────────────────────────┘
```

---

## 🛠️ Stack tecnológico

- **Frontend:** HTML5, CSS3, JavaScript ES6+ (Vanilla, sin frameworks)
- **Backend:** [Firebase](https://firebase.google.com/) (Firestore para notificaciones y bugs)
- **IA:** [Google Gemini API](https://ai.google.dev/) (generación de flashcards desde PDF/texto)
- **Hosting:** [GitHub Pages](https://pages.github.com/)
- **Algoritmo de estudio:** SM-2 (Spaced Repetition, mismo que Anki)

---

## 🚀 Ejecutar localmente

No necesitas instalar nada. Solo necesitas un servidor HTTP local para evitar restricciones CORS con los módulos de Firebase.

### Opción 1 — VS Code Live Server
1. Instala la extensión [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
2. Abre el proyecto en VS Code
3. Clic derecho en `index.html` → **Open with Live Server**

### Opción 2 — Python
```bash
# Python 3
python -m http.server 8080
# Abre http://localhost:8080
```

### Opción 3 — Node.js
```bash
npx serve .
```

---

## 📁 Estructura del proyecto

```
Learn-it/
├── index.html        # Pantalla de login + preview de features
├── dashboard.html    # App principal (SPA con sidebar)
├── admin.html        # Panel de administración
└── README.md
```

Toda la lógica, estilos y markup están autocontenidos en cada archivo HTML — sin dependencias de build ni node_modules.

---

## 🗝️ Variables de entorno / Configuración

El proyecto usa claves de API directamente en el frontend (compatible con GitHub Pages). Para uso en producción considera:

| Variable | Descripción |
|---|---|
| Firebase config | En `dashboard.html`, bloque `<script type="module">` |
| Gemini API Key | En `dashboard.html`, constante `GEMINI_KEY` |

> 💡 Firebase está en plan Spark (gratuito). Gemini tiene cuota gratuita generosa.

---

## 🗺️ Roadmap

- [ ] 🎮 Minijuegos educativos (sección en construcción)
- [ ] 📱 PWA / instalable en móvil
- [ ] ☁️ Sincronización con cuenta Google (Firestore por usuario)
- [ ] 📊 Gráficas de progreso histórico
- [ ] 🔔 Recordatorios push para flashcards vencidas
- [ ] 🤝 Barajas compartidas entre usuarios
- [ ] 🌙 Modo enfoque (oculta distracciones del sidebar)

---

## 📄 Licencia

MIT © 2026 [GermanQuinS](https://github.com/GermanQuinS)

---

<p align="center">
  Hecho con ❤️ para estudiar mejor
</p>
