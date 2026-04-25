<!-- l10n-sync: source-file="README.md" -->
🌐 [English](README.md) | [Português (BR)](README.pt_BR.md)

<div align="center">

# 🎯 Soc Ops

### Social Bingo para encuentros presenciales

*Encuentra personas que coincidan con las preguntas. Consigue 5 en fila. ¡Gana la sala!*

[![Jugar](https://img.shields.io/badge/🎮%20Jugar-Demo%20en%20vivo-4f46e5?style=for-the-badge)](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/)
[![Guía del Lab](https://img.shields.io/badge/📚%20Guía%20del%20Lab-Workshop-0ea5e9?style=for-the-badge)](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/)

[![.NET](https://img.shields.io/badge/.NET-10.0-512BD4?logo=dotnet)](https://dotnet.microsoft.com/download/dotnet/10.0)
[![Blazor](https://img.shields.io/badge/Blazor-WebAssembly-7C3AED?logo=blazor)](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor)
[![Deploy](https://img.shields.io/badge/Deploy-GitHub%20Pages-22c55e?logo=github)](https://pages.github.com/)

</div>

---

## 🎲 ¿Qué es Soc Ops?

**Soc Ops** es una aplicación web de Social Bingo optimizada para móviles, diseñada para eventos de networking, dinámicas de equipo y rompehielos. Los jugadores recorren la sala buscando personas reales que coincidan con cada casilla ("va al trabajo en bici", "tiene un talento oculto", "habla 2+ idiomas") y corren por conseguir **5 en fila**.

Pero también es mucho más que un juego — es el **punto de partida de un workshop práctico de GitHub Copilot** donde usarás el modo agente de IA para rediseñar, extender y publicar nuevas funcionalidades en menos de una hora.

---

## 🚀 Inicio Rápido

**Requisitos previos:** [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) o superior

```bash
# Clona tu fork (reemplaza con la URL de tu repositorio)
git clone https://github.com/tu-usuario/tu-fork.git
cd tu-fork/SocOps
dotnet run
```

Luego abre **http://localhost:5000** en tu navegador. 🎉

> **¿Prefieres la nube?** Abre en GitHub Codespaces — todo está preconfigurado.  
> Haz clic en **Code → Codespaces → Create codespace on main** y estás listo en minutos.

---

## 🛠️ Stack Tecnológico

| Capa | Tecnología |
|------|------------|
| Framework | [Blazor WebAssembly](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor) |
| Runtime | .NET 10 |
| Estilos | Utilidades CSS personalizadas (app.css) |
| Hosting | GitHub Pages (deploy automático al hacer push a `main`) |

---

## 🤖 Workshop: Construye con GitHub Copilot Agent Mode

Este repositorio es la base de un **lab práctico de ~1 hora** donde usarás el modo agente de VS Code con GitHub Copilot para transformar la app. No se requiere experiencia previa con Copilot.

### Lo que aprenderás

| # | Habilidad | Qué harás |
|---|-----------|-----------|
| 1 | **Ingeniería de Contexto** | Enseña a la IA tu codebase con `.github/instructions` |
| 2 | **Primitivas Agénticas** | Ejecuta agentes en background, cloud agents y flujos personalizados |
| 3 | **Desarrollo Design-First** | Deja que la IA itere en la UI mientras tú guías la visión creativa |
| 4 | **Desarrollo Guiado por Tests** | Usa agentes TDD para construir nuevas funcionalidades de forma fiable |

### Guía del Lab

| Parte | Título | Tiempo |
|-------|--------|--------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Descripción General & Lista Rápida | — |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Configuración & Ingeniería de Contexto | 15 min |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Frontend Design-First | 15 min |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Quiz Master Personalizado | 10 min |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Desarrollo Multi-Agent | 20 min |

> 📝 Las guías del lab también están disponibles offline en la carpeta [`workshop/es/`](workshop/es/).

---

## 🏗️ Compilar y Desplegar

```bash
# Ejecutar localmente
cd SocOps && dotnet run

# Compilar para producción
cd SocOps && dotnet build
```

Hacer push a `main` → GitHub Actions compila y despliega automáticamente en GitHub Pages.
