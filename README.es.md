<!-- l10n-sync: source-file="README.md" -->
🌐 [Português (BR)](README.pt_BR.md) | [English](README.md)

# 🎯 Soc Ops — Social Bingo

> **¡Rompe el hielo, haz conexiones, gana en el networking!**

Soc Ops es un juego interactivo de bingo social diseñado para encuentros presenciales, eventos de equipo y conferencias. ¡Encuentra personas que coincidan con las preguntas, marca tu tarjeta y corre a conseguir 5 en fila!

<p align="center">
  <img src="https://github.com/user-attachments/assets/2c6d0c33-72ec-47e8-b6bc-20837e7d830b" alt="Pantalla de Inicio" width="300" />
  <img src="https://github.com/user-attachments/assets/4785afd4-c22a-4b1c-9b78-64d426c599e9" alt="Tablero del Juego" width="300" />
</p>

<p align="center">
  🎮 <a href="https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/"><strong>Jugar</strong></a> &nbsp;•&nbsp;
  📚 <a href="https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/"><strong>Ver Guía del Lab</strong></a>
</p>

---

## ✨ Características

- 🎲 **Tableros aleatorios** — Cada jugador recibe una distribución única
- 💾 **Guardado automático** — Retoma donde lo dejaste
- 🏆 **Detección de Bingo** — Detección automática de victorias en filas, columnas y diagonales
- 🎉 **Modal de celebración** — Pantalla de victoria con confeti
- 📱 **Mobile-first** — Funciona perfecto en teléfonos durante eventos

---

## 🚀 Inicio Rápido

### Requisitos Previos
- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) o superior

### Ejecutar Localmente
```bash
cd SocOps
dotnet run
# Abrir http://localhost:5166
```

### Abrir en GitHub Codespaces (opcional)

Después de crear tu propio repo desde esta plantilla:

1. Abre tu repo en GitHub
2. Haz clic en **Code** → **Codespaces** → **Create codespace on main**
3. Espera a que el devcontainer termine la configuración
4. Desde la raíz del repositorio, ejecuta:
   ```bash
   cd SocOps
   dotnet run
   ```

### Compilar
```bash
cd SocOps
dotnet build
```

---

## 🎨 Personaliza tu Juego

### Cambiar Preguntas
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

## 🛠️ Stack Tecnológico

- **Framework**: Blazor WebAssembly (.NET 10)
- **Estilos**: Utilidades CSS personalizadas (inspiradas en Tailwind)
- **Estado**: Servicios con persistencia en localStorage
- **Despliegue**: GitHub Pages mediante Actions

---

## 📁 Estructura del Proyecto

```
SocOps/
├── Components/     # BingoBoard, BingoSquare, Modales
├── Models/         # Estado del juego y modelos de datos
├── Services/       # Lógica del juego y gestión de estado
├── Data/           # Banco de preguntas
└── wwwroot/        # Recursos estáticos
```

---

## 📚 Guía del Lab

Este repositorio también es un taller práctico sobre agentes de GitHub Copilot. ¡Sigue los pasos a continuación para construir el juego con asistencia de IA!

| Parte | Título |
|-------|--------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Descripción General & Lista Rápida |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Configuración & Ingeniería de Contexto |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Frontend Design-First |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Quiz Master Personalizado |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Desarrollo Multi-Agent |

> 📝 Las guías del lab también están disponibles en la carpeta [`workshop/es/`](workshop/es/) para lectura offline.

---

## 🚢 Despliegue

Se despliega automáticamente en GitHub Pages al hacer push a `main`:
- Tu juego: `https://{usuario}.github.io/{nombre-repo}`

---

## 📝 Licencia

MIT — ¡úsalo en tu próximo evento!
