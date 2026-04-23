---
name: privacidade-financeira
description: >
  Privacidade e segurança financeira digital. Use quando o usuário perguntar sobre
  proteção de dados bancários, cartões virtuais, golpes financeiros (Pix, boleto,
  WhatsApp), criptomoedas com privacidade (Monero), proteção de identidade
  financeira, vazamento de CPF, score de crédito, ou qualquer tema de segurança
  com dimensão financeira. Exemplos: "como proteger meu banco online", "cartão
  virtual", "golpe no Pix", "Monero", "meu CPF vazou", "score Serasa", "cartão
  clonado", "phishing bancário", "2FA no banco".
---

# Privacidade Financeira

## Contexto

Dados financeiros são dos mais sensíveis e lucrativos para atacantes. Atua primariamente em **[Camada 4 — Aplicação]**, com dimensões físicas (cartões) e legais (LGPD). No Brasil, o CPF funciona como identificador universal e seu vazamento facilita fraudes de identidade.

---

## 1. Proteção do Banco Online

### Configurações Obrigatórias

| Ação | Por quê |
|---|---|
| **Ativar notificação em tempo real** (push/SMS) para todas as transações | Detectar transações não autorizadas imediatamente |
| **Definir limites de transação** (Pix, TED, cartão) | Limitar o dano em caso de comprometimento |
| **Ativar 2FA no app do banco** | Impede acesso mesmo com senha correta |
| **Cadastrar dispositivo confiável** | Apps bancários geralmente exigem re-autenticação em dispositivos novos |
| **Nunca usar banco em Wi-Fi público sem VPN** | Risco de interceptação (MITM) |
| **Verificar certificado HTTPS** (cadeado verde + domínio correto) | Proteção contra phishing de banco |
| **Senha exclusiva para o banco** (nunca reutilizar) | Isolamento de comprometimento |

### O que Bancos NUNCA Fazem

- Nunca pedem senha completa por telefone, WhatsApp ou e-mail
- Nunca pedem token/código de autenticação por telefone
- Nunca pedem para instalar apps de "suporte remoto"
- Nunca pedem para transferir dinheiro para "conta segura"

> Se alguém ligar se passando por banco e pedir qualquer dessas coisas: **desligue e ligue para o número oficial do banco no verso do cartão**.

---

## 2. Cartões Virtuais (Privacidade em Compras Online)

Cartões virtuais permitem compras online sem expor o número do cartão físico real.

| Serviço | País | Gratuito | Diferencial | Link |
|---|---|---|---|---|
| **Privacy.com** | EUA | ✅ (3 cartões/mês) | Cartões virtuais vinculados a qualquer banco, limites e merchants específicos | https://privacy.com/ |
| **Cartão Virtual do próprio banco** | BR | ✅ (maioria) | Número temporário descartável. Solicitar no app. Disponível em: Nubank, Itaú, Bradesco, C6, Inter, PicPay | — |
| **Nubank (cartão virtual)** | BR | ✅ | Cartão virtual para compras online + número que muda automaticamente | — |
| **Revolut Virtual** | EU/Global | ✅ | Cartões virtuais descartáveis para cada transação | https://revolut.com/ |
| **Wise Virtual Card** | Global | ✅ | Cartão virtual em múltiplas moedas | https://wise.com/ |
| **PayPal** | Global | ✅ | Intermediário de pagamento — comerciante não vê dados do cartão real | https://paypal.com/ |
| **Apple Pay / Google Pay** | Global | ✅ | Tokenização — o comerciante recebe apenas um token, não o número real do cartão | — |

> **Regra prática:** Para compras online em sites desconhecidos ou que usará apenas uma vez — use sempre cartão virtual descartável.

---

## 3. Proteção contra Golpes Financeiros no Brasil

### Golpes do Pix

| Golpe | Como identificar | O que fazer |
|---|---|---|
| **Pix errado** | "Transferi por engano, pode devolver?" | Verificar extrato — se recebeu, o dinheiro é seus. Golpe usa contas laranja. **Nunca devolver sem confirmar diretamente com seu banco.** |
| **Falso comprador** | Comprador envia comprovante falso antes de receber o produto | Verificar o recebimento no app do banco **antes** de entregar qualquer coisa |
| **QR Code adulterado** | QR code de cobrança trocado por criminoso em estabelecimento físico | Sempre conferir o nome e CPF/CNPJ do destinatário antes de confirmar |
| **Pix agendado para "testar"** | Golpista pede para fazer Pix para verificar dados bancários | Nenhum procedimento legítimo exige transferência de teste |
| **Falso Pix de prêmio** | "Você ganhou, primeiro pague uma taxa" | Nenhum prêmio legítimo exige pagamento antecipado |

### Proteção Recomendada do Banco Central

- **Limites de transação noturna**: BCB exige que bancos ofereçam configuração de limite reduzido entre 20h e 6h — ativar sempre
- **Mecanismo Especial de Devolução (MED)**: em caso de fraude, contate o banco em até 80 dias — ele pode recuperar o valor via MED
- **Chave Pix**: prefira usar CPF/CNPJ (reversível para investigação) a telefone para chaves aleatórias

---

## 4. Seu CPF Vazou — O Que Fazer

O CPF é o identificador central de dados no Brasil. Vazamentos frequentes de grandes bases (como os de 2021 com 220M de CPFs) expõem praticamente todos os brasileiros.

### Verificar se seus Dados Estão Expostos

| Ferramenta | O que mostra | Link |
|---|---|---|
| **Have I Been Pwned** | E-mails em vazamentos globais | https://haveibeenpwned.com/ |
| **Registrato (BCB)** | Chaves Pix, contas e empréstimos em seu CPF | https://registrato.bcb.gov.br/ |
| **Serasa/Boa Vista (verificação gratuita)** | Consultas ao seu CPF (tentativas de crédito em seu nome) | https://www.serasa.com.br/ |
| **gov.br** | Consultar benefícios, contratos e procurações em seu CPF | https://www.gov.br/ |
| **Cadastro Positivo** | Ver instituições consultando seu CPF | — |

### O Que Fazer se seus Dados Vazaram

```
🟡 CPF/Dados vazados — Protocolo

1. Monitorar alertas de crédito (Serasa, Boa Vista) — suspeitos de crédito em seu nome
2. Verificar Registrato (BCB): contas bancárias abertas em seu CPF sem você saber
3. Ativar bloqueio de crédito (cadastro gratuito nos birôs — Serasa, SPC)
4. Monitorar extratos bancários diariamente nas primeiras semanas
5. Se encontrar movimentação suspeita: Boletim de Ocorrência imediatamente
6. LGPD Art. 18 — solicitar exclusão de dados às empresas que os possuem
7. Registrar reclamação na ANPD se a empresa não responder
```

---

## 5. Criptomoedas com Privacidade

### Por Que Bitcoin NÃO é Anônimo

Bitcoin é **pseudônimo**, não anônimo. Todas as transações são públicas e rastreáveis on-chain. Análise de blockchain pode associar endereços a identidades (especialmente via exchanges KYC).

### Ferramentas de Privacidade em Cripto

| Ferramenta | Tipo | Diferencial | Nível |
|---|---|---|---|
| **Monero (XMR)** | Criptomoeda | Privacidade por padrão: ring signatures, stealth addresses, RingCT — oculta remetente, destinatário e valor | Avançado |
| **Sparrow Wallet + CoinJoin** | Carteira Bitcoin | CoinJoin mistura transações Bitcoin, aumentando privacidade | Intermediário |
| **Wasabi Wallet (WabiSabi)** | Carteira Bitcoin | CoinJoin nativo, fácil de usar | Intermediário |
| **Feather Wallet** | Carteira Monero | Leve, suporte a Tor, interface amigável | Intermediário |
| **BTCPay Server** | Processador de pagamentos | Auto-hospedado, sem custódia, sem KYC | Avançado |
| **Lightning Network** | Layer 2 Bitcoin | Transações off-chain, mais privadas que on-chain | Intermediário |

> ⚠️ **Atenção legal:** O uso de moedas de privacidade e CoinJoin é legal no Brasil, mas pode aumentar o escrutínio em exchanges. Declare criptoativos na Receita Federal conforme exigido.

### Exchanges com Menor Exposição de Dados

- Prefira exchanges com mínimo de dados KYC para pequenas quantias
- Para valores maiores, o KYC é geralmente obrigatório por lei
- Considere P2P (HodlHodl, Bisq) para transações sem custódia

---

## 6. Seguro e Recuperação

### Senhas e 2FA em Contas Financeiras

- **NUNCA use SMS como 2FA para banco** se houver alternativa — suscetível a SIM swap
- Prefira app autenticador (Aegis, Ente Auth) ou chave física (YubiKey)
- SIM Swap: criminoso convence operadora a transferir seu número para um chip deles → recebem todos os SMS, inclusive códigos bancários

### Proteção contra SIM Swap

| Ação | Como fazer |
|---|---|
| **PIN/senha na conta da operadora** | Cadastrar PIN na operadora (Vivo, Claro, TIM, Oi) que será exigido em qualquer alteração |
| **Não usar número de telefone como 2FA** | Migrar para app autenticador |
| **Alertas de portabilidade** | Ativar notificações da operadora |
| **Verificar conta da operadora regularmente** | Checar planos e dispositivos associados |

## Regras

- Banco online em dispositivo dedicado ou navegador isolado (perfil separado)
- Nunca discuta saldos, senhas ou dados bancários em redes sociais ou apps não criptografados
- Proporcionalidade: o nível de proteção deve ser compatível com o valor em risco
- Em caso de fraude financeira: registrar B.O., contatar banco imediatamente e guardar todos os comprovantes
