# Changelog

Todas as mudanças relevantes deste projeto serão documentadas neste arquivo.

O formato é baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/)
e este projeto segue [Versionamento Semântico](https://semver.org/lang/pt-BR/).

## [Unreleased]

### Added
- _(adicione aqui suas mudanças antes do próximo release)_

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
