# CYBERSHIELD — Base de Conhecimento: Ferramentas de Segurança Digital e Privacidade

> **Versão:** 4.0 | **Atualização:** Abril 2026
> **Fonte primária:** "Proteja-se Online: Dicas e Softwares Essenciais para Sua Segurança Digital" (TWalking, 1ª Edição, Janeiro 2025)
> **Fontes complementares:** PrivacyGuides.org, PrivacyTools.io, EFF, awesome-selfhosted, auditorias independentes, documentação oficial das ferramentas.

---

## 6. VPNs

### [Camada 3 — Transporte]

| VPN | Open-Source | Jurisdição | No-Log Auditado | Protocolo Principal | Servidores | Dispositivos Simultâneos | Preço Mensal | Diferencial | Link |
|---|---|---|---|---|---|---|---|---|---|
| **Mullvad VPN** | ✅ Sim | Suécia | ✅ (auditoria independente) | WireGuard | ~800 / 39 países | 5 | €5/mês fixo | Registro anônimo (sem e-mail), aceita Monero e dinheiro por correio. Busca policial em 2023 não encontrou dados. | https://mullvad.net/pt |
| **ProtonVPN** | ✅ Sim | Suíça | ✅ (auditoria independente) | WireGuard/OpenVPN | ~2.900 / 65 países | 1-10 | Gratuito - €9,99 | Secure Core (multi-hop), Tor sobre VPN, NetShield (bloqueador), plano gratuito sem limite de dados | https://protonvpn.com/pt-br |
| **IVPN** | ✅ Sim | Gibraltar | ✅ (auditoria independente) | WireGuard/OpenVPN | ~90 / 30+ países | 7 | ~$6/mês | Multi-hop, AntiTracker, registro anônimo, aceita Monero | https://www.ivpn.net |
| **NordVPN** | ❌ Não | Panamá | ✅ (PwC) | NordLynx (WireGuard) | ~5.800 / 60 países | 6 | ~$3-12/mês | Double VPN, Threat Protection (bloqueio malware/anúncios), grande rede. ⚠️ Incidente em datacenter Finlândia 2018 (sem dados comprometidos). | https://nordvpn.com/pt-br/ |
| **ExpressVPN** | ❌ Não | Ilhas Virgens Britânicas | ✅ (PwC, KPMG) | Lightway | ~3.000 / 94 países | 5 | ~$6-13/mês | TrustedServer (RAM-only), velocidade premium. ⚠️ Adquirida pela Kape Technologies (2021). Vazamento DNS com split tunneling (2022-2024, corrigido). | https://www.expressvpn.com/pt |
| **Surfshark** | ❌ Não | Ilhas Virgens Britânicas → Holanda | ✅ (Deloitte, Cure53) | WireGuard | ~3.200 / 100 países | Ilimitado | ~$2-13/mês | Dispositivos ilimitados, CleanWeb, MultiHop, Rotating IP, Camouflage Mode | https://surfshark.com/pt-br |
| **Private Internet Access (PIA)** | ✅ Sim (cliente) | EUA | Parcial (Deloitte 2020) | WireGuard/OpenVPN | ~35.000 / 78 países | 10 | ~$2-12/mês | Maior rede de servidores, PIA MACE (bloqueador), no-logs comprovado em tribunal (2015, 2016). ⚠️ Sede nos EUA (5 Eyes). | https://www.privateinternetaccess.com/pt/ |
| **Windscribe** | ✅ Sim (cliente) | Canadá | Parcial | WireGuard/OpenVPN | ~480 / 69 países | Ilimitado | Grat. 10 GB/mês – ~$5,75/mês | R.O.B.E.R.T. (firewall DNS), Build-a-Plan, plano grat. generoso | https://windscribe.com/ |
| **AirVPN** | ✅ Sim (cliente) | Itália | Não auditado público | OpenVPN/WireGuard | ~250 / 23 países | 5 | ~€3-7/mês | Operada por ativistas, port forwarding, aceita cripto, transparência em tempo real | https://airvpn.org/ |
| **TorGuard** | ❌ Não | EUA | Parcial | WireGuard/OpenVPN | ~3.000 / 50 países | 8 | ~$5-10/mês | Foco em P2P, IPs dedicados | https://torguard.net/ |
| **OVPN** | Parcial | Suécia | ✅ Auditado | WireGuard/OpenVPN | ~110 / 29 países | 4-7 | ~$4-11/mês | Servidores RAM-only de propriedade própria, transparência legal | https://www.ovpn.com/ |
| **Hide.me** | Parcial | Malásia | ✅ Auditado | WireGuard/OpenVPN | ~2.400 / 90+ países | 10 | Grat. 10 GB – ~$5/mês | Plano grat. sem publicidade, kill switch | https://hide.me/ |
| **CyberGhost** | ❌ Não | Romênia | Parcial | WireGuard/OpenVPN | ~11.000 / 100 países | 7 | ~$2-13/mês | Servidores otimizados para streaming. ⚠️ Também do grupo Kape | https://www.cyberghostvpn.com/ |
| **TunnelBear** | ❌ Não | Canadá | ✅ Auditado | OpenVPN/IKEv2 | ~5.000 / 47 países | Ilimitado | Grat. 2 GB – ~$3-10/mês | Interface amigável para iniciantes (do grupo McAfee desde 2018) | https://www.tunnelbear.com/ |

### 6.1 Clientes VPN Open-Source (multi-protocolo)

| Cliente | Plataformas | Diferencial |
|---|---|---|
| **WireGuard (oficial)** | Multi | Cliente referência, leve, ideal para perfis manuais |
| **OpenVPN Connect** | Multi | Cliente oficial OpenVPN |
| **Tunnelblick** | macOS | GUI OpenVPN gratuita para macOS |
| **Viscosity** | Windows, macOS | OpenVPN profissional, pagamento único |
| **WG Easy** | Auto-hospedado | UI web para gerenciar peers WireGuard |

---

## 7. PROXIES

### [Camada 2 — Internet / Camada 3 — Transporte]

### 7.1 Proxies Pagos (mais seguros)

| Serviço | Tipo | Diferencial |
|---|---|---|
| **Smartproxy** | Residencial/Datacenter | Velocidade e confiabilidade, pool grande de IPs |
| **Oxylabs** | Residencial/Datacenter | Criptografia forte, APIs avançadas |
| **Bright Data** (ex-Luminati) | Residencial/Datacenter/Móvel | Recursos avançados de segurança, grande escala |
| **IPRoyal** | Residencial | Foco em privacidade |

### 7.2 Proxies Gratuitos (uso limitado)

| Serviço | Tipo | Observação |
|---|---|---|
| **Hide.me** | Web proxy | Versão gratuita limitada, boa reputação |
| **VPNBook** | Web proxy | Gratuito, sem registro |
| **HMA (HideMyAss)** | Web proxy | Opção gratuita de proxy web. ⚠️ Histórico controverso (logs entregues a autoridades) |

> ⚠️ **ATENÇÃO:** Proxies NÃO criptografam dados. Use apenas para contornar restrições geográficas, NUNCA para anonimato. Para proteção real, use VPN ou Tor.

---

## 8. REDE TOR E ANONIMATO DE REDE

### [Camada 2 — Internet]

| Ferramenta | Tipo | Diferencial |
|---|---|---|
| **Tor Browser** | Navegador | Navegação anônima via onion routing, 3 saltos, resistente a fingerprinting | https://www.torproject.org/ |
| **Tor Bridges** | Infraestrutura | Relays não listados para contornar bloqueio do Tor em países com censura |
| **Snowflake** | Transporte plugável | Transforma navegadores de voluntários em proxies de acesso ao Tor |
| **I2P** | Rede de anonimato | Alternativa ao Tor, focada em serviços internos (eepsites), garlic routing | https://geti2p.net/ |
| **Lokinet** | Rede de anonimato | Onion routing baseado em LLARP da Oxen, suporta qualquer protocolo IP | https://lokinet.org/ |
| **Freenet/Hyphanet** | Rede de anonimato | Datastore P2P resistente à censura | https://www.hyphanet.org/ |
| **ZeroNet** | Rede descentralizada | Sites P2P usando Bitcoin/BitTorrent (⚠️ manutenção irregular) | https://zeronet.io/ |
| **Yggdrasil** | Mesh network IPv6 | Rede mesh criptografada e auto-organizável | https://yggdrasil-network.github.io/ |
| **cwtch** | Mensagens via Tor | Mensageria P2P metadata-resistant via Tor | https://cwtch.im/ |
| **Orbot** | Cliente Tor (mobile/desktop) | Roteia tráfego de apps específicos via Tor | https://orbot.app/ |
| **Onion Browser (iOS)** | Navegador Tor | Navegador oficial Tor para iOS | https://onionbrowser.com/ |
| **obfs4 / meek / WebTunnel** | Pluggable transports | Disfarçam tráfego Tor para evitar DPI/censura |

---

## 16. DNS SEGURO E BLOQUEIO DE RASTREADORES

### [Camada 4 — Aplicação / Camada 2 — Internet]

### 16.1 Provedores DNS Criptografados

| Provedor | DoH | DoT | DNSSEC | Diferencial |
|---|---|---|---|---|
| **Quad9** (9.9.9.9) | ✅ | ✅ | ✅ | Sem fins lucrativos, bloqueio de malware, Suíça |
| **Cloudflare** (1.1.1.1) | ✅ | ✅ | ✅ | Rápido, auditado, opção family (1.1.1.3) |
| **Mullvad DNS** | ✅ | ✅ | ✅ | Bloqueio de anúncios/rastreadores, sem log |
| **NextDNS** | ✅ | ✅ | ✅ | Customizável, listas de bloqueio, logs opcionais |
| **AdGuard DNS** | ✅ | ✅ | ✅ | Bloqueio de anúncios/rastreadores integrado |
| **dns0.eu** | ✅ | ✅ | ✅ | DNS europeu, sem fins lucrativos |
| **ControlD** | ✅ | ✅ | ✅ | Custom profiles, regras geográficas, redirecionamento de serviços |
| **OpenDNS / Cisco Umbrella** | Parcial | ❌ | ✅ | Clássico, parental controls, da Cisco |
| **CleanBrowsing** | ✅ | ✅ | ✅ | Filtros family/adult/security, gratuito |
| **LibreDNS** | ✅ | ✅ | ✅ | Sem logs, foco em privacidade, sem censura |
| **DNSCrypt-proxy** | — | — | — | Cliente local que adiciona DNSCrypt/DoH a qualquer SO | https://dnscrypt.info/ |
| **Stubby** | — | ✅ | — | Cliente DNS-over-TLS local | https://dnsprivacy.org/ |
| **YogaDNS** | — | — | — | Cliente Windows que aplica regras (DoH/DoT/DoQ) por domínio | https://www.yogadns.com/ |

### 16.2 Bloqueadores de Rastreadores em Rede

| Ferramenta | Tipo | Diferencial |
|---|---|---|
| **Pi-hole** | DNS sinkhole (auto-hospedado) | Bloqueia anúncios e rastreadores em toda a rede doméstica |
| **AdGuard Home** | DNS sinkhole (auto-hospedado) | Alternativa ao Pi-hole com interface moderna, DoH/DoT nativo |
| **Technitium DNS Server** | DNS recursivo + sinkhole | Servidor DNS completo com bloqueio, DoH/DoT/DoQ | https://technitium.com/dns/ |
| **Blocky** | DNS proxy | DNS proxy rápido em Go, listas de bloqueio | https://0xerr0r.github.io/blocky/ |
| **DNSCloak (iOS)** | Cliente DoH/DoT | Cliente móvel para usar DoH em iOS | App Store |
| **Nebulo (Android)** | Cliente DoH/DoT/DNSCrypt | Cliente Android open-source | F-Droid |

---

## 21. SEGURANÇA DE REDE DOMÉSTICA

### [Camada 1 — Acesso à Rede / Camada 4 — Aplicação]

| Ferramenta | Tipo | Diferencial |
|---|---|---|
| **Pi-hole** | DNS sinkhole | Bloqueia anúncios e rastreadores em toda a rede |
| **AdGuard Home** | DNS sinkhole | Interface moderna, DoH/DoT nativo, filtros customizáveis |
| **pfSense** | Firewall/Router | Firewall open-source profissional |
| **OPNsense** | Firewall/Router | Fork do pfSense, interface moderna |
| **OpenWrt** | Firmware de roteador | Firmware open-source para roteadores, customizável |
| **DD-WRT** | Firmware de roteador | Clássico custom firmware, ampla compat |
| **FreshTomato** | Firmware de roteador | Sucessor do Tomato, foco em desempenho |
| **IPFire** | Firewall/Router | Distribuição Linux focada em firewall |
| **Untangle / Edge Threat Management** | Firewall/UTM | Plataforma UTM com módulos comerciais e gratuitos |
| **Suricata** | IDS/IPS | Engine de detecção de intrusão de alta performance |
| **Snort 3** | IDS/IPS | IDS clássico mantido pela Cisco, regras comunitárias |
| **Zeek (Bro)** | NSM | Network monitoring para análise comportamental |
| **Wireshark** | Análise | Sniffer/analisador de pacotes padrão da indústria |
| **nmap / Zenmap** | Scanner de rede | Mapeamento de hosts e portas, descoberta de devices |
| **Fing** | Mobile/Desktop | Detecção de devices na rede doméstica |
| **Angry IP Scanner** | Scanner | Scanner de IP/portas multiplataforma |
| **WireGuard / Tailscale / Headscale** | VPN mesh | VPN mesh para acessar rede doméstica remotamente |
| **NetBird** | VPN mesh | Alternativa open-source ao Tailscale |
| **ZeroTier** | SDN/VPN | Rede virtual P2P |
| **Nebula** | Mesh VPN | Mesh VPN da Slack, escalável |

---

## 53. OFUSCAÇÃO DE TRÁFEGO E ANTI-CENSURA

### [Camada 2/3]

| Ferramenta | Open-Source | Tipo | Diferencial | Link |
|---|---|---|---|---|
| **obfs4 / lyrebird** | ✅ Sim | Pluggable transport | Disfarça tráfego Tor como random | — |
| **meek** | ✅ Sim | Pluggable transport | Domain fronting (Azure/CDN) | — |
| **WebTunnel** | ✅ Sim | Pluggable transport | Tor disfarçado de tráfego HTTPS | https://webtunnel.torproject.org/ |
| **Snowflake** | ✅ Sim | Pluggable transport | WebRTC peers como bridges | https://snowflake.torproject.org/ |
| **V2Ray (Project V) / V2Fly** | ✅ Sim | Proxy | Múltiplos protocolos (VMess, VLESS, Trojan) | https://www.v2fly.org/ |
| **Xray-core** | ✅ Sim | Proxy | Fork avançado do V2Ray | https://xtls.github.io/ |
| **Shadowsocks** | ✅ Sim | Proxy | Proxy criptografado popular contra GFW | https://shadowsocks.org/ |
| **ShadowsocksR (legado)** | ✅ Sim | Proxy | Fork com mais ofuscações | — |
| **Trojan-GFW** | ✅ Sim | Proxy | Tráfego indistinguível de HTTPS | https://trojan-gfw.github.io/trojan/ |
| **Naïve Proxy** | ✅ Sim | Proxy | Baseado em Chrome network stack | https://github.com/klzgrad/naiveproxy |
| **Hysteria 2** | ✅ Sim | Proxy | UDP-based, alta velocidade em redes lossy | https://v2.hysteria.network/ |
| **Cloak** | ✅ Sim | Wrapper | Disfarça outros proxies como HTTPS | https://github.com/cbeuw/Cloak |
| **Outline VPN** | ✅ Sim | VPN/proxy | Baseado em Shadowsocks (Jigsaw/Google) | https://getoutline.org/ |
| **Lantern** | Parcial | Proxy | Anti-censura focado em mercados restritos | https://lantern.io/ |
| **Psiphon** | Parcial | Proxy/VPN | Anti-censura clássico | https://psiphon.ca/ |
| **GoodbyeDPI / Zapret / SpoofDPI** | ✅ Sim | DPI bypass | Burlam DPI sem servidor remoto | https://github.com/ValdikSS/GoodbyeDPI |
| **dnstt** | ✅ Sim | Túnel DNS | Túnel TCP sobre DoH/DoT (anti-censura) | https://www.bamsoftware.com/software/dnstt/ |

---

## 56. SERVIDORES VPN AUTO-HOSPEDADOS

### [Camada 3]

| Ferramenta | Open-Source | Tipo | Diferencial | Link |
|---|---|---|---|---|
| **WireGuard** | ✅ Sim | VPN moderna | Padrão atual: rápido, simples, baseado em Curve25519 | https://www.wireguard.com/ |
| **OpenVPN** | ✅ Sim | VPN clássica | Maduro, TLS, ampla compatibilidade | https://openvpn.net/ |
| **OpenVPN Access Server** | Parcial | VPN | Versão empresarial OpenVPN | — |
| **strongSwan** | ✅ Sim | IKEv2/IPsec | Implementação robusta IPsec | https://www.strongswan.org/ |
| **Libreswan** | ✅ Sim | IPsec | Fork de Openswan | https://libreswan.org/ |
| **PiVPN** | ✅ Sim | Wrapper | Setup automatizado WireGuard/OpenVPN em Linux | https://www.pivpn.io/ |
| **Algo VPN** | ✅ Sim | Provisionador | Provisiona VPN WireGuard em VPS automaticamente | https://github.com/trailofbits/algo |
| **Streisand** | ✅ Sim | Provisionador | Provisiona múltiplos protocolos anti-censura | https://github.com/StreisandEffect/streisand |
| **Outline Server** | ✅ Sim | Shadowsocks | Servidor Shadowsocks gerenciado (Jigsaw) | https://getoutline.org/ |
| **SoftEther** | ✅ Sim | Multi-proto | Suporta L2TP/IPsec/SSTP/OpenVPN/SoftEther | https://www.softether.org/ |
| **Tailscale** | Parcial | Mesh | Rede mesh sobre WireGuard (controle plano fechado) | https://tailscale.com/ |
| **Headscale** | ✅ Sim | Mesh | Implementação open-source do plano de controle Tailscale | https://headscale.net/ |
| **NetBird** | ✅ Sim | Mesh | Alternativa FOSS completa | https://netbird.io/ |
| **Nebula** | ✅ Sim | Mesh | Mesh VPN escalável (Slack) | https://github.com/slackhq/nebula |
| **ZeroTier** | Parcial | SDN | Rede virtual P2P | https://www.zerotier.com/ |
| **Innernet** | ✅ Sim | WireGuard | Rede WireGuard gerenciada por CRDT | https://github.com/tonarino/innernet |
| **WireGuard Easy (wg-easy)** | ✅ Sim | UI | UI Docker simples para WG | https://github.com/wg-easy/wg-easy |

---

