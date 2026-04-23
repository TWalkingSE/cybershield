---
name: protecao-familiar
description: >
  Segurança digital para famílias, crianças e adolescentes. Use quando o usuário
  quiser proteger filhos online, configurar controles parentais, filtrar conteúdo
  inadequado, monitorar uso de internet de crianças, proteger idosos de golpes,
  configurar DNS familiar, ou quando mencionar: "meu filho", "meus pais", "avós",
  "controle parental", "criança online", "golpe no WhatsApp", "segurança para
  família", "bloquear sites", "tempo de tela". Inclui proteção de idosos contra
  golpes financeiros e de engenharia social.
---

# Proteção Familiar — Segurança Digital para Toda a Família

## Contexto

Famílias têm perfis de ameaça distintos por faixa etária. Crianças enfrentam riscos de conteúdo inapropriado, predadores e cyberbullying; adolescentes, riscos de privacidade e exposição em redes sociais; idosos, golpes financeiros e phishing. Atua em **[Camada 4 — Aplicação]** e **[Transversal]**.

---

## 1. DNS Familiar (bloqueia conteúdo inadequado em toda a rede)

A abordagem mais eficiente: configure o DNS do roteador para filtrar conteúdo automaticamente para todos os dispositivos da casa.

| Provedor | Diferencial | DNS Primário | DNS Secundário |
|---|---|---|---|
| **CleanBrowsing (Family)** | Bloqueia adultos, proxy, VPN, domínios maliciosos | `185.228.168.168` | `185.228.169.168` |
| **Cloudflare for Families (1.1.1.3)** | Bloqueia adultos e malware, Cloudflare | `1.1.1.3` | `1.0.0.3` |
| **Quad9** | Bloqueia malware/phishing, sem filtro de conteúdo (para adultos com filhos) | `9.9.9.9` | `149.112.112.112` |
| **OpenDNS FamilyShield** | Clássico, bloqueia adultos | `208.67.222.123` | `208.67.220.123` |
| **NextDNS** | Customizável por perfil, logs, listas por categoria, plano família | https://nextdns.io/ | — |
| **AdGuard DNS (Family)** | Bloqueio de adultos + anúncios/rastreadores | `94.140.14.15` | `94.140.15.16` |

> **Como configurar:** No roteador, acesse as configurações DNS (geralmente em "WAN" ou "Internet") e substitua os servidores DNS do provedor pelos valores acima. Todos os dispositivos da rede usarão automaticamente o filtro.

### DNS Local Avançado (Pi-hole + listas familiares)

Para controle granular, combine **Pi-hole** ou **AdGuard Home** com listas de bloqueio para crianças:
- `hagezi/dns-blocklists` — listas curadas por categoria
- `StevenBlack/hosts` — lista abrangente de anúncios/malware
- Categorias disponíveis: adultos, apostas, redes sociais, jogos (por horário)

---

## 2. Controles Parentais por Dispositivo

### Android (crianças)
- **Google Family Link**: controle parental nativo do Google — aprovação de apps, tempo de tela, localização
- **Screen Time / Digital Wellbeing**: limites de tempo por app
- **Configurar conta Google supervisionada** (para menores de 13 anos)
- **NetGuard ou RethinkDNS**: filtro DNS por app sem root

### iOS / iPhone (crianças)
- **Screen Time** (Configurações > Tempo de Uso): limites por app, horários de uso, restrições de conteúdo
- **Family Sharing (iCloud)**: compras requerem aprovação, localização familiar
- **Restrições de conteúdo**: bloquear apps por classificação etária, conteúdo explícito
- **Ask to Buy**: compras no App Store requerem autorização do responsável

### Windows (crianças)
- **Microsoft Family Safety**: tempo de tela, filtro de conteúdo, localização, histórico de atividades
- **Conta Microsoft Kids** (separada da conta adulto)
- **DNS no roteador** (CleanBrowsing) como camada adicional — mais difícil de contornar

### Roteador (todos os dispositivos)
- Criar **SSID separado** para crianças com DNS filtrado
- **Agendamento de Wi-Fi**: desligar automaticamente em horários de sono/estudo
- **Controle por MAC address**: bloquear dispositivos específicos em certos horários

---

## 3. Proteção de Crianças Online

### Riscos Principais

| Risco | Idade mais afetada | Abordagem |
|---|---|---|
| **Conteúdo inadequado** | 6–12 anos | DNS familiar + controles parentais |
| **Predadores online** | 10–16 anos | Conversas abertas + supervisão de chats |
| **Cyberbullying** | 10–17 anos | Ferramentas de denúncia + comunicação aberta |
| **Golpes e phishing** | Todas | Educação + filtros DNS |
| **Oversharing (exposição pessoal)** | 13–18 anos | Educação sobre privacidade, revisão de perfis |
| **Sexting não consensual** | 14–18 anos | Educação sobre consequências, confiança familiar |

### Plataformas Seguras para Crianças

| Plataforma | Faixa Etária | Diferencial |
|---|---|---|
| **YouTube Kids** | 3–12 anos | Conteúdo curado, sem comentários livres |
| **Messenger Kids (Meta)** | 6–12 anos | Chat controlado pelos pais, sem estranhos |
| **Roblox (com configurações)** | 7–16 anos | Restrições de chat, verificação parental |
| **Khan Academy Kids** | 2–8 anos | Educacional, sem publicidade, sem dados |
| **PBS Kids** | 3–8 anos | Conteúdo educativo americano, sem anúncios |

### O que NUNCA compartilhar online (ensine às crianças)
- Nome completo, escola, endereço, horários de rotina
- Fotos do rosto identificável de menores (em locais reconhecíveis)
- Informações dos pais ou financeiras

---

## 4. Proteção de Idosos (Golpes e Phishing)

### Golpes mais comuns no Brasil

| Golpe | Como funciona | Proteção |
|---|---|---|
| **Golpe do falso neto** | Ligação fingindo ser neto/filho em emergência pedindo Pix | Código família secreto para emergências reais |
| **Golpe do Pix errado** | "Caiu na sua conta por engano, me devolva" (dinheiro era lavado) | Nunca devolver sem confirmar com o banco diretamente |
| **Golpe do falso banco** | Ligação do "banco" pedindo dados/tokens | Banco NUNCA pede senha por telefone — desligar e ligar pro número oficial |
| **WhatsApp clonado** | Invasão da conta para pedir dinheiro a contatos | Ativar 2FA no WhatsApp, código de verificação secreto |
| **Phishing em e-mail/SMS** | Links falsos de Correios, Receita Federal, banco | Não clicar em links de e-mail/SMS — acessar o site diretamente |
| **Falso suporte técnico** | Pop-up de "vírus" com número para ligar | Fechar o navegador, nunca ligar |

### Configurações de Proteção para Idosos

**WhatsApp (obrigatório para idosos):**
1. Ativar verificação em dois passos (PIN de 6 dígitos): Menu > Configurações > Conta > Verificação em duas etapas
2. Ninguém pode adicionar a um grupo sem permissão: Privacidade > Grupos > "Meus contatos"
3. Desativar preview de links automaticamente

**Smartphone:**
- Instalar apenas apps da loja oficial (Google Play / App Store)
- Não instalar apps de fontes desconhecidas
- Ativar bloqueio de tela com PIN
- Configurar número de emergência de contato familiar

**E-mail:**
- Ativar filtro de spam forte
- Nunca clicar em links de e-mails não solicitados
- Verificar sempre o remetente completo (não apenas o nome exibido)

### Código de Segurança Familiar

Crie uma **palavra de código secreta** que só a família conhece — qualquer ligação de emergência que não souber o código é golpe. Ensine aos idosos a usar antes de qualquer transferência.

---

## 5. Recursos e Educação

| Recurso | Tipo | Link |
|---|---|---|
| **SaferNet Brasil** | Denúncia e educação (BR) | https://www.safernet.org.br/ |
| **EFF: Teaching Privacy** | Educação digital para jovens | https://teachingprivacy.org/ |
| **Cyber.org** | Currículo de cibersegurança para escolas | https://cyber.org/ |
| **Common Sense Media** | Avaliações de apps/jogos/filmes para pais | https://www.commonsensemedia.org/ |
| **Internet Matters** | Guias para pais sobre segurança online | https://www.internetmatters.org/ |
| **Procon (BR)** | Denúncias de golpes e orientação | https://www.procon.sp.gov.br/ |
| **ANPD** | Direitos de dados (inclui menores) | https://www.gov.br/anpd/ |

## Regras

- Tecnologia não substitui conversa: diálogo aberto é a melhor proteção para adolescentes
- Controles parentais devem ser transparentes com adolescentes — segredo cria desconfiança
- Para idosos: repita instruções simples com calma e sem julgamento
- Adapte o nível de controle à faixa etária e maturidade de cada criança
- Nunca instale apps de monitoramento sem o conhecimento da criança (adolescentes) — exceto em casos de risco grave
