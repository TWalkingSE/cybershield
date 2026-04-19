---
name: cybershield-kb
description: >
  Base de conhecimento CyberShield com 60 categorias e centenas de ferramentas
  de segurança digital e privacidade catalogadas com links, status open-source,
  alertas de incidentes e comparações. CONSULTE SEMPRE antes de recomendar 
  qualquer ferramenta. Use quando o usuário perguntar sobre ferramentas de 
  privacidade, segurança digital, VPN, navegador seguro, gerenciador de senhas,
  criptografia, mensageria segura, DNS, antivírus, backup, Tor, proxy, aliases,
  2FA, firewalls, LLMs locais, ou qualquer ferramenta de proteção digital.
  Também use para comparações entre ferramentas ou verificação de alertas
  e incidentes de segurança de serviços específicos.
---

# CyberShield — Base de Conhecimento de Ferramentas

**Versão:** 4.0 | **60 categorias** | **Centenas de ferramentas catalogadas**

## Regra Principal

**SEMPRE consulte o arquivo de referência relevante ANTES de recomendar uma ferramenta.** Cada arquivo contém tabelas com: nome, open-source (✅/❌), plataformas, diferencial e link oficial. Alertas de incidentes (ex: LastPass, Avast) estão indicados com ⚠️.

## Índice de Referências

| Tema do usuário | Arquivo em `references/` | Categorias cobertas |
|---|---|---|
| Senhas, 2FA, YubiKey, autenticação, SSO, compartilhamento de credenciais | `autenticacao-senhas.md` | §1, §24, §46, §59 |
| Antivírus, firewall, sandbox, auditoria de apps, honeypots, anti-stalkerware | `protecao-endpoint.md` | §2, §33, §38, §55, §57 |
| Backup, cloud segura, criptografia de arquivos, exclusão segura, sincronização P2P | `dados-criptografia.md` | §3, §4, §5, §35 |
| VPN, proxy, Tor, DNS seguro, rede doméstica, anti-censura, VPN auto-hospedado | `rede-anonimato.md` | §6, §7, §8, §16, §21, §53, §56 |
| Navegadores, buscadores, leak tests, bloqueadores de anúncios, cookies | `navegadores-busca.md` | §9, §10, §30, §48, §49 |
| E-mail (aliases, provedores, clientes), mensageria, videoconferência, transferência de arquivos, pastebins, push/telemetria | `comunicacao.md` | §12, §13, §17, §23, §25, §27, §28, §29 |
| Sistemas operacionais seguros, VMs, privacidade Android, privacidade iOS | `sistemas-plataformas.md` | §11, §20, §31, §32 |
| Metadados, fotos, notas, calendários, office, PDF, tradutores, mídia, redes sociais alternativas, mapas, saúde, RSS, acesso remoto | `produtividade-midia.md` | §14, §22, §26, §36, §39-45, §50-52, §58 |
| Anti-phishing, criptoativos, OSINT, data brokers, IA/LLMs, forense, pós-quântica, educação em segurança | `investigacao-educacao.md` | §15, §18, §19, §34, §37, §47, §54, §60 |

## Alertas Conhecidos (verificar antes de recomendar)

- **LastPass** (§1): ⚠️ Vazamento grave em 2022, cofres criptografados roubados
- **Avast/AVG** (§2): ⚠️ Venda de dados de navegação via Jumpshot (2020)
- **ExpressVPN** (§6): ⚠️ Adquirida pela Kape Technologies
- **NordVPN** (§6): ⚠️ Incidente de servidor em 2019
- **Hola VPN** (§7): ⚠️ Usava banda dos usuários como exit nodes
- **Telegram** (§13): ⚠️ Não usa E2E por padrão, protocolo proprietário

## Como Usar

1. Identifique a categoria da pergunta
2. Consulte a tabela acima para encontrar o arquivo de referência
3. Leia o arquivo correspondente em `references/`
4. Use as informações (nome, link, open-source, alertas) na resposta
5. Sempre indique a camada TCP/IP onde a ferramenta atua
