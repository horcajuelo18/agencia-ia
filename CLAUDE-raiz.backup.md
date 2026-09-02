<!--
  COPIA DE SEGURIDAD de PROYECTOS/CLAUDE.md
  Snapshot del 2 de septiembre de 2026.

  El original vive un nivel por encima (PROYECTOS/CLAUDE.md) y NO esta
  versionado en ningun repositorio. Este archivo existe solo para que
  exista una copia con historial en GitHub.

  Si editas el original, vuelve a copiarlo aqui:
    cp ../CLAUDE.md "AGENCIA IA/CLAUDE-raiz.backup.md"
  (y respeta esta cabecera)
-->

# CLAUDE.md — Agencia IA · Alejandro Horcajuelo (2026)

Tres carpetas raíz en PROYECTOS/:

- `AGENCIA IA/` — web de la agencia, demos, dashboard interno, portfolio de práctica, futuros clientes reales
- `PERSONAL/` — proyectos propios: plataforma de clases y canal YouTube (Curio Files)

---

## Estructura de carpetas

```
PROYECTOS/
  AGENCIA IA/
    index.html + vercel.json        ← web pública de la agencia (Vercel · repo: horcajuelo18/agencia-ia)
    guion-primer-contacto.html      ← guión de primer contacto con negocios (uso interno)
    ESTADO_plantilla.md             ← plantilla ESTADO.md para cuando llegue el primer cliente real
    DEMOS/                          ← 31 HTMLs autocontenidos de referencia por tipo de servicio
    dashboard/                      ← dashboard interno React/Vite (repo: horcajuelo18/agencia-ia-dashboard)
    PORTFOLIO/                      ← proyectos de práctica — NO son clientes reales
      bar-las-tablas/web/           ← repo: horcajuelo18/portfolio-bar-las-tablas
      clinica-dental/web/           ← repo: horcajuelo18/WEB-CL-NICA-DENTAL · Vercel
      mana-peluqueros/web/          ← repo: horcajuelo18/WEB-PELUQUERIA · Vercel
      nurr-ink/web/                 ← repo: horcajuelo18/WEB-TATUAJES · Netlify (nurr.ink)
    CLIENTES/                       ← crear cuando llegue el primer cliente real
      [cliente]/
        [servicio]/                 ← web/, chatbot/, landing/, etc.
        ESTADO.md                   ← estado: activo / entregado / pausado · ver plantilla

  PERSONAL/
    clases-particulares/            ← plataforma educativa · repo: horcajuelo18/clases-programacion · Vercel
    VIDEOS IA/                      ← canal YouTube Curio Files · independiente de la agencia
```

**Nuevo cliente real:** crear `AGENCIA IA/CLIENTES/[nombre-cliente]/[servicio]/` + `ESTADO.md` (copiar de `ESTADO_plantilla.md`)

**Nuevo proyecto de práctica:** crear carpeta en `AGENCIA IA/PORTFOLIO/[nombre]/web/`

---

## Flujo de trabajo con clientes

```
/prospeccion → buscar nicho, o preparar la visita a un negocio concreto
       ↓
/auditoria → diagnóstico que demuestra el problema
       ↓
/gestion-cliente → presupuesto → propuesta → ejecución → onboarding → seguimiento
       ↓
/qa-entrega → verificación obligatoria antes de entregar cualquier web
```

`/prospeccion` (modo preparar visita) es el Paso 0 — siempre antes del primer contacto.
`/gestion-cliente` orquesta el resto y avisa de qué skills va a activar en cada paso.

**Las 11 skills propias funcionan en tres fases:** planificar (entrevista → aviso de
dependencias → plan → tu aprobación), implementar y verificar. Ninguna escribe nada
antes de que apruebes. Para encargos que toquen varias skills, usa además el modo
plan nativo (Shift+Tab).

---

## Catálogo de servicios → skills

| Servicio | Skill | Dónde guardar (cliente real) |
|----------|-------|------------------------------|
| **Prospección** (buscar nicho / preparar visita) | `/prospeccion` | `CLIENTES/[cliente]/prospeccion/` |
| **Auditoría** (SEO / negocio / Meta Ads / Google Ads / accesibilidad) | `/auditoria` | `CLIENTES/[cliente]/auditoria-*/` |
| **Webs** (completa / landing / instagram / multipágina) | `/creacion-web` | `CLIENTES/[cliente]/web/` o `/landing/` |
| **Bots** (demo / chatbot / voz / reservas) | `/bots-ia` | `CLIENTES/[cliente]/chatbot/` |
| **Contenido** (calendario / emails) | `/marketing-contenido` | `CLIENTES/[cliente]/calendario/` o `/emails/` |
| Automatizaciones | `/automatizaciones-n8n` | `CLIENTES/[cliente]/automatizacion/` |
| Extensiones Chrome | `/extension-chrome` | `CLIENTES/[cliente]/extension/` |
| Panel financiero | `/dashboard-facturas` | `CLIENTES/[cliente]/facturas/` |
| Seguridad (proyectos con backend) | `/seguridad-web` | — |
| QA previa a entrega | `/qa-entrega` | — |
| Ciclo comercial (presupuesto, propuesta, contrato, onboarding, informe, postventa) | `/gestion-cliente` | `CLIENTES/[cliente]/` |

---

## Naming

**Carpeta cliente:** `[nombre-cliente]` — minúsculas, guiones, sin tildes, sin espacios

Ejemplos: `bar-las-tablas`, `mana-peluqueros`, `nurr-ink`

---

## ESTADO.md — obligatorio por cliente real

Cada carpeta en `CLIENTES/` tiene un `ESTADO.md` (basado en `ESTADO_plantilla.md`) con:
- Estado actual (activo / entregado / pausado)
- Fecha última interacción
- Contacto del cliente
- Servicios contratados con estado y cobro
- URL producción + repo GitHub
- Pendiente cliente / pendiente agencia

---

## Demos de referencia

`AGENCIA IA/DEMOS/` — 31 archivos HTML autocontenidos por tipo de servicio.
Consultar antes de crear un entregable nuevo para mantener el nivel de calidad.

---

## Datos del negocio

- **Email:** aecadro@gmail.com
- **GitHub:** https://github.com/horcajuelo18
- **WhatsApp negocio:** +34 647 471 991
- **Nombre comercial:** Alejandro Horcajuelo / Agencia IA

---

## Repos GitHub

| Repo | Proyecto | Deploy |
|------|----------|--------|
| `horcajuelo18/agencia-ia` | Web pública agencia (`index.html`) | Vercel |
| `horcajuelo18/agencia-ia-dashboard` | Dashboard interno (privado) | Solo local |
| `horcajuelo18/portfolio-bar-las-tablas` | Bar Las Tablas (práctica, privado) | Pendiente |
| `horcajuelo18/WEB-CL-NICA-DENTAL` | Clínica dental (práctica) | Vercel |
| `horcajuelo18/WEB-PELUQUERIA` | Maña Peluqueros (práctica) | Vercel |
| `horcajuelo18/WEB-TATUAJES` | nurr.ink (práctica) | Netlify |
| `horcajuelo18/clases-programacion` | Plataforma clases (personal) | Vercel |

⚠️ Los repos de PORTFOLIO/ (WEB-CL-NICA-DENTAL, WEB-PELUQUERIA, WEB-TATUAJES) siguen conectados a Vercel/Netlify con su historial antiguo. No hacer force-push sin verificar que no se rompe el deploy.

---

## Stack tecnológico por tipo de proyecto

| Proyecto | Stack base |
|----------|------------|
| Webs React | React 18, TypeScript, Vite, Tailwind, Framer Motion |
| Webs Next.js | Next.js 14, TypeScript, Supabase, NextAuth |
| Chatbots | Node.js o Python + Claude API + Telegram/WhatsApp |
| Automatizaciones | n8n (cloud) + Google Calendar/Sheets/WhatsApp |
| Landings / demos | HTML + CSS autocontenido (sin dependencias externas) |
| Extensiones | Manifest V3, vanilla JS, sin frameworks |
| Dashboard interno | React 18, TypeScript, Vite, Tailwind, Framer Motion, Recharts |

---

## Deploy por plataforma

| Plataforma | Proyectos |
|------------|-----------|
| **Vercel** | Web agencia, clínica dental, maña peluqueros, clases particulares |
| **Netlify** | nurr.ink (tatuajes) |
| **n8n cloud** | Automatizaciones y reservas |
| **Railway / Render** | Chatbots con servidor |

---

## Reglas universales

- **Nunca hardcodear** texto en componentes → JSON / arrays de config
- **Nunca inventar datos** de cliente → preguntar siempre
- **Nunca blanco puro** en fondos light mode → mínimo `#dde4f0`
- **Colores** → siempre en `tailwind.config.js`, nunca hex inline
- **Credenciales** → `.env.local` + panel deploy, nunca en código
- **Dark mode** → estrategia `class` en `<html>`, localStorage key `theme`
- **i18n** → localStorage key `lang`, todo en `es.json`/`en.json`, cero hardcoding
- **GSAP** → siempre `fromTo()`, nunca `from()` con React StrictMode
- **Animaciones** → máximo 600ms entrada, no spring por defecto
- **`Write` sin `Read` previo** → siempre leer antes de escribir archivos existentes

---

## Errores recurrentes globales

| Error | Fix |
|-------|-----|
| Estado asíncrono React | Calcular localmente, propagar valor nuevo |
| `NEXTAUTH_URL` localhost en Vercel | `https://dominio.vercel.app` sin `/` final → Redeploy sin caché |
| Grid impar descentrado | `grid-cols-N` = número items + `max-w-* mx-auto` |
| `rm -rf` en Windows | `Remove-Item -Recurse -Force` o `cmd /c rmdir /s /q` |
| SSL localhost Chrome | `http://` sin S, `server: { https: false }` en Vite |
| `gsap.from()` + StrictMode | Usar siempre `gsap.fromTo()` |
| `lucide-react` sin iconos redes sociales | SVGs inline como componentes sin props |
| `lucide-react` export `Github` no existe | Usar `GitBranch` en su lugar |
| `Set` spread TS2802 | `new Set(Array.from(prev).concat(id))` |
| `npx create-next-app` con espacios | Directorio minúsculas sin espacios |
| Tailwind `@apply` + opacidades | No funciona → usar en JSX directo |
| `@import` Google Fonts en index.css | Poner en `<link>` en index.html, no en CSS (PostCSS error) |
| `node_modules` .node nativo bloqueado en Windows | `Stop-Process -Name node -Force` → `cmd /c rmdir /s /q` |
| PowerShell heredoc git commit | Usar `@'...'@` — closing `'@` en columna 0, sin indentación |
| PowerShell operador ternario `? :` | No disponible en PS 5.1 → usar `if/else` |

_Última actualización: 2 de septiembre de 2026_
