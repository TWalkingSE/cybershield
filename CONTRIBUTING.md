# Contribuindo com o CyberShield

Obrigado por considerar contribuir! Este projeto é uma base de conhecimento de
segurança digital usada por agentes de IA em diversas IDEs. Qualidade,
precisão e neutralidade importam mais do que volume.

## Tipos de contribuição

1. **Novas ferramentas para a base de conhecimento** (`.github/skills/cybershield-kb/references/`)
2. **Correções de links, versões, informações desatualizadas**
3. **Novos skills** ou melhorias aos existentes (`.github/skills/*/SKILL.md`)
4. **Ajustes em `AGENTS.md`, `README.md` e regras de IDE**
5. **Tradução, clareza, exemplos**
6. **Relatos de problemas** — abra uma [issue](https://github.com/TWalkingSE/cybershield/issues)

## Princípios do projeto

Antes de abrir um PR, releia `AGENTS.md`. Toda contribuição precisa respeitar:

- **TCP/IP como espinha dorsal** — recomendações indicam a camada `[Camada X — Nome]`.
- **Defense in depth** — nenhuma solução isolada é apresentada como suficiente.
- **Trade-offs explícitos** — custo em usabilidade, performance e complexidade.
- **Proporcionalidade ao threat model** — adeque a indicação ao perfil de usuário.
- **Admita incerteza** — nunca fabrique auditorias, versões, estatísticas ou protocolos.
- **Responda em português brasileiro.**

## Como adicionar uma ferramenta à base de conhecimento

1. Identifique a categoria em `.github/skills/cybershield-kb/references/`
   (ex.: `navegadores-busca.md`, `rede-anonimato.md`).
2. Para cada ferramenta, inclua no mínimo:
   - **Nome** e **link oficial** (https, domínio legítimo — sem typosquatting).
   - **Open-source?** (sim/não) e licença quando aplicável.
   - **Plataformas suportadas** (Windows/macOS/Linux/Android/iOS/Web).
   - **Camada TCP/IP** em que atua.
   - **Diferencial** (por que entrar na lista).
   - **Alertas de incidentes** conhecidos (ex.: Avast/venda de dados,
     LastPass/vazamento) — **omitir isso é motivo para rejeitar o PR**.
   - **Auditoria independente** quando houver — link e data.
3. Prefira projetos ativos, auditados e com reputação pública.
4. Rejeitamos ferramentas com histórico grave não divulgado, forks sem
   manutenção ou apps proprietários sem auditoria externa em categorias
   sensíveis (VPN, mensageria, criptografia).

## Como propor um skill novo

1. Copie a estrutura de um skill existente em `.github/skills/`.
2. `SKILL.md` deve conter frontmatter com `name` e `description` curtos e
   conteúdo progressivo (idealmente ≤95 linhas no arquivo principal).
3. Referências extensas vão em subpasta `references/`.
4. Se criar skill, lembre de adicionar **wrappers** em:
   - `.windsurf/skills/<nome>/SKILL.md` — apontando para o arquivo canônico
   - `.claude/skills/<nome>/SKILL.md` — idem
5. Atualize a tabela de skills no `README.md` e a lista em `AGENTS.md`.

## Padrões de estilo

- **Idioma:** português brasileiro em todo conteúdo voltado ao usuário.
  Metadados (frontmatter `name`) podem ficar em inglês se facilitar slash commands.
- **Markdown:** títulos `#`, listas com `-`, tabelas padrão GFM.
- **Links:** sempre absolutos, com `https://` e domínio oficial.
- **Sem emojis** no conteúdo técnico, exceto onde já existem (ex.: tabela do README).
- **Citação de fontes:** ao afirmar que uma ferramenta é auditada ou teve
  incidente, **inclua o link** para o relato/auditoria original.

## Fluxo de Pull Request

1. Faça um fork e crie uma branch com nome descritivo
   (ex.: `kb/adicionar-mullvad-browser`, `skill/novo-skill-autenticacao`).
2. Faça commits pequenos e com mensagens claras em português
   (ex.: `kb(rede-anonimato): adicionar Mullvad Browser com auditoria Cure53`).
3. Verifique que:
   - Links abrem e apontam para o domínio oficial.
   - Não há typosquatting nem URLs encurtadas.
   - Não há dados pessoais, tokens ou segredos no conteúdo.
   - Alertas de incidentes estão declarados quando aplicáveis.
4. Abra o PR contra `main` e preencha o template.
5. Seja paciente com a revisão — priorizamos precisão sobre velocidade.

## Relatar problemas de segurança

**Não abra issue pública** para problemas sensíveis. Siga `SECURITY.md`.

## Código de conduta

Ao participar, você concorda em seguir o `CODE_OF_CONDUCT.md`.

## Dúvidas

Abra uma [issue](https://github.com/TWalkingSE/cybershield/issues) com o
rótulo `question` ou use [Discussions](https://github.com/TWalkingSE/cybershield/discussions)
se habilitadas.

---

*Privacidade não é ter algo a esconder — é um direito fundamental.*
