---
name: mapa-tcpip
description: >
  Mapeamento completo de proteções de segurança digital organizadas por camada TCP/IP.
  Use quando o usuário quiser ver o panorama completo de proteções, visualizar 
  lacunas de segurança, entender onde cada ferramenta atua na rede, ou pedir 
  "mapa de segurança", "quais camadas estou protegido", "visão geral TCP/IP", 
  "o que falta na minha segurança". Essencial para qualquer resposta que precise 
  do framework TCP/IP completo como referência.
---

# Mapa TCP/IP — Framework de Proteções

## Camada 4 — Aplicação (Application Layer)
**Protocolos:** HTTP, HTTPS, DNS, SMTP, IMAP, FTP, SSH, TLS/SSL

**Proteções:**
- Navegadores seguros: Tor Browser, Mullvad Browser, Brave, Firefox hardened, LibreWolf, Ungoogled Chromium
- Buscadores: DuckDuckGo, Startpage, SearXNG, Brave Search, Mojeek
- DNS criptografado: DoH, DoT, DNSCrypt, DNSSEC (Quad9, Mullvad DNS, NextDNS)
- Aliases de e-mail: SimpleLogin, addy.io, Firefox Relay, Apple Hide My Email
- Mensageria: Signal, SimpleX Chat, Session, Briar, Element/Matrix
- Senhas e 2FA: KeePassXC, Bitwarden, Proton Pass / Aegis, Ente Auth, YubiKey
- Cloud segura: Proton Drive, Tresorit, Cryptomator + qualquer cloud, Nextcloud
- Criptografia de arquivos: VeraCrypt, age, GnuPG, Cryptomator, 7-Zip
- E-mail seguro: Proton Mail, Tuta, Mailfence / Thunderbird, FairEmail
- Notas criptografadas: Standard Notes, Joplin, Notesnook, CryptPad
- Transferência segura: OnionShare, Magic Wormhole, Croc, LocalSend
- Limpeza de metadados: ExifTool, mat2, Scrambled Exif
- Videoconferência: Jitsi Meet, Signal, Brave Talk
- Backup seguro: BorgBackup, Restic, Kopia
- Exclusão segura: BleachBit, shred, DBAN
- Anti-fingerprinting: ver skill `/fingerprinting`

## Camada 3 — Transporte (Transport Layer)
**Protocolos:** TCP, UDP, QUIC

**Proteções:**
- VPNs: Mullvad, ProtonVPN, IVPN (critérios: no-log auditado, jurisdição, WireGuard/OpenVPN, kill switch)
- Firewalls pessoais: Little Snitch, LuLu, Portmaster, OpenSnitch, simplewall
- Análise TLS/SSL: verificação de certificados, HSTS, certificate pinning
- TCP/IP stack fingerprinting: proteção e detecção

## Camada 2 — Internet (Internet Layer)
**Protocolos:** IP (IPv4/IPv6), ICMP, IPsec

**Proteções:**
- Rede Tor: onion routing, bridges, Snowflake (riscos de exit nodes)
- Proxies: SOCKS5, HTTP/HTTPS, proxy chains
- Proteção de IP: leak tests, IPv6 leaks, WebRTC leaks
- I2P (Invisible Internet Project)
- IPsec e túneis VPN de rede

## Camada 1 — Acesso à Rede (Network Access / Link Layer)
**Protocolos:** Ethernet, Wi-Fi (802.11), ARP, MAC

**Proteções:**
- Spoofing/randomização de MAC address
- Segurança Wi-Fi: WPA3, riscos de redes públicas
- Proteção de SSID, força de sinal, metadados de rede
- Proteção física: IMEI, dicas para celular

## Transversal (múltiplas camadas)
- SOs seguros: Tails, Whonix, Qubes OS, GrapheneOS, CalyxOS, Linux hardened
- Android privado: GrapheneOS, F-Droid, Aurora Store, NetGuard, RethinkDNS, Shelter
- iOS privado: Safari hardened, Lockdown Privacy, iCloud Private Relay
- VMs: VirtualBox, KVM/QEMU, Whonix
- Hardening de SO: firewall, AppArmor/SELinux, atualizações
- Criptografia de disco: LUKS, BitLocker (com cuidados), FileVault
- Chaves físicas: YubiKey, Nitrokey, SoloKeys, OnlyKey
- Sincronização: Syncthing, Rclone
- Calendários/contatos: Proton Calendar, EteSync, DAVx⁵

## Formato de Apresentação

Ao apresentar o mapa, destaque com ícones:
- ✅ Proteção ativa (se conhecida)
- ⚠️ Proteção parcial ou com ressalvas
- ❌ Sem proteção / lacuna identificada
- 🔲 Não avaliado

Se o perfil do usuário for conhecido, personalize destacando as lacunas.
