# Changelog

Todas as mudanças relevantes deste projeto serão documentadas neste arquivo.

O formato é baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/)
e este projeto segue [Versionamento Semântico](https://semver.org/lang/pt-BR/).

## [Unreleased]

### Added
- **`/seguranca-fisica`**: Novo skill — proteção física de dispositivos, shoulder surfing, evil maid, RFID/NFC, câmeras de segurança locais, roubo de dispositivos.
- **`/resposta-incidente`**: Novo skill — 5 protocolos de emergência: conta invadida, dispositivo comprometido, stalkerware, senha vazada, phishing.
- **`/protecao-familiar`**: Novo skill — DNS familiar, controles parentais por plataforma, proteção de crianças online, golpes contra idosos (Pix, WhatsApp clonado, falso banco).
- **`/privacidade-financeira`**: Novo skill — banco online seguro, cartões virtuais, golpes do Pix, CPF vazado, Monero/CoinJoin, proteção contra SIM Swap.
- **`/checklist-viagem`**: Novo skill — preparação pré-viagem, fronteiras, Wi-Fi de hotel, conectividade (chip/eSIM), seguridade em quartos, mapa de países de vigilância.
- **`iot-seguranca-fisica.md`** (KB): Nova referência da base de conhecimento — IoT, câmeras IP, assistentes de voz, smart TVs, Tasmota, Home Assistant, Zigbee2MQTT, isolação de rede.

---

## [4.0.0] — 2026-04-22

### Added

- **KB v4.0**: Base de conhecimento expandida para 60 categorias com centenas de novas ferramentas.
- **`privacidade-ia/SKILL.md`**: Riscos de RAG, plugins e integrações de terceiros em ferramentas de IA.
- **`limpeza-digital/SKILL.md`**: Template de solicitação GDPR (Art. 17) adicionado.
- **`hardening/SKILL.md`**: Subseção de roteadores mesh (Eero, Google Nest, TP-Link Deco).
- **`kit-privacidade/SKILL.md`**: Orientações para usuários Windows no Kit Avançado.
- **`AGENTS.md`**: Instrução de fallback para IDEs sem suporte nativo a skills.

### Changed

- **`AGENTS.md`**: Versão atualizada de v3.0 para v4.0 (sincronização com KB).
- **`diagnostico-privacidade/SKILL.md`**: Expandido com critérios de avaliação por ferramenta e integração com KB.

### Fixed

- **`referencias/comunicacao.md`**: Skiff Mail marcado como descontinuado (adquirido Notion 2024).
- **`referencias/investigacao-educacao.md`**: Samourai Wallet atualizado com alerta DOJ/prisão fundadores (abril 2024).
- **`referencias/rede-anonimato.md`**: Streisand marcado como legado/arquivado.

---

## [3.0.0] — 2026-04-19

Primeira publicação pública no GitHub. Consolidação do CyberShield sobre o
padrão aberto **Agent Skills** (`AGENTS.md` + `SKILL.md`), com suporte
nativo a múltiplas IDEs com modo agente.

### Added

- **Identidade e regras centrais** em `AGENTS.md` — TCP/IP como espinha dorsal,
  defense in depth, trade-offs explícitos, proporcionalidade ao threat model,
  proibição de fabricar dados técnicos.
- **10 agent skills** em `.github/skills/` com conteúdo canônico:
  - `cybershield-kb` — base de conhecimento com 9 arquivos temáticos
    (autenticação/senhas, comunicação, dados/criptografia,
    investigação/educação, navegadores/busca, produtividade/mídia,
    proteção de endpoint, rede/anonimato, sistemas/plataformas).
  - `fingerprinting`, `threat-modeling`, `analise-ferramenta`,
    `mapa-tcpip`, `hardening`, `diagnostico-privacidade`,
    `kit-privacidade`, `privacidade-ia`, `limpeza-digital`.
- **Wrappers de descoberta** em `.windsurf/skills/` e `.claude/skills/`
  apontando para os arquivos canônicos em `.github/skills/` (sem duplicação
  de conteúdo).
- **Compatibilidade multi-IDE**:
  - VS Code + GitHub Copilot — `AGENTS.md` + `.github/copilot-instructions.md`
  - Google Antigravity — `AGENTS.md`
  - Windsurf (Cascade) — `AGENTS.md` + `.windsurf/rules/cybershield.md`
  - Cursor — `AGENTS.md` + `.cursorrules`
  - Claude Code — `CLAUDE.md` + `AGENTS.md`
  - GitHub Copilot CLI — `AGENTS.md`
  - Kiro — `AGENTS.md`
- **Menu interativo** em `.github/prompts/cybershield-menu.prompt.md`.
- **Carregamento progressivo** em três níveis (always-on / sob demanda /
  referência) para não inflar o contexto.
- **Framework TCP/IP** aplicado a toda recomendação, com mapeamento explícito
  das camadas 1–4 e transversais.

### Notes

- Versões anteriores (1.x, 2.x) foram iterações internas antes da publicação
  pública e não possuem tags correspondentes neste repositório.

---

[Unreleased]: https://github.com/TWalkingSE/cybershield/compare/v3.0.0...HEAD
[3.0.0]: https://github.com/TWalkingSE/cybershield/releases/tag/v3.0.0
