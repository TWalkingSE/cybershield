---
name: seguranca-fisica
description: >
  Segurança física de dispositivos, ambientes e identidade presencial. Use quando
  o usuário perguntar sobre proteção contra roubo/perda de dispositivos, câmeras
  de segurança, telas de privacidade, espiões visuais (shoulder surfing), cartões
  RFID/NFC, segurança em escritórios/hotéis, vigilância física, proteção de
  periféricos (USB drops, evil maid attacks), ou qualquer ameaça que exija
  presença física do adversário. Também use para: "me roubaram o celular",
  "preciso de câmera de segurança", "proteção no trabalho", "wi-fi público".
---

# Segurança Física — Módulo Especializado

## Contexto

A segurança digital falha se a camada física for ignorada. Um adversário com acesso físico ao dispositivo pode contornar quase qualquer proteção de software. Atua em **[Camada 1 — Acesso à Rede]** e **[Transversal]**.

**Princípio central:** Segurança física e digital são complementares — uma não substitui a outra.

---

## 1. Proteção de Dispositivos Móveis (Celular/Notebook)

### Antes do Roubo (prevenção)
- **Criptografia de disco ativa** (BitLocker / FileVault / LUKS / criptografia Android — padrão Android 6+)
- **PIN/senha forte** — evite padrão deslizante (visível por manchas de dedo) e biometria como única autenticação
- **Bloqueio automático** em 30s–1min de inatividade
- **Disable USB debugging** (Android) e restringir boot por USB (BIOS/UEFI)
- **Localização remota ativa**: Find My (Apple), Find My Device (Google), Prey Project (FOSS, multi-plataforma)
- **Etiquetas de recuperação**: NFC ou código QR com contato alternativo (sem nome real se necessário)

### Após Roubo/Perda
```
🔴 AÇÕES IMEDIATAS (primeiros 30 minutos):

1. Wipe remoto: Find My / Find My Device / Prey Project
2. Revogar acesso: trocar senhas de contas no dispositivo
3. Invalidar sessões ativas (Google, Apple ID, redes sociais)
4. Notificar operadora: bloquear chip via IMEI (solicitar junto à operadora)
5. Registrar boletim de ocorrência (com IMEI — verificar em *#06#)
6. Revogar tokens 2FA: invalidar sessões em todos os apps de 2FA
7. Se necessário: notificar banco (cancelar cartões vinculados ao Google/Apple Pay)
```

### Ferramentas de Localização/Recuperação

| Ferramenta | Open-Source | Plataformas | Diferencial | Link |
|---|---|---|---|---|
| **Find My (Apple)** | ❌ | iOS, macOS | Rede Find My offline, localiza sem GPS via Bluetooth | — |
| **Find My Device (Google)** | ❌ | Android | Wipe remoto, bloqueio de emergência | — |
| **Prey Project** | ✅ Parcial | Multi | FOSS, multi-plataforma, timelapse e rastreamento | https://preyproject.com/ |
| **Cerberus** | ❌ | Android | Anti-roubo avançado, controle remoto, câmera furtiva | — |
| **Tile / AirTag** | ❌ | Multi | Rastreadores Bluetooth físicos | — |
| **Galaxy SmartTag (Samsung)** | ❌ | Android | Rastreadores UWB + Bluetooth | — |

---

## 2. Proteção Visual (Shoulder Surfing)

### Telas de Privacidade

| Produto | Ângulo de Privacidade | Uso Ideal |
|---|---|---|
| **3M Privacy Filters** | 60° (±30° do centro) | Notebook em espaços públicos, aviões |
| **Kensington MagPro** | 60° | Monitores de escritório |
| **VistaProtect (3M para celular)** | 60° | Smartphones |

- Use sempre em **transporte público, cafés, aeroportos e salas de reunião abertas**
- Em vídeo-chamada: posicione a câmera de costas para a parede (não para a sala)
- Prefira posições que deixem a tela voltada para a parede

### Anti-Câmeras de Visão

- **Tampa física de câmera (webcam cover)**: adesiva ou deslizante — proteção contra acesso indevido à câmera mesmo com malware ativo
- **Indicadores visuais de câmera/microfone**: no macOS e iOS, indicadores de hardware piscam ao ativar. No Android 12+, ícones aparecem na barra de status
- Ferramentas de detecção: **Oversight** (macOS), **Warden** (Android)

---

## 3. Ataques Físicos a Hardware

### Evil Maid Attack
**O que é:** adversário com acesso físico temporário ao dispositivo instala keylogger, bootkit ou copia disco sem seu conhecimento (em hotéis, fronteiras, etc.)

**Proteções:**
- **Secure Boot + TPM 2.0**: impede bootloader não assinado
- **Carimbo de borracha/esmalte sobre parafusos**: detecta abertura do case
- **BIOS/UEFI password**: dificulta boot de dispositivo externo
- **Tails/Whonix** em live USB: não usa o disco interno
- **Verificação de integridade**: ferramentas como **Heads** e **TPMTOTP** vinculam o estado de boot ao TPM

### USB Drops (dispositivos USB maliciosos abandonados)
- **NUNCA conecte** pen drives encontrados em locais públicos (ataque clássico de engenharia social)
- **USBGuard** (Linux): whitelist de dispositivos USB permitidos
- **USB Condom / PortaPow Data Blocker**: bloqueia dados, permite apenas carregamento
- Prefira carregadores de tomada a portas USB públicas (suscetíveis a juice jacking)

### Keyloggers de Hardware
- Inspecione visualmente o cabo entre teclado e computador em ambientes não confiáveis
- Use **teclado virtual** ou **teclado Bluetooth próprio** em terminais desconhecidos
- **Nitrokey / OnlyKey**: armazenam senhas no hardware — menos exposição ao teclado

---

## 4. Cartões RFID/NFC (Contacless)

**Risco:** Leitores de longa distância (até ~50cm) podem clonar cartões de crédito contactless, cartões de acesso e documentos com chip NFC.

| Proteção | Descrição |
|---|---|
| **Carteira bloqueadora de RFID** | Cage de Faraday embutida — bloqueia leituras não autorizadas |
| **Sleeve RFID para cartões individuais** | Forro de alumínio por cartão |
| **Desativar NFC** quando não usar | Configurações do smartphone |
| **Aplicar contactless apenas quando intencionalmente** | Não deixar cartão exposto em bolso externo |

- Documentos afetados: Cartão de crédito/débito contactless, passaporte com chip (RFID), cartões de acesso corporativo, RG digital

---

## 5. Câmeras de Segurança Residencial/Escritório (Privacidade)

| Ferramenta | Open-Source | Tipo | Diferencial | Link |
|---|---|---|---|---|
| **Frigate** | ✅ Sim | NVR local | Detecção de objetos com IA local (YOLOv8), sem nuvem | https://frigate.video/ |
| **Scrypted** | ✅ Sim | NVR/Hub | HomeKit + Google Home local, sem nuvem | https://www.scrypted.app/ |
| **MotionEye / MotionEyeOS** | ✅ Sim | NVR local | Interface web, gravação por movimento | https://github.com/motioneye-project/motioneye |
| **ZoneMinder** | ✅ Sim | NVR local | Clássico, robusto, muitas câmeras | https://www.zoneminder.com/ |
| **Shinobi** | ✅ Sim | NVR local | CCTV moderno, notificações, multi-servidor | https://shinobi.video/ |
| **go2rtc** | ✅ Sim | Streaming | Gateway de streams de câmeras para WebRTC/HLS | https://github.com/AlexxIT/go2rtc/ |

> ⚠️ **Câmeras de nuvem (Ring, Nest, Arlo, Wyze):** Enviam vídeo para servidores do fabricante. Políticas de compartilhamento com policiais/governo já foram documentadas. Para privacidade real, use NVR local.

---

## 6. Proteção em Viagens e Ambientes Hostis

> Para checklist completo de viagem, use `/checklist-viagem`.

**Resumo rápido:**
- Criptografia de disco ativa ANTES de viajar
- Considere levar dispositivo vazio ("travel device") com dados mínimos
- Em fronteiras: você pode ser forçado a desbloquear dispositivos legalmente em alguns países
- **Passphrase de negação plausível** (VeraCrypt hidden volume) para situações de coerção

---

## Regras

- Segurança física sem segurança digital = cofre de papel
- Segurança digital sem segurança física = porta blindada com janela aberta
- A combinação das duas é o que garante defense in depth real
- Adapte o nível ao modelo de ameaça: um ativista em país autoritário tem necessidades diferentes de um usuário casual
