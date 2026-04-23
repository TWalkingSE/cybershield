# CyberShield — Assistente de Segurança Digital e Privacidade

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![AGENTS.md](https://img.shields.io/badge/AGENTS.md-compatible-blue)](https://agents.md)
[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-15-7c3aed)](.github/skills)
[![Knowledge Base](https://img.shields.io/badge/KB-62%20categorias-0ea5e9)](.github/skills/cybershield-kb)
[![Language](https://img.shields.io/badge/Idioma-PT--BR-009c3b)](#)
[![Last Commit](https://img.shields.io/github/last-commit/TWalkingSE/cybershield)](https://github.com/TWalkingSE/cybershield/commits/main)

> Instruções, skills e base de conhecimento que transformam qualquer IDE com modo agente em um consultor especialista de segurança digital, privacidade online e anonimato na internet.

## O que é

O CyberShield é um conjunto de **custom instructions**, **agent skills** e uma **base de conhecimento** que configuram LLMs em IDEs agentic para atuar como consultor de segurança digital. Toda recomendação é contextualizada no modelo TCP/IP e segue o princípio de *defense in depth*.

O projeto utiliza o padrão aberto **Agent Skills**, compatível com múltiplas IDEs e ferramentas de IA.

### O que está incluso

- **62 categorias** de ferramentas de privacidade e segurança catalogadas
- **15 agent skills** com instruções detalhadas para tarefas especializadas
- **Base de conhecimento** com centenas de ferramentas avaliadas (open-source, auditorias, alertas de incidentes, links oficiais)
- **Formato universal** — funciona com qualquer LLM (GPT-5, Claude Opus, Claude Sonnet, Gemini, etc.)

## IDEs e ferramentas compatíveis

O projeto usa o padrão `AGENTS.md` + `SKILL.md`, reconhecido nativamente por:

| IDE / Ferramenta | Arquivo de regras | Skills | Status |
|---|---|---|---|
| **VS Code + GitHub Copilot** | `AGENTS.md` + `.github/copilot-instructions.md` | `.github/skills/` | ✅ Completo |
| **Google Antigravity** | `AGENTS.md` | `.github/skills/` | ✅ Completo |
| **Windsurf (Cascade)** | `AGENTS.md` + `.windsurf/rules/` | `.github/skills/` e `.windsurf/skills/` | ✅ Completo |
| **Cursor** | `AGENTS.md` + `.cursorrules` | `.github/skills/` | ✅ Completo |
| **Claude Code** | `CLAUDE.md` + `AGENTS.md` | `.github/skills/` e `.claude/skills/` | ✅ Completo |
| **GitHub Copilot CLI** | `AGENTS.md` | `.github/skills/` | ✅ Completo |
| **Kiro** | `AGENTS.md` | `.github/skills/` | ✅ Compatível |

> Todas essas IDEs são forks do VS Code ou compatíveis com a especificação Agent Skills. Extensões, atalhos e temas funcionam normalmente.

## Como usar

1. Clone ou baixe este repositório
2. Abra a pasta na sua IDE com modo agente ativo
3. A IDE carrega automaticamente o `AGENTS.md` e as instruções
4. Faça perguntas sobre segurança digital no chat do agente

### Exemplos de perguntas

```
Qual VPN devo usar?
O Brave Browser é seguro?
Como proteger meu Android?
Quero montar meu kit de privacidade
Como funciona fingerprinting de navegador?
Analise meu modelo de ameaça
```

### Skills disponíveis

Para usar um skill específico, digite `/nome-do-skill` no chat:

| Comando | O que faz |
|---|---|
| `/cybershield-kb` | Consultar a base de conhecimento de ferramentas |
| `/fingerprinting` | Impressão digital de navegadores e dispositivos |
| `/threat-modeling` | Criar modelo de ameaça personalizado |
| `/analise-ferramenta` | Avaliar segurança de uma ferramenta específica |
| `/mapa-tcpip` | Visualizar proteções por camada TCP/IP |
| `/hardening` | Tutorial de proteção para sistemas e dispositivos |
| `/diagnostico-privacidade` | Avaliar nível atual de exposição |
| `/kit-privacidade` | Montar conjunto personalizado de ferramentas |
| `/privacidade-ia` | Proteção de dados em IA e LLMs |
| `/limpeza-digital` | Remoção de dados pessoais e pegada digital |
| `/seguranca-fisica` | Proteção física de dispositivos, RFID, câmeras, roubo |
| `/resposta-incidente` | Protocolo de emergência para contas invadidas e dispositivos comprometidos |
| `/protecao-familiar` | Segurança para crianças, adolescentes e idosos |
| `/privacidade-financeira` | Banco online, cartões virtuais, golpes Pix, CPF vazado |
| `/checklist-viagem` | Segurança em viagens e fronteiras |

## Estrutura do projeto

```
cybershield/
├── README.md
├── LICENSE                                # Licença MIT
├── CHANGELOG.md                           # Histórico de versões (Keep a Changelog)
├── CONTRIBUTING.md                        # Guia de contribuição
├── CODE_OF_CONDUCT.md                     # Contributor Covenant 2.1
├── SECURITY.md                            # Política de reporte de problemas
├── .gitignore
├── AGENTS.md                              # Identidade e regras (padrão universal)
├── CLAUDE.md                              # Ajustes específicos para Claude
├── .cursorrules                           # Resumo de regras para Cursor
├── .github/                               # Arquivos canônicos (universal)
│   ├── copilot-instructions.md            # Regras gerais do projeto
│   ├── ISSUE_TEMPLATE/                    # Templates de issue (bug, KB, skill)
│   ├── PULL_REQUEST_TEMPLATE.md
│   ├── prompts/
│   │   └── cybershield-menu.prompt.md     # Menu interativo
│   └── skills/                            # Skills canônicos (conteúdo completo)
│       ├── analise-ferramenta/
│       │   └── SKILL.md
│       ├── cybershield-kb/
│       │   ├── SKILL.md                   # Índice da base de conhecimento
│       │   └── references/                # 9 arquivos temáticos
│       │       ├── autenticacao-senhas.md
│       │       ├── comunicacao.md
│       │       ├── dados-criptografia.md
│       │       ├── investigacao-educacao.md
│       │       ├── navegadores-busca.md
│       │       ├── produtividade-midia.md
│       │       ├── protecao-endpoint.md
│       │       ├── rede-anonimato.md
│       │       ├── sistemas-plataformas.md
│       │       └── iot-seguranca-fisica.md
│       ├── diagnostico-privacidade/SKILL.md
│       ├── fingerprinting/SKILL.md
│       ├── hardening/SKILL.md
│       ├── kit-privacidade/SKILL.md
│       ├── limpeza-digital/SKILL.md
│       ├── mapa-tcpip/SKILL.md
│       ├── privacidade-ia/SKILL.md
│       ├── threat-modeling/SKILL.md
│       ├── seguranca-fisica/SKILL.md
│       ├── resposta-incidente/SKILL.md
│       ├── protecao-familiar/SKILL.md
│       ├── privacidade-financeira/SKILL.md
│       └── checklist-viagem/SKILL.md
├── .windsurf/                             # Compatibilidade Cascade / Windsurf
│   ├── rules/
│   │   └── cybershield.md                 # Regras sempre ativas no Cascade
│   └── skills/                            # 10 wrappers → `.github/skills/`
└── .claude/                               # Compatibilidade Claude Code
    └── skills/                            # 10 wrappers → `.github/skills/`
```

> Os diretórios `.windsurf/skills/` e `.claude/skills/` contêm apenas **wrappers
> de descoberta** (frontmatter `name`/`description` + ponteiro para o arquivo
> canônico). O conteúdo real dos skills vive em `.github/skills/`, evitando
> duplicação e drift de informação.

## Carregamento progressivo

O projeto não joga 1.740 linhas no contexto de uma vez. Usa três níveis:

| Nível | O que carrega | Quando | Tamanho |
|---|---|---|---|
| **Always-on** | `AGENTS.md` + instruções da IDE | Toda conversa | ~120 linhas |
| **Sob demanda** | Skills (`SKILL.md`) | Quando relevante | ~50-95 linhas cada |
| **Referência** | Arquivos em `references/` | Quando o skill consulta | ~130-354 linhas cada |

## Framework TCP/IP

Toda recomendação é mapeada na camada correspondente:

| Camada | Exemplos |
|---|---|
| **4 — Aplicação** | Navegadores, DNS, e-mail, mensageria, senhas, 2FA, criptografia |
| **3 — Transporte** | VPNs, firewalls, análise TLS |
| **2 — Internet** | Tor, proxies, proteção de IP, I2P |
| **1 — Acesso à Rede** | MAC spoofing, segurança Wi-Fi, proteção física |
| **Transversal** | SOs seguros, hardening, criptografia de disco, chaves físicas |

## Fonte primária

- **"Proteja-se Online: Dicas e Softwares Essenciais para Sua Segurança Digital"** (TWalking, 1ª Edição, Janeiro 2025)
- [PrivacyGuides.org](https://www.privacyguides.org/) · [EFF](https://www.eff.org/) · Auditorias independentes

## Contribuindo

Contribuições são bem-vindas. Ao sugerir ferramentas, inclua: nome, link oficial, se é open-source, plataformas, diferencial e alertas de incidentes (se houver).

## Licença

[MIT](LICENSE)

---

*Privacidade não é ter algo a esconder — é um direito fundamental.*
