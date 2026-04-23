# CYBERSHIELD — Base de Conhecimento: Ferramentas de Segurança Digital e Privacidade

> **Versão:** 4.0 | **Atualização:** Abril 2026
> **Fonte primária:** "Proteja-se Online: Dicas e Softwares Essenciais para Sua Segurança Digital" (TWalking, 1ª Edição, Janeiro 2025)
> **Fontes complementares:** PrivacyGuides.org, EFF, OWASP IoT Security, NIST IR 8259, awesome-selfhosted.

---

## 61. SEGURANÇA DE DISPOSITIVOS IoT (Internet of Things)

### [Camada 1 — Acesso à Rede / Camada 4 — Aplicação]

IoT abrange câmeras IP, smart TVs, assistentes de voz, fechaduras inteligentes, termostatos, roteadores, NAS, impressoras e qualquer dispositivo "inteligente" conectado à rede doméstica.

### 61.1 Riscos Específicos de IoT

| Risco | Descrição | Impacto |
|---|---|---|
| **Senhas padrão** | Fabricantes usam credenciais genéricas (admin/admin, 1234) | Acesso imediato por qualquer atacante |
| **Firmware desatualizado** | Vulnerabilidades conhecidas nunca corrigidas | Comprometimento remoto |
| **Comunicação sem TLS** | Dados transmitidos em texto claro | Interceptação por MITM |
| **Cloud obrigatória** | Dispositivo requer conta no servidor do fabricante | Dados de uso enviados sem consentimento claro |
| **UPnP habilitado** | Abre portas automaticamente no roteador sem aviso | Exposição de serviços internos à internet |
| **Assistentes de voz** | Gravações armazenadas em servidores dos fabricantes | Análise de conversas privadas |
| **Câmeras IP** | Streams acessíveis via internet se mal configuradas | Violação de privacidade, vigilância não autorizada |
| **Smart TV** | Coleta de dados de visualização, ACR (Automatic Content Recognition) | Perfil comportamental detalhado |
| **Pivoting** | Dispositivo IoT comprometido como ponto de entrada para a rede | Acesso a todos os outros dispositivos |

### 61.2 Proteções Essenciais (toda instalação IoT)

```
🔒 CHECKLIST DE SEGURANÇA IoT

✅ CRÍTICO:
1. Trocar senha padrão por senha forte e única em CADA dispositivo
2. Atualizar firmware imediatamente após instalação e monitorar atualizações
3. Criar VLAN/rede Wi-Fi separada para dispositivos IoT (isolamento)
4. Desabilitar UPnP no roteador
5. Desabilitar acesso remoto via internet se não for necessário

✅ RECOMENDADO:
6. Desativar funções não usadas (câmera, microfone, Bluetooth, Zigbee)
7. Verificar se o fabricante tem histórico de atualizações e suporte longo
8. Preferir dispositivos com firmware open-source ou self-hostable
9. Bloquear acesso à internet do dispositivo no firewall do roteador
   (Pi-hole ou pfSense para controle por dispositivo)
10. Monitorar tráfego de saída (Wireshark, Zeek, ou roteador com logs)

✅ AVANÇADO:
11. VLAN dedicada com firewall entre VLAN IoT e rede principal
12. IDS/IPS (Suricata no pfSense/OPNsense) monitorando tráfego IoT
13. Substituir firmware de fábrica por open-source quando possível (OpenWrt, Tasmota)
14. Desconectar dispositivos da internet e usar apenas localmente (Zigbee, Z-Wave local)
```

### 61.3 Isolamento de Rede (VLAN IoT)

A segmentação de rede é a proteção mais eficaz para IoT:

| Configuração | Ferramentas | Resultado |
|---|---|---|
| **SSID separado no roteador** | Qualquer roteador dual-band | IoT em banda 2.4GHz, devices pessoais em 5GHz — separação básica |
| **VLAN com regras de firewall** | pfSense, OPNsense, OpenWrt | IoT não pode acessar rede principal; tráfego da internet ainda permitido |
| **VLAN sem acesso à internet** | pfSense/OPNsense + Zigbee2MQTT | IoT 100% local — sem comunicação com servidores do fabricante |

### 61.4 Assistentes de Voz (Alexa, Google Home, Siri)

| Dispositivo | Privacidade | Alternativa Local |
|---|---|---|
| **Amazon Alexa** | ⚠️ Gravações armazenadas na AWS. Amazon pode acessar. | Home Assistant + Whisper local |
| **Google Nest/Home** | ⚠️ Historial de comandos no Google. Treinamento de modelos. | Home Assistant + Rhasspy/Wyoming |
| **Apple HomePod/Siri** | ⚠️ Melhor entre os três, mas ainda envia áudio à Apple. Processamento on-device parcial | — |
| **Home Assistant** | ✅ 100% local, sem nuvem obrigatória, open-source | https://www.home-assistant.io/ |
| **openHAB** | ✅ 100% local, Java-based, ampla compatibilidade | https://www.openhab.org/ |

> **Para máxima privacidade:** Desconecte assistentes de voz da rede quando não usar, ou prefira automação local via Home Assistant com microfone local (Whisper.cpp + Piper TTS).

### 61.5 Câmeras IP — Configuração Segura

| Ferramenta/Configuração | Descrição |
|---|---|
| **Frigate (NVR local)** | IA de detecção de objetos 100% local, sem nuvem | https://frigate.video/ |
| **Credencial única por câmera** | Nunca usar admin/admin ou senha igual em todas |
| **Stream RTSP com credenciais** | Habilitar autenticação no stream RTSP |
| **Desabilitar P2P cloud** | Muitas câmeras enviam stream via cloud mesmo sem pedir |
| **VLAN sem internet** | Câmera IP sem acesso à internet = nenhuma exfiltração |
| **Verificar marca antes de comprar** | Marcas com histórico de backdoors: Hikvision ⚠️, Dahua ⚠️ (banidas por órgãos governamentais em EUA/UK) |

### 61.6 Smart TVs — Mitigação de ACR

ACR (Automatic Content Recognition) captura frames do que você assiste e envia para servidores do fabricante e anunciantes.

| Ação | Como fazer |
|---|---|
| **Recusar ACR na configuração inicial** | Durante o setup, recusar coleta de dados de visualização |
| **Desativar nas configurações** | Samsung: Configurações > Suporte > Termos & Política > Política de Visualização de Conteúdo. LG: Configurações > Opções > Live Plus (desativar) |
| **Bloquear no DNS** | Pi-hole com listas específicas por marca bloqueia servidores ACR |
| **Usar mídia via HDMI** | Conectar Raspberry Pi / mini PC como source evita o sistema da TV |
| **Apple TV / Chromecast / Fire Stick** | Ainda enviam dados, mas geralmente menos que TVs com sistema nativo |
| **Raspberry Pi 4 + LibreELEC/Kodi** | Reprodução de mídia 100% local e privada |

### 61.7 Ferramentas de Monitoramento e Segurança de Rede IoT

| Ferramenta | Tipo | Diferencial | Link |
|---|---|---|---|
| **Home Assistant** | Automação local | Hub de IoT 100% local, suporta Zigbee, Z-Wave, MQTT | https://www.home-assistant.io/ |
| **Zigbee2MQTT** | Bridge local | Conecta dispositivos Zigbee ao MQTT sem cloud | https://www.zigbee2mqtt.io/ |
| **Z-Wave JS** | Bridge local | Suporte a dispositivos Z-Wave localmente | https://zwave-js.github.io/ |
| **Frigate** | NVR | CCTV local com IA de detecção | https://frigate.video/ |
| **Pi-hole + listas IoT** | DNS sinkhole | Bloqueia telemetria de dispositivos por domínio | https://pi-hole.net/ |
| **AdGuard Home** | DNS sinkhole | Alternativa ao Pi-hole, mais amigável | https://adguard.com/adguard-home/ |
| **OpenWrt** | Firmware de roteador | Controle total — VLAN, firewall, monitoramento | https://openwrt.org/ |
| **pfSense / OPNsense** | Firewall | VLAN IoT com regras granulares, IDS/IPS integrado | https://opnsense.org/ |
| **Suricata** | IDS/IPS | Detecção de comportamento anômalo em tráfego IoT | https://suricata.io/ |
| **Fing** | Scanner de rede | Descobre dispositivos IoT desconhecidos na rede | https://www.fing.com/ |
| **nmap** | Scanner | Auditoria de portas abertas em dispositivos IoT | https://nmap.org/ |
| **IoT Inspector (Princeton)** | Análise de tráfego | Análise de privacidade de dispositivos IoT | https://iotinspector.org/ |
| **Tasmota** | Firmware alternativo | Firmware open-source para dispositivos Tuya/Sonoff, sem cloud | https://tasmota.github.io/ |
| **ESPHome** | Firmware | Firmware ESP8266/ESP32 para automação local | https://esphome.io/ |
| **WLED** | Firmware | Firmware de tiras LED com controle local | https://kno.wled.ge/ |
| **Mosquitto** | MQTT Broker | Broker MQTT local para comunicação IoT sem cloud | https://mosquitto.org/ |
| **Node-RED** | Automação | Fluxos de automação IoT locais, visual | https://nodered.org/ |

### 61.8 Protocolo de Compra Consciente de IoT

Antes de comprar um dispositivo IoT, verifique:

- [ ] O dispositivo funciona sem internet? (modo local?)
- [ ] Tem suporte a firmware alternativo (Tasmota, ESPHome)?
- [ ] O fabricante tem histórico de atualizações de segurança?
- [ ] Qual a política de dados e por quanto tempo o suporte de cloud é garantido?
- [ ] O app requer conta obrigatória? Os dados vão para qual país?
- [ ] Há protocolos locais suportados? (Zigbee, Z-Wave, Matter, MQTT)

> **Protocolo Matter (2022+):** Padrão aberto da Connectivity Standards Alliance (Google, Apple, Amazon, Samsung). Funciona localmente sem internet obrigatória. Prefira dispositivos com certificação Matter para automação futura sem lock-in.

---

## 62. SEGURANÇA FÍSICA E DISPOSITIVOS PORTÁTEIS

### [Camada 1 — Acesso à Rede / Transversal]

> Para proteção física detalhada, use o skill `/seguranca-fisica`.

| Categoria | Ferramentas/Práticas | Link |
|---|---|---|
| **Telas de privacidade** | 3M Privacy Filter, Kensington MagPro, VistaProtect (celular) | — |
| **Tampas de webcam** | Vários modelos físicos deslizantes — proteção contra acesso de câmera por malware | — |
| **USB Data Blocker** | PortaPow, CableCreation — carregamento seguro em USB públicos | — |
| **Carteiras RFID** | Bloqueadores de leitura contactless para cartões e passaporte | — |
| **Rastreadores GPS/BT** | Apple AirTag, Tile, Samsung SmartTag (detecção anti-stalking em iOS/Android nativo) | — |
| **Prey Project** | Localização/wipe remoto de notebook/celular open-source | https://preyproject.com/ |
| **Trava Kensington** | Trava física para notebooks em ambientes públicos/escritório | — |
| **Faraday Bag** | Saco que bloqueia sinais (GPS, GSM, Wi-Fi, Bluetooth) — útil em fronteiras | — |

---
