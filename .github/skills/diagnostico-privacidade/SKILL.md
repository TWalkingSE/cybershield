---
name: diagnostico-privacidade
description: >
  Diagnóstico de privacidade e avaliação de exposição digital do usuário. 
  Use quando o usuário quiser avaliar seu nível de proteção atual, perguntar 
  "estou seguro?", "o que preciso mudar?", "avalie minha segurança", listar 
  suas ferramentas atuais para avaliação, ou pedir uma auditoria de privacidade.
---

# Diagnóstico de Privacidade

## Fluxo

1. Pergunte: "Quais ferramentas e serviços você usa no dia a dia? (navegador, e-mail, mensageiro, VPN, SO)"
2. **Consulte `/cybershield-kb`** para verificar o perfil de cada ferramenta mencionada antes de avaliar
3. Avalie cada item contra as melhores práticas por camada TCP/IP
4. Entregue relatório estruturado

## Alertas Automáticos (acionar sempre que a ferramenta aparecer)

Antes de pontuar, verifique se o usuário usa qualquer ferramenta desta lista:

| Ferramenta | Alerta |
|---|---|
| **LastPass** | ⚠️ Vazamento grave 2022 — cofres roubados. Sugerir migração urgente para Bitwarden/KeePassXC |
| **Avast / AVG** | ⚠️ Venda de dados de navegação (FTC, 2024). Sugerir ClamAV / Windows Defender |
| **ExpressVPN** | ⚠️ Adquirida pela Kape Technologies (histórico de adware). Sugerir Mullvad/ProtonVPN |
| **Hola VPN** | 🔴 Usava banda dos usuários como exit nodes. Substituição imediata necessária |
| **Telegram** | ⚠️ Sem E2EE por padrão. Informar sobre Secret Chats e sugerir Signal/SimpleX |
| **WhatsApp** | ⚠️ Metadados extensos coletados pela Meta. Mencionar limitações |
| **Chrome (sem hardening)** | ⚠️ Telemetria Google. Sugerir Firefox + uBlock Origin ou Brave |
| **Gmail** | ⚠️ Análise de conteúdo pelo Google. Sugerir Proton Mail ou aliases |
| **Google Drive** | ⚠️ Acesso pelo Google. Sugerir Proton Drive ou Cryptomator |
| **Authy** | ⚠️ Requer número de telefone, código proprietário. Sugerir Aegis / Ente Auth |
| **Google Authenticator** | ⚠️ Backup na nuvem não é E2EE. Sugerir Aegis / Ente Auth |

## Formato de Entrega

```
📊 DIAGNÓSTICO DE PRIVACIDADE

[Camada 4 — Aplicação] Nota: X/10
✅ Pontos fortes: [o que está bom]
❌ Pontos críticos: [o que precisa mudar urgente]
🟡 Melhorias sugeridas: [otimizações]

[Camada 3 — Transporte] Nota: X/10
[idem]

[Camada 2 — Internet] Nota: X/10
[idem]

[Camada 1 — Acesso à Rede] Nota: X/10
[idem]

[Transversal] Nota: X/10
[idem]

⚡ TOP 3-5 AÇÕES PRIORITÁRIAS:
1. [ação de maior impacto]
...

📈 Nota Geral: X/10 — [Nível: Iniciante / Em desenvolvimento / Bom / Avançado / Expert]
```

## Critérios de Nota por Camada

- **9-10**: Ferramentas auditadas, open-source, configuração avançada
- **7-8**: Boas ferramentas com configuração padrão
- **5-6**: Ferramentas aceitáveis com lacunas
- **3-4**: Ferramentas problemáticas ou configuração fraca
- **1-2**: Sem proteção ou ferramentas com histórico de abuso de dados

## Regras

- Sempre consulte a KB (`/cybershield-kb`) antes de avaliar uma ferramenta desconhecida
- Para ferramentas com alertas: informe o alerta ANTES de dar a nota da camada
- Priorize ações de maior impacto com menor esforço de implementação
- Adapte o tom ao nível do usuário (leigo vs avançado)
- Nunca garanta que o usuário "está seguro" — segurança é um processo contínuo
