---
name: analise-ferramenta
description: >
  Análise de segurança e confiabilidade de ferramentas e serviços digitais.
  Use quando o usuário perguntar se uma ferramenta é segura, confiável, ou 
  privada. Exemplos: "o Brave é seguro?", "posso confiar no LastPass?", 
  "NordVPN é boa?", "qual o melhor gerenciador de senhas?", "essa extensão 
  é segura?", "devo usar o Telegram ou Signal?". Também use para comparações 
  diretas entre ferramentas de segurança/privacidade.
---

# Análise de Ferramenta

## Critérios de Avaliação

Para TODA ferramenta analisada, avalie estes critérios:

| Critério | O que verificar |
|---|---|
| Código aberto? | Repositório público, licença, contribuições ativas |
| Auditoria independente? | Auditorias de segurança por terceiros, data da última |
| Política de privacidade? | Coleta de dados, telemetria, compartilhamento com terceiros |
| Jurisdição? | País sede, leis de vigilância aplicáveis (Five/Nine/Fourteen Eyes) |
| Histórico de incidentes? | Vazamentos, controvérsias, mudanças de propriedade |
| Modelo de negócio? | Como ganha dinheiro (assinatura, anúncios, venda de dados) |
| Alternativas superiores? | Ferramentas concorrentes com melhor perfil |

## Alertas Conhecidos (consultar antes de recomendar)

- **Avast/AVG**: venda de dados de navegação via Jumpshot (2020)
- **LastPass**: vazamentos graves em 2022-2023, cofres criptografados comprometidos
- **ExpressVPN**: adquirida pela Kape Technologies (histórico de adware)
- **NordVPN**: incidente de servidor em 2019, propriedade via Tesonet (controvérsias)
- **Hola VPN**: usava banda dos usuários como exit nodes
- **Telegram**: não usa E2E por padrão, protocolo MTProto proprietário
- **WhatsApp**: metadados compartilhados com Meta

## Formato de Saída

```
📋 ANÁLISE: [Nome da Ferramenta]
[Camada TCP/IP onde atua]

| Critério | Avaliação |
|---|---|
| Código aberto | ✅/⚠️/❌ + detalhe |
| Auditoria | ✅/⚠️/❌ + detalhe |
| Privacidade | ✅/⚠️/❌ + detalhe |
| Jurisdição | [país] + implicações |
| Incidentes | ✅/⚠️/❌ + detalhe |

🏷️ Veredicto: [Recomendado / Com ressalvas / Não recomendado]
Justificativa: [resumo]

🔄 Alternativas:
- [Ferramenta 1] — [diferencial]
- [Ferramenta 2] — [diferencial]
```

## Regras

- NUNCA recomende ferramenta com histórico problemático sem mencionar o alerta
- Sempre ofereça pelo menos 2 alternativas
- Diferencie entre "seguro para uso casual" e "seguro para alto risco"
- Indique a camada TCP/IP onde a ferramenta atua
