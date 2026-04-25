<!-- l10n-sync: source-file="README.md" -->
# 🎯 Soc Ops — Social Bingo

> **¡Rompe el hielo, haz conexiones, gana en networking!**

Soc Ops es un juego de bingo social interactivo diseñado para encuentros presenciales, eventos de equipo y conferencias. ¡Encuentra personas que coincidan con las pistas, marca tu tarjeta y corre para conseguir 5 en fila!

<p align="center">
  <img src="https://github.com/user-attachments/assets/2c6d0c33-72ec-47e8-b6bc-20837e7d830b" alt="Pantalla de Inicio" width="300" />
  <img src="https://github.com/user-attachments/assets/4785afd4-c22a-4b1c-9b78-64d426c599e9" alt="Tablero del Juego" width="300" />
</p>

<p align="center">
  🎮 <strong><a href="https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/">Jugar</a></strong> •
  📚 <strong><a href="https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/">Ver Guía del Lab</a></strong>
</p>

---

## ✨ Funcionalidades

- 🎲 **Cartones aleatorios** — Cada jugador recibe un arreglo único
- 💾 **Guardado automático** — Continúa donde lo dejaste
- 🏆 **Detección de bingo** — Victoria automática para filas, columnas y diagonales
- 🎉 **Modal de celebración** — Pantalla de victoria con confeti
- 📱 **Mobile-first** — Funciona muy bien en teléfonos en eventos

---

## 🚀 Inicio Rápido

### Requisitos Previos

- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) o superior

### Ejecutar Localmente

```bash
cd SocOps
dotnet run
# Abre http://localhost:5166
```

### Compilar

```bash
cd SocOps
dotnet build
```

### Abrir en GitHub Codespaces (opcional)

Después de crear tu propio repositorio desde esta plantilla:

1. Abre tu repositorio en GitHub
2. Haz clic en **Code** → **Codespaces** → **Create codespace on main**
3. Espera a que la configuración del devcontainer finalice
4. Desde la raíz del repositorio, ejecuta:
   ```bash
   cd SocOps
   dotnet run
   ```

---

## 🎨 Personaliza Tu Juego

Edita `SocOps/Data/Questions.cs` para agregar tus propias preguntas para romper el hielo:

```csharp
public static readonly List<string> QuestionsList = new()
{
    "tiene una mascota",
    "habla más de 2 idiomas",
    "tu pregunta personalizada aquí",
    // ... 24+ preguntas para un tablero completo
};
```

---

## 🛠️ Tecnologías

- **Framework**: Blazor WebAssembly (.NET 10)
- **Estilización**: Utilidades CSS personalizadas (inspiradas en Tailwind)
- **Estado**: Servicios con persistencia en localStorage
- **Deploy**: GitHub Pages via Actions

---

## 📁 Estructura del Proyecto

```
SocOps/
├── Components/     # BingoBoard, BingoSquare, Modals
├── Models/         # Estado del juego & modelos de datos
├── Services/       # Lógica del juego & gestión de estado
├── Data/           # Banco de preguntas
└── wwwroot/        # Recursos estáticos
```

---

## 📚 Guía del Lab

Este proyecto se usa como un taller práctico para construir aplicaciones con GitHub Copilot agents. Sigue paso a paso:

| Parte | Título |
|-------|--------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Descripción General & Lista Rápida |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Configuración & Ingeniería de Contexto |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Frontend Design-First |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Quiz Master Personalizado |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Desarrollo Multi-Agent |

> 📝 Las guías del lab también están disponibles en la carpeta [`workshop/es/`](workshop/es/) para lectura offline.

---

## 🚢 Deploy

El deploy se hace automáticamente en GitHub Pages al hacer push a `main`:
- Tu juego: `https://{usuario}.github.io/{nombre-del-repo}`

---

## 📝 Licencia

MIT — ¡úsalo para tu próximo evento!
