<!-- l10n-sync: source-file="README.md" -->
# 🎯 Soc Ops — Social Bingo

> **Quebre o gelo, faça conexões, vença no networking!**

Soc Ops é um jogo de bingo social interativo projetado para encontros presenciais, eventos de equipe e conferências. Encontre pessoas que correspondam às dicas, marque seu cartão e corra para conseguir 5 em fila!

<p align="center">
  <img src="https://github.com/user-attachments/assets/2c6d0c33-72ec-47e8-b6bc-20837e7d830b" alt="Tela Inicial" width="300" />
  <img src="https://github.com/user-attachments/assets/4785afd4-c22a-4b1c-9b78-64d426c599e9" alt="Tabuleiro do Jogo" width="300" />
</p>

<p align="center">
  🎮 <strong><a href="https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/">Jogar</a></strong> •
  📚 <strong><a href="https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/">Ver Guia do Lab</a></strong>
</p>

---

## ✨ Funcionalidades

- 🎲 **Cartelas aleatórias** — Cada jogador recebe um arranjo único
- 💾 **Salvamento automático** — Continue de onde parou
- 🏆 **Detecção de bingo** — Vitória automática para linhas, colunas e diagonais
- 🎉 **Modal de celebração** — Tela de vitória com confetes
- 📱 **Mobile-first** — Funciona muito bem em celulares em eventos

---

## 🚀 Início Rápido

### Pré-requisitos

- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) ou superior

### Executar Localmente

```bash
cd SocOps
dotnet run
# Abra http://localhost:5166
```

### Compilar

```bash
cd SocOps
dotnet build
```

### Abrir no GitHub Codespaces (opcional)

Após criar seu próprio repositório a partir deste template:

1. Abra seu repositório no GitHub
2. Clique em **Code** → **Codespaces** → **Create codespace on main**
3. Aguarde a configuração do devcontainer finalizar
4. Na raiz do repositório, execute:
   ```bash
   cd SocOps
   dotnet run
   ```

---

## 🎨 Personalize Seu Jogo

Edite `SocOps/Data/Questions.cs` para adicionar suas próprias perguntas de quebra-gelo:

```csharp
public static readonly List<string> QuestionsList = new()
{
    "tem um animal de estimação",
    "fala mais de 2 idiomas",
    "sua pergunta personalizada aqui",
    // ... 24+ perguntas para um tabuleiro completo
};
```

---

## 🛠️ Tecnologias

- **Framework**: Blazor WebAssembly (.NET 10)
- **Estilização**: Utilitários CSS personalizados (inspirados no Tailwind)
- **Estado**: Serviços com persistência em localStorage
- **Deploy**: GitHub Pages via Actions

---

## 📁 Estrutura do Projeto

```
SocOps/
├── Components/     # BingoBoard, BingoSquare, Modals
├── Models/         # Estado do jogo & modelos de dados
├── Services/       # Lógica do jogo & gerenciamento de estado
├── Data/           # Banco de perguntas
└── wwwroot/        # Recursos estáticos
```

---

## 📚 Guia do Lab

Este projeto é usado como um workshop prático para construir aplicações com GitHub Copilot agents. Siga passo a passo:

| Parte | Título |
|-------|--------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Visão Geral & Lista Rápida |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Configuração & Engenharia de Contexto |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Frontend Design-First |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Quiz Master Personalizado |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Desenvolvimento Multi-Agent |

> 📝 Os guias do lab também estão disponíveis na pasta [`workshop/pt_BR/`](workshop/pt_BR/) para leitura offline.

---

## 🚢 Deploy

O deploy é feito automaticamente no GitHub Pages ao fazer push para `main`:
- Seu jogo: `https://{usuario}.github.io/{nome-do-repo}`

---

## 📝 Licença

MIT — use para o seu próximo evento!
