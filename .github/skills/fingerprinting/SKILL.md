---
name: fingerprinting
description: >
  Módulo especializado em impressão digital (fingerprinting) de navegadores e dispositivos.
  Use quando o usuário perguntar sobre fingerprinting, rastreamento sem cookies, 
  Canvas fingerprinting, WebGL fingerprint, AudioContext fingerprint, supercookies, 
  evercookies, tracking cross-site, browser uniqueness, anti-fingerprinting, 
  ou como sites identificam visitantes sem cookies. Também use quando o tema 
  envolver BrowserLeaks, CreepJS, FingerprintJS, AmIUnique, ou proteção contra 
  rastreamento avançado.
---

# Fingerprinting — Módulo Especializado

## Contexto

Fingerprinting é a técnica de identificar um dispositivo/navegador por suas características únicas, sem usar cookies ou login. Atua na **[Camada 4 — Aplicação]** via APIs do navegador.

**Conceito-chave:** a melhor defesa é **uniformidade** — seu fingerprint deve ser idêntico ao de milhares de outros usuários, não apenas diferente do seu fingerprint real.

## Categorias de Fingerprinting

Organize SEMPRE a resposta nestas categorias quando relevante:

### 1. Identificadores de Sistema e Navegador
- Arquitetura do sistema, user-agent, modo de navegação
- Cabeçalhos HTTP, suporte a cookies/JS/DNT
- Detecção de Tor/VPN, métodos de autenticação
- **Proteção:** Tor Browser/Mullvad Browser (normalizam user-agent), Firefox com `privacy.resistFingerprinting`

### 2. Hardware e Sensores
- Touchscreen, câmera/microfone, giroscópio, acelerômetro
- Sensores de luz/proximidade, nível de bateria, Bluetooth, NFC, biometria
- **Proteção:** Permissões restritivas, GrapheneOS (sensores controlados), desabilitar APIs desnecessárias

### 3. Gráficos e Renderização
- **WebGL**: vendor, renderer, extensions, tamanho máximo de textura
- **Canvas fingerprinting**: renderização de texto/gráficos produz hash único por hardware+driver+SO
- Capacidade de codificação de vídeo, suporte VR/AR, múltiplos monitores
- **Proteção:** Brave Shields (ruído em Canvas/WebGL), CanvasBlocker (Firefox), Tor Browser (normaliza)

### 4. Armazenamento e Persistência
- Cookies HTTP/persistentes, supercookies, ETags
- Flash cookies (LSOs), Evercookies
- Local/Session Storage, IndexedDB, Cache, Web SQL, Prefetch Cache
- **Proteção:** Containers de navegador (Firefox Multi-Account), limpeza automática, extensões como Cookie AutoDelete

### 5. APIs e Contextos de Execução
- **AudioContext fingerprinting**: `OscillatorNode` → `DynamicsCompressorNode` → hash único (~35 bits de entropia)
- Clipboard, Service Workers, geolocalização
- **WebRTC**: vazamento de IP local mesmo com VPN
- Vibration API, Idle Detection API
- **Proteção:** `media.peerconnection.enabled = false` (WebRTC), `dom.webaudio.enabled = false` (áudio), Brave Shields

### 6. Rede e Conexão
- IPs (IPv4/IPv6), proxies, MAC (quando acessível)
- Tipo de rede, velocidade, SSID, operadoras
- Handshake TLS, TCP/IP stack fingerprinting, servidores DNS
- **Proteção:** VPN (IP), Tor (IP+TLS), DNS criptografado, desabilitar IPv6 se não usar

### 7. Identificadores de Dispositivo
- IMEI, UUID, IDFA (Apple), GAID (Google)
- FingerprintJS, Device ID de apps, metadata de dispositivo
- **Proteção:** GrapheneOS (reset IDs por app), limitar tracking IDs nas configurações do SO

## Protocolo de Resposta

Para CADA subcategoria mencionada, explique:
1. **O QUE** é coletado
2. **COMO** é usado para rastreamento
3. **COMO** se proteger (ferramentas concretas + configurações)

## Ferramentas de Teste

Recomende para o usuário testar seu próprio fingerprint:
- **BrowserLeaks** (browserleaks.com) — teste abrangente por categoria
- **CreepJS** — detecção avançada de spoofing
- **AmIUnique** — comparação com base de dados de fingerprints
- **Mullvad Check** (mullvad.net/check) — verificação rápida
- **Cover Your Tracks** (EFF) — teste de rastreabilidade

## Exemplo de Resposta Avançada (AudioContext)

Quando perguntado sobre AudioContext especificamente, inclua:
- Mecanismo: `OscillatorNode` (triangle, 10000Hz) → `DynamicsCompressorNode` → `AnalyserNode` → `getFloatFrequencyData()`/`getChannelData()` → hash
- A saída varia por: hardware de áudio, drivers, versão do SO, implementação do navegador
- Funciona em modo privado, persiste entre sessões, sem permissões especiais
- Mitigações tabuladas com eficácia e trade-offs

## Referências

- Paper: "AudioContext Fingerprint Test Page"
- FingerprintJS documentation (open-source version)
- MDN Web Audio API, W3C Web Audio API spec
- EFF Cover Your Tracks methodology
