---
name: threat-modeling
description: >
  Modelo de ameaça personalizado para segurança digital. Use quando o usuário 
  quiser avaliar seu perfil de risco, descobrir suas vulnerabilidades, criar um 
  plano de segurança personalizado, ou perguntar "como me proteger", "qual meu 
  nível de risco", "preciso de VPN?", "estou seguro?". Também use quando o 
  contexto envolver jornalistas, ativistas, profissionais que lidam com dados 
  sensíveis, ou qualquer avaliação de segurança personalizada.
---

# Threat Modeling — Modelo de Ameaça Personalizado

## Quando Usar

- Usuário quer avaliar seu nível de risco
- Usuário pergunta "como me proteger" sem tema específico
- Usuário menciona perfil profissional sensível (jornalista, ativista, advogado, TI)
- Usuário pede recomendações personalizadas de segurança

## Fluxo Interativo (3 Rodadas)

### Rodada 1 — Perfil Básico
Pergunte:
1. Qual sua atividade principal? (estudante, profissional de TI, jornalista, ativista, empresário, uso pessoal)
2. Você lida com informações sensíveis no dia a dia? (dados de clientes, fontes confidenciais, propriedade intelectual, dados pessoais)

### Rodada 2 — Superfície de Exposição
Pergunte:
1. Quais dispositivos usa regularmente? (PC pessoal, celular, PC de trabalho, tablet)
2. Usa redes públicas (cafés, aeroportos) com frequência?

### Rodada 3 — Adversários e Preocupações
Pergunte:
1. Quem são seus potenciais adversários? (rastreadores de anúncios, hackers oportunistas, espionagem corporativa, governo, stalker/assediador)
2. Qual sua maior preocupação hoje? (vazamento de dados, rastreamento online, interceptação de comunicações, segurança física do dispositivo)

## Formato de Entrega

Após as 3 rodadas, entregue:

```
🎯 MODELO DE AMEAÇA PERSONALIZADO

Perfil: [Casual / Profissional / Alto Risco / Crítico]
Adversários identificados: [lista]
Ativos a proteger: [dados, comunicações, identidade, dispositivos]
Superfície de ataque: [pontos de exposição]

📊 PRIORIDADES POR CAMADA TCP/IP:

[Camada 4 — Aplicação]
🔴 Crítico: [ações imediatas]
🟡 Recomendado: [melhorias importantes]
🟢 Ideal: [proteção avançada]

[Camada 3 — Transporte]
🔴/🟡/🟢 [idem]

[Camada 2 — Internet]
🔴/🟡/🟢 [idem]

[Camada 1 — Acesso à Rede]
🔴/🟡/🟢 [idem]

[Transversal]
🔴/🟡/🟢 [idem]

⚡ TOP 5 AÇÕES IMEDIATAS (por ordem de impacto):
1-5. [ações concretas]

⏱️ Tempo estimado de implementação: [estimativa realista]
```

## Classificação de Perfil

- **Casual**: uso pessoal, sem dados sensíveis. Adversários: trackers, hackers oportunistas.
- **Profissional**: lida com dados de trabalho. Adversários: + espionagem corporativa, phishing direcionado.
- **Alto Risco**: jornalista, ativista, advogado com casos sensíveis. Adversários: + governo, vigilância.
- **Crítico**: dissidente, whistleblower, situação de risco físico. Adversários: + ataques direcionados, 0-days.

## Regras

- Sempre adapte recomendações ao perfil — não sugira Qubes OS para um usuário casual
- Priorize ações de alto impacto e baixo esforço primeiro
- Inclua estimativa realista de tempo de implementação
- Nunca garanta segurança absoluta
