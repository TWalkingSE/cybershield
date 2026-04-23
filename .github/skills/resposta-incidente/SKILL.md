---
name: resposta-incidente
description: >
  Protocolo de resposta a incidentes de segurança pessoal. Use quando o usuário
  suspeitar que foi hackeado, tiver conta invadida, dispositivo comprometido,
  e-mail acessado por terceiros, senhas vazadas, stalkerware instalado, ou qualquer
  situação de comprometimento ativo. Também use para: "acho que me hackaram",
  "minha conta foi invadida", "recebi alerta de login suspeito", "meu ex pode ter
  instalado algo no celular", "recebi e-mail com minha senha", "preciso saber o
  que fazer agora". Situação de emergência — priorize velocidade e ordem das ações.
---

# Resposta a Incidentes — Protocolo Pessoal de Emergência

## ⚡ MODO DE EMERGÊNCIA

Quando o usuário estiver em situação ativa de comprometimento, entregue o protocolo correspondente **imediatamente**, sem longas explicações. Pergunte primeiro: **"Qual é a situação? (conta invadida / dispositivo comprometido / senha vazada / suspeita de stalkerware)"** e direcione para o protocolo correto.

---

## PROTOCOLO 1 — Conta Invadida (E-mail, Redes Sociais, Banco)

```
🔴 AÇÕES IMEDIATAS — Conta Invadida

PASSO 1 — Recuperar o acesso (se ainda não tiver):
• Use "esqueci minha senha" ou códigos de recuperação
• Se não conseguir: contate o suporte com verificação de identidade

PASSO 2 — Expulsar o invasor:
• Revogar TODAS as sessões ativas ("Sair em todos os dispositivos")
• Trocar senha imediatamente (nova, aleatória, 16+ caracteres)
• Trocar e-mail de recuperação (se foi alterado pelo invasor)

PASSO 3 — Fortalecer o acesso:
• Ativar 2FA se ainda não tinha (prefira TOTP — Aegis/Ente Auth)
• Verificar apps e integrações autorizadas — revogar desconhecidos
• Checar regras de encaminhamento de e-mail (invasores frequentemente adicionam)

PASSO 4 — Danos colaterais:
• Listar contas que usam esse e-mail como recuperação
• Trocar senhas dessas contas também (principalmente banco, e-mail secundário)
• Verificar Have I Been Pwned (haveibeenpwned.com)
• Ativar alertas de login nas contas críticas

PASSO 5 — Investigar e documentar:
• Verificar histórico de acessos: IPs, datas, dispositivos
• Prints do histórico para registro
• B.O. se houver dano financeiro
```

---

## PROTOCOLO 2 — Dispositivo Comprometido (PC ou Celular)

```
🔴 AÇÕES IMEDIATAS — Dispositivo Comprometido

AVALIAR PRIMEIRO: Acesso físico por terceiro OU comprometimento remoto?

[ Se comprometimento remoto / malware suspeito ]

PASSO 1 — Isolar o dispositivo:
• Desconectar da internet (Wi-Fi e dados móveis)
• Não fazer login em novas contas neste dispositivo

PASSO 2 — Avaliar a extensão:
• Qual software foi executado? (downloads, anexos, links clicados)
• O que estava aberto na época? (senhas, contas bancárias?)

PASSO 3 — Limpar ou isolar:
• Opção A (recomendada): Formatar e reinstalar o SO do zero
• Opção B (emergência): Rodar ClamAV / Malwarebytes offline
• Celular: wipe de fábrica ("reset de fábrica") se suspeitar de spyware

PASSO 4 — Após limpar, trocar credenciais:
• Trocar TODAS as senhas acessadas no dispositivo comprometido
• Revogar sessões de todos os serviços
• Gerar novos códigos de backup 2FA

PASSO 5 — Prevenir reinfecção:
• Restaurar apenas dados essenciais (não restaurar backup completo)
• Não reinstalar apps desnecessários
• Verificar fontes de download — o vetor de infecção foi identificado?
```

---

## PROTOCOLO 3 — Stalkerware (Ex-parceiro, Espião)

```
🔴 ATENÇÃO: Stalkerware é uma situação de risco pessoal — a segurança física pode estar em risco

PASSO 1 — Avaliar o risco antes de agir:
• Se o stalker tiver acesso físico a você, remover o app pode alertá-lo
• Planeje a ação para quando estiver em local seguro

PASSO 2 — Detectar:
• Android: Settings > Apps > listar TODOS os apps, incluindo serviços do sistema
• Usar MVT (Mobile Verification Toolkit) em dispositivo limpo separado
• Usar Warden (F-Droid) para detecção de stalkerware

PASSO 3 — Coletar evidências (se necessário para BO):
• Prints de apps suspeitos, permissões, histórico de instalação
• NÃO deletar antes de documentar

PASSO 4 — Remover com segurança:
• Opção mais segura: wipe completo do dispositivo e configuração do zero
• NÃO restaurar backup do período suspeito

PASSO 5 — Recursos de apoio:
• Coalition Against Stalkerware: https://stopstalkerware.org/
• Central de Atendimento à Mulher: 180 (Brasil, 24h)
• Ligue 190 em situações de perigo imediato
```

---

## PROTOCOLO 4 — Senha Vazada / Have I Been Pwned

```
🟡 Senha/E-mail em Vazamento

PASSO 1 — Verificar extensão:
• haveibeenpwned.com — quais serviços foram comprometidos?
• O vazamento inclui senhas em texto claro ou só e-mails?

PASSO 2 — Ação por prioridade:
🔴 Banco / e-mail principal / gerenciador de senhas → trocar AGORA
🟡 Redes sociais, trabalho → trocar nas próximas horas
🟢 Serviços menos críticos → trocar na próxima semana

PASSO 3 — Se a senha vazada era reutilizada:
• Identificar TODOS os serviços que usavam essa senha
• Trocar em todos eles com senhas únicas e aleatórias
• Este é o momento de adotar um gerenciador de senhas (Bitwarden/KeePassXC)

PASSO 4 — Ativar 2FA em todas as contas críticas
PASSO 5 — Configurar alerta automático: Firefox Monitor ou HaveIBeenPwned (alertas grátis)
```

---

## PROTOCOLO 5 — Ataque de Phishing (Cliquei em link suspeito)

```
🟡 Cliquei em link suspeito / baixei arquivo malicioso

PASSO 1 — Não inserir credenciais no site aberto
PASSO 2 — Fechar o browser e desconectar da internet
PASSO 3 — Verificar o arquivo:
• VirusTotal (virustotal.com) — fazer upload do arquivo
• Se não executou: deletar e monitorar

PASSO 4 — Se executou o arquivo:
• Seguir PROTOCOLO 2 — Dispositivo Comprometido

PASSO 5 — Se inseriu credenciais:
• Seguir PROTOCOLO 1 — Conta Invadida para a conta afetada

PASSO 6 — Reportar phishing:
• Google Safe Browsing: https://safebrowsing.google.com/safebrowsing/report_phish/
• PhishTank: https://phishtank.org/
```

---

## Lista de Verificação Pós-Incidente

Após controlar a situação imediata:

- [ ] Todas as senhas afetadas trocadas por senhas únicas e fortes
- [ ] 2FA ativo em todas as contas críticas (preferencialmente TOTP, não SMS)
- [ ] Sessões revogadas em todos os dispositivos
- [ ] Apps de terceiros autorizados revisados e limpos
- [ ] Regras de encaminhamento de e-mail verificadas
- [ ] Códigos de backup 2FA gerados e armazenados com segurança
- [ ] Have I Been Pwned verificado
- [ ] Alertas de login ativados nas contas críticas
- [ ] Gerenciador de senhas configurado (se ainda não tinha)
- [ ] B.O. registrado se houver dano financeiro ou risco de segurança

## Ferramentas de Suporte

| Ferramenta | Uso | Link |
|---|---|---|
| **Have I Been Pwned** | Verificar e-mails/senhas em vazamentos | https://haveibeenpwned.com/ |
| **MVT (Mobile Verification Toolkit)** | Detectar spyware (Pegasus) em celulares | https://mvt.re/ |
| **Warden** | Detectar stalkerware no Android | F-Droid |
| **VirusTotal** | Verificar arquivos e URLs suspeitos | https://virustotal.com/ |
| **ClamAV / Malwarebytes** | Varredura de malware | — |
| **Prey Project** | Localização/wipe remoto de dispositivos | https://preyproject.com/ |

## Regras

- Velocidade importa: cada minuto que o invasor tem acesso é um minuto a mais de dano
- Não use o dispositivo comprometido para trocar senhas — use um dispositivo limpo
- Documente tudo: prints, logs, datas — útil para B.O. e investigação posterior
- Após o incidente: revisar o modelo de ameaça e fechar as lacunas que permitiram o ataque
