---
name: checklist-viagem
description: >
  Checklist de segurança digital para viagens nacionais e internacionais. Use
  quando o usuário for viajar, cruzar fronteiras, usar Wi-Fi de hotel/aeroporto,
  ou precisar proteger dispositivos em trânsito. Exemplos: "vou viajar ao exterior",
  "como proteger meu notebook na viagem", "posso usar Wi-Fi do hotel", "fronteira",
  "alfândega", "viagem internacional", "Wi-Fi público", "roaming", "chip local",
  "dispositivo para viagem". Inclui países com vigilância elevada e dicas de OPSEC
  para jornalistas e ativistas em trânsito.
---

# Checklist de Viagem — Segurança Digital

## Contexto

Viagens expõem dispositivos a riscos únicos: fronteiras com poder de inspeção, redes Wi-Fi não confiáveis, perda/roubo físico, e jurisdições com diferentes leis de privacidade. Atua em **[Camada 1 — Acesso à Rede]**, **[Camada 3 — Transporte]** e **[Transversal]**.

---

## ✈️ ANTES DE VIAJAR — Checklist de Preparação

### Mínimo Recomendado (toda viagem)

- [ ] **Criptografia de disco ativa** em todos os dispositivos (BitLocker, FileVault, LUKS)
- [ ] **Backup completo** em local seguro offline (não leve o backup)
- [ ] **Senha forte no BIOS/UEFI** para impedir boot externo
- [ ] **VPN configurada e testada** — saber como ativar rapidamente
- [ ] **2FA em todas as contas críticas** sem dependência de SMS (SIM estrangeiro não recebe SMS do Brasil)
- [ ] **Códigos de backup 2FA** impressos ou armazenados offline
- [ ] **Localização remota ativa**: Find My, Find My Device, Prey
- [ ] **IMEI anotado** (discque `*#06#`) — necessário para boletim de ocorrência
- [ ] **Senhas críticas memorizadas** — não dependa exclusivamente do gerenciador se perder acesso

### Para Destinos de Alto Risco (países com vigilância intensa)

- [ ] **Dispositivo de viagem dedicado ("travel device")** — notebook/celular limpo, sem dados sensíveis
- [ ] **Contas de viagem separadas** — não use contas pessoais reais nesses dispositivos
- [ ] **Criptografia adicional de arquivos sensíveis** (VeraCrypt antes de embarcar)
- [ ] **Volume oculto VeraCrypt** para negação plausível sob coerção
- [ ] **Tails em pendrive** como alternativa a levar notebook completo
- [ ] **Apagar apps desnecessários** — menos superfície de ataque visível em inspeção
- [ ] **Sair de todas as contas** antes de cruzar a fronteira (redes sociais, e-mails não essenciais)
- [ ] **Desativar Touch ID / Face ID** — biometria pode ser coercitiva; PIN é protegido em muitas jurisdições

---

## 🛃 NA FRONTEIRA — Inspeção de Dispositivos

### Seus Direitos (variável por país)

| País | Situação |
|---|---|
| **Brasil** | Não há lei específica obrigando senha — mas dispositivos podem ser retidos |
| **EUA (CBSA)** | Agentes podem solicitar desbloqueio. Cidadãos têm proteção maior. Portadores de visto: alto risco de coerção |
| **UK** | Poder legal explícito de exigir senhas (RIPA) — recusa é crime |
| **China / Rússia / Belarus** | Inspeção de dispositivos comum, especialmente para jornalistas e ativistas |
| **UE (Schengen)** | Direitos mais protegidos, mas inspeção ainda possível |

### Estratégias para Fronteiras Difíceis

```
🔒 Opções por nível de risco:

[ Risco Baixo ]
• Criptografia de disco ativa + senha forte
• Fotos e arquivos sensíveis em nuvem criptografada (não no dispositivo)

[ Risco Médio ]
• Dispositivo de viagem separado com conteúdo mínimo
• Chaves de decriptação armazenadas remotamente (acesse depois de cruzar)

[ Risco Alto ]
• Dispositivo completamente vazio — restaurar dados via VPN após fronteira
• Tails em pendrive (sem dados persistentes)
• Volume oculto VeraCrypt para negação plausível
• Considerar enviar notebook por frete em vez de levar na bagagem
```

---

## 📶 WI-FI EM VIAGEM — Redes Não Confiáveis

### Riscos em Wi-Fi Público (hotéis, aeroportos, cafés)

- **MITM (Man-in-the-Middle)**: roteador comprometido intercepta tráfego
- **Evil Twin**: rede falsa com nome similar ao hotel/aeroporto
- **Captive portals maliciosos**: injetam JavaScript, coletam dados
- **ARP Spoofing**: redirecionamento de tráfego na mesma rede

### Protocolo Wi-Fi Seguro

```
✅ Sempre que conectar a Wi-Fi de hotel/aeroporto:

1. Verificar o nome exato da rede com a recepção (evitar Evil Twin)
2. Conectar → ATIVAR VPN IMEDIATAMENTE antes de qualquer navegação
3. Verificar que a VPN está ativa (checar em mullvad.net/check ou ipleak.net)
4. Usar HTTPS apenas — verificar cadeado em cada site
5. Não aceitar certificados SSL inválidos (alerta do browser)
6. Após uso: "esquecer" a rede Wi-Fi no dispositivo
```

### VPNs Recomendadas para Viagem

| VPN | Diferencial para Viagem | Link |
|---|---|---|
| **Mullvad VPN** | WireGuard, servidores em 40+ países, kill switch robusto | https://mullvad.net/ |
| **ProtonVPN** | Secure Core (multi-hop), Tor sobre VPN, kill switch | https://protonvpn.com/ |
| **IVPN** | Multi-hop, AntiTracker, muito confiável | https://www.ivpn.net/ |

> Para países com censura (China, Rússia, Irã): configure **bridges Tor** ou **Shadowsocks** antes de viajar — estas ferramentas podem não estar acessíveis de dentro do país.

---

## 📱 CHIP E CONECTIVIDADE

### Opções para Conexão no Exterior

| Opção | Privacidade | Custo | Considerações |
|---|---|---|---|
| **eSIM de viagem** (Airalo, Holafly) | ⚠️ Médio | Médio | Conveniente, mas requer cadastro e cartão |
| **Chip local pré-pago** | ✅ Melhor | Baixo | Comprar em dinheiro, exige documento em alguns países |
| **Roaming da operadora brasileira** | ❌ Baixo | Alto | Cara e rastreável pela operadora |
| **Roteador Wi-Fi portátil (Pocket Wi-Fi)** | ⚠️ Médio | Médio | Alugado — provedor tem seus dados |
| **Hotspot do celular** | Depende | — | Depende do chip usado |

> **Dica de privacidade:** Chip pré-pago comprado com dinheiro e sem vínculo a sua identidade oferece melhor isolamento de rastreamento por operadora.

---

## 🏨 SEGURANÇA NO HOTEL

- **Não deixe dispositivos no quarto** sem quartos trancados em cofre — mesmo safes de hotel são abertos pelo staff
- **Desconecte notebooks da rede** quando não estiver usando
- **Não use o computador do hotel** para acessar contas pessoais
- **Cuidado com carregadores USB públicos** (juice jacking) — use sempre adaptador de tomada ou cabo com Data Blocker
- **Se hospedar por longo período**: considere Tails em USB para não deixar rastros no ambiente
- **Camera/microfone do quarto**: câmeras ocultas em aluguéis por temporada são um problema real — verificar objetos suspeitos (despertadores, detectores de fumaça) com apps de detecção de RF

---

## 🆘 EMERGÊNCIAS NA VIAGEM

```
📋 Antes de viajar, prepare:

1. Número de emergência local (112 na UE, 911 nos EUA, 190 no Brasil)
2. Número do banco no exterior (verso do cartão) — para bloqueio imediato
3. Cópia do passaporte armazenada em nuvem criptografada (Proton Drive)
4. Contato de emergência familiar com acesso a informações necessárias
5. Seguro viagem com cobertura para dispositivos eletrônicos

Se o celular for roubado:
→ Wipe remoto (Find My / Prey)
→ Contato de emergência via Skype/WhatsApp Web em outro dispositivo
→ B.O. local + B.O. no Brasil (consulado pode ajudar)
→ Bloqueio do chip via operadora
```

---

## Países de Vigilância Elevada (atenção especial)

| País | Risco | Observação |
|---|---|---|
| 🔴 **China** | Muito alto | GFW bloqueia maioria das VPNs. Configure Shadowsocks/V2Ray antes. |
| 🔴 **Rússia** | Alto | Bloqueio de VPNs, vigilância ativa. Use Tor com bridges. |
| 🔴 **Irã** | Alto | Bloqueios extensivos. Tor com bridges ou Psiphon. |
| 🔴 **Bielorrússia** | Alto | Mesmo perfil da Rússia pós-2020. |
| 🟡 **EUA** | Médio (fronteira) | NSA surveillance history. Fronteira arriscada para non-citizens. |
| 🟡 **UK** | Médio | RIPA permite exigir senhas. Retenção de dados extensiva. |
| 🟡 **UAE / Emirados** | Médio-alto | VoIP bloqueado, VPN restrita, vigilância de comunicações. |
| 🟢 **UE (maioria)** | Baixo-médio | GDPR protege dados, mas Five Eyes participation em UK. |

## Regras

- A melhor proteção é levar menos dados — não carregue o que não precisa
- Criptografia antes de partir, não durante — não há como garantir integridade após inspeção
- Nunca conecte a redes antes de ativar a VPN
- Em caso de coerção física: a segurança pessoal é prioridade — dados podem ser trocados
