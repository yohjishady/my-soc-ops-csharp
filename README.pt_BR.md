<!-- l10n-sync: source-file="README.md" -->
🌐 [English](README.md) | [Español](README.es.md)

<div align="center">

# 🎯 Soc Ops

### Social Bingo para encontros presenciais

*Encontre pessoas que correspondam às perguntas. Consiga 5 em uma fileira. Ganhe a sala!*

[![Jogar](https://img.shields.io/badge/🎮%20Jogar-Demo%20ao%20vivo-4f46e5?style=for-the-badge)](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/)
[![Guia do Lab](https://img.shields.io/badge/📚%20Guia%20do%20Lab-Workshop-0ea5e9?style=for-the-badge)](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/)

[![.NET](https://img.shields.io/badge/.NET-10.0-512BD4?logo=dotnet)](https://dotnet.microsoft.com/download/dotnet/10.0)
[![Blazor](https://img.shields.io/badge/Blazor-WebAssembly-7C3AED?logo=blazor)](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor)
[![Deploy](https://img.shields.io/badge/Deploy-GitHub%20Pages-22c55e?logo=github)](https://pages.github.com/)

</div>

---

## 🎲 O que é Soc Ops?

**Soc Ops** é um aplicativo web de Social Bingo otimizado para mobile, criado para eventos de networking, dinâmicas de equipe e quebra-gelos. Os jogadores percorrem a sala em busca de pessoas reais que correspondam a cada quadrado ("vai de bicicleta ao trabalho", "tem um talento oculto", "fala 2+ idiomas") e correm para conseguir **5 em uma fileira**.

Mas também é muito mais do que um jogo — é o **ponto de partida de um workshop prático de GitHub Copilot** onde você usará o modo agente de IA para redesenhar, estender e publicar novos recursos em menos de uma hora.

---

## 🚀 Início Rápido

**Pré-requisitos:** [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) ou superior

```bash
# Clone seu fork (substitua pela URL do seu repositório)
git clone https://github.com/seu-usuario/seu-fork.git
cd seu-fork/SocOps
dotnet run
```

Em seguida, abra **http://localhost:5000** no seu navegador. 🎉

> **Prefere a nuvem?** Abra no GitHub Codespaces — tudo está pré-configurado.  
> Clique em **Code → Codespaces → Create codespace on main** e estará pronto em minutos.

---

## 🛠️ Stack Tecnológico

| Camada | Tecnologia |
|--------|------------|
| Framework | [Blazor WebAssembly](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor) |
| Runtime | .NET 10 |
| Estilos | Utilitários CSS personalizados (app.css) |
| Hosting | GitHub Pages (deploy automático ao fazer push para `main`) |

---

## 🤖 Workshop: Construa com GitHub Copilot Agent Mode

Este repositório é a base de um **lab prático de ~1 hora** onde você usará o modo agente do VS Code com GitHub Copilot para transformar o app. Nenhuma experiência prévia com Copilot é necessária.

### O que você aprenderá

| # | Habilidade | O que você fará |
|---|------------|-----------------|
| 1 | **Engenharia de Contexto** | Ensine a IA sobre sua base de código com `.github/instructions` |
| 2 | **Primitivos Agênticos** | Execute agentes em background, cloud agents e fluxos personalizados |
| 3 | **Desenvolvimento Design-First** | Deixe a IA iterar na UI enquanto você guia a visão criativa |
| 4 | **Desenvolvimento Orientado a Testes** | Use agentes TDD para construir novos recursos de forma confiável |

### Guia do Lab

| Parte | Título | Tempo |
|-------|--------|-------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Visão Geral & Lista Rápida | — |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Configuração & Engenharia de Contexto | 15 min |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Frontend Design-First | 15 min |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Quiz Master Personalizado | 10 min |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Desenvolvimento Multi-Agent | 20 min |

> 📝 Os guias do lab também estão disponíveis offline na pasta [`workshop/pt_BR/`](workshop/pt_BR/).

---

## 🏗️ Compilar e Implantar

```bash
# Executar localmente
cd SocOps && dotnet run

# Compilar para produção
cd SocOps && dotnet build
```

Fazer push para `main` → GitHub Actions compila e implanta automaticamente no GitHub Pages.
