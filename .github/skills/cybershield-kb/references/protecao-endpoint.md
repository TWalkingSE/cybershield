# CYBERSHIELD — Base de Conhecimento: Ferramentas de Segurança Digital e Privacidade

> **Versão:** 4.0 | **Atualização:** Abril 2026
> **Fonte primária:** "Proteja-se Online: Dicas e Softwares Essenciais para Sua Segurança Digital" (TWalking, 1ª Edição, Janeiro 2025)
> **Fontes complementares:** PrivacyGuides.org, PrivacyTools.io, EFF, awesome-selfhosted, auditorias independentes, documentação oficial das ferramentas.

---

## 2. ANTIVÍRUS E PROTEÇÃO DE ENDPOINT

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Plataformas | Diferencial | Alerta de Privacidade |
|---|---|---|---|---|
| **ClamAV** | ✅ Sim | Windows, macOS, Linux | Antivírus open-source, ideal para servidores e scans sob demanda | ✅ Respeita privacidade |
| **Hypatia** | ✅ Sim | Android (via F-Droid) | Scanner de malware baseado em ClamAV para Android | ✅ Respeita privacidade |
| **Windows Defender** | ❌ Não | Windows 10/11 | Integrado ao Windows, proteção em tempo real, sem custo adicional | ⚠️ Telemetria Microsoft |
| **Bitdefender** | ❌ Não | Windows, macOS, Linux, Android, iOS | Excelente detecção, baixo impacto no sistema, VPN e firewall inclusos | ⚠️ Coleta telemetria |
| **Kaspersky** | ❌ Não | Windows, macOS, Linux, Android, iOS | Alta taxa de detecção, VPN e gerenciador de senhas inclusos | ⚠️ Preocupações geopolíticas (empresa russa) |
| **ESET NOD32** | ❌ Não | Windows, macOS, Linux, Android, iOS | Leve, proteção bancária, anti-phishing avançado | ⚠️ Coleta telemetria |
| **Sophos Home** | ❌ Não | Windows, macOS, Android, iOS | Gerenciamento remoto via painel web, protege até 10 dispositivos | ⚠️ Coleta telemetria |
| **Norton 360** | ❌ Não | Windows, macOS, Android, iOS | VPN, backup em nuvem, monitoramento de identidade | ⚠️ Coleta telemetria extensiva |
| **McAfee** | ❌ Não | Windows, macOS, Android, iOS, ChromeOS | Proteção familiar, monitoramento de identidade | ⚠️ Coleta telemetria extensiva |
| **Avast** | ❌ Não | Windows, macOS, Linux, Android, iOS | ⚠️ ALERTA: Multada em US$16,5M pela FTC em 2024 por vender dados de navegação dos usuários. Uso NÃO recomendado. | 🔴 Histórico de venda de dados |
| **Malwarebytes** | ❌ Não | Windows, macOS, Android, iOS | Excelente para remoção de malware/PUPs em modo on-demand, complementa AVs tradicionais | ⚠️ Telemetria moderada |
| **Emsisoft** | ❌ Não | Windows | Dual-engine, anti-ransomware comportamental, foco em PMEs | ⚠️ Telemetria |
| **F-Secure** | ❌ Não | Windows, macOS, Android, iOS | Finlandês, banking protection, VPN inclusa | ⚠️ Telemetria |
| **GData** | ❌ Não | Windows, macOS, Android | Alemão, dual-engine (Bitdefender + próprio), no-backdoor pledge | ⚠️ Telemetria |
| **chkrootkit** | ✅ Sim | Linux, macOS | Detector de rootkits clássico, CLI | ✅ Respeita privacidade |
| **rkhunter** | ✅ Sim | Linux, macOS | Rootkit Hunter, baseline de integridade do sistema | ✅ Respeita privacidade |
| **Lynis** | ✅ Sim | Linux, macOS, BSD | Auditoria de hardening de sistemas, checks de compliance | ✅ Respeita privacidade |
| **YARA** | ✅ Sim | Multi | Engine de regras para identificar malware (usado por SOCs) | ✅ Respeita privacidade |
| **Wazuh** | ✅ Sim | Multi | XDR/SIEM open-source com EDR para endpoints | ✅ Respeita privacidade |

---

## 33. FIREWALLS PESSOAIS (DESKTOP)

### [Camada 3 — Transporte / Camada 1 — Acesso à Rede]

| Ferramenta | Open-Source | Plataformas | Diferencial | Link |
|---|---|---|---|---|
| **Little Snitch** | ❌ Não | macOS | Firewall de aplicação com visualização de conexões em tempo real, controle granular | https://www.obdev.at/littlesnitch/ |
| **LuLu** | ✅ Sim | macOS | Firewall open-source para macOS, bloqueia conexões de saída não autorizadas | https://objective-see.org/products/lulu.html |
| **Portmaster** | ✅ Sim | Windows, Linux | Firewall de aplicação + DNS seguro + controle de privacidade por app | https://safing.io/portmaster/ |
| **simplewall** | ✅ Sim | Windows | Interface simples para Windows Filtering Platform (WFP), leve | https://github.com/henrypp/simplewall |
| **OpenSnitch** | ✅ Sim | Linux | Firewall de aplicação para Linux (similar ao Little Snitch) | https://github.com/evilsocket/opensnitch |
| **GlassWire** | ❌ Não | Windows, Android | Monitoramento visual de rede + firewall, detecta ameaças | https://www.glasswire.com/ |
| **Comodo Firewall** | ❌ Não | Windows | Firewall gratuito robusto com sandboxing de aplicações | https://www.comodo.com/home/internet-security/firewall.php |
| **UFW (Uncomplicated Firewall)** | ✅ Sim | Linux | Frontend simplificado para iptables, ideal para iniciantes Linux | — (nativo) |
| **firewalld** | ✅ Sim | Linux | Firewall dinâmico padrão em RHEL/Fedora | — |
| **nftables** | ✅ Sim | Linux | Sucessor moderno do iptables | — |
| **PFBlockerNG** | ✅ Sim | pfSense | Módulo para bloquear listas IP/DNS no pfSense | https://www.pfsense.org/ |
| **Sunshine Firewall (PFSense plugin)** | Parcial | pfSense | Painel amigável sobre pfSense | — |
| **TinyWall** | ✅ Sim | Windows | Wrapper leve para o firewall nativo do Windows | https://tinywall.pados.hu/ |
| **Windows Firewall Control** | ❌ Não | Windows | GUI avançada para Windows Defender Firewall | https://www.binisoft.org/ |
| **NetLimiter** | ❌ Não | Windows | Firewall + traffic shaping por aplicação | https://www.netlimiter.com/ |
| **PeerBlock** | ✅ Sim | Windows | Bloqueia ranges de IP por listas (legado, pouco mantido) | — |

---

## 38. SANDBOX E ISOLAMENTO DE APLICAÇÕES

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Plataformas | Diferencial | Link |
|---|---|---|---|---|
| **Sandboxie-Plus** | ✅ Sim | Windows | Sandbox clássico para isolar apps Windows, fork mantido | https://sandboxie-plus.com/ |
| **Windows Sandbox** | ❌ Não | Windows 10/11 Pro | Sandbox descartável nativo baseado em Hyper-V | — |
| **Firejail** | ✅ Sim | Linux | Sandbox via namespaces/seccomp, perfis prontos para 1000+ apps | https://firejail.wordpress.com/ |
| **Bubblewrap** | ✅ Sim | Linux | Sandbox de baixo nível usado pelo Flatpak | https://github.com/containers/bubblewrap |
| **Flatpak** | ✅ Sim | Linux | Apps em sandbox com permissões via portals | https://flatpak.org/ |
| **Snap** | Parcial | Linux | Sandboxing AppArmor da Canonical | https://snapcraft.io/ |
| **AppImage + Firejail** | ✅ Sim | Linux | AppImages portáteis isoladas com Firejail | — |
| **Toolbx / Distrobox** | ✅ Sim | Linux | Containers de desenvolvimento integrados ao host | https://distrobox.it/ |
| **Cuckoo Sandbox** | ✅ Sim | Linux | Sandbox para análise dinâmica de malware | https://cuckoosandbox.org/ |
| **CAPE Sandbox** | ✅ Sim | Linux | Fork moderno do Cuckoo focado em malware atual | https://github.com/kevoreilly/CAPEv2 |
| **Shade Sandbox** | ❌ Não | Windows | Sandbox simples para Windows | — |
| **macOS App Sandbox** | ❌ Não | macOS | Sandboxing nativo para apps da App Store | — |
| **gVisor** | ✅ Sim | Linux | Sandbox de container com kernel userspace (Google) | https://gvisor.dev/ |
| **Kata Containers** | ✅ Sim | Linux | Containers com isolamento de VM leve | https://katacontainers.io/ |

---

## 55. AUDITORIA DE APPS E ANÁLISE DE PERMISSÕES

### [Transversal]

| Ferramenta | Open-Source | Plataformas | Tipo | Diferencial | Link |
|---|---|---|---|---|---|
| **Exodus Privacy** | ✅ Sim | Android/Web | Análise estática | Lista rastreadores e permissões em apps Android | https://exodus-privacy.eu.org/ |
| **TrackerControl** | ✅ Sim | Android | Tempo real | Bloqueio de rastreadores via VPN local | https://trackercontrol.org/ |
| **MobSF (Mobile Security Framework)** | ✅ Sim | Multi | Análise | Análise estática/dinâmica para Android/iOS | https://mobsf.live/ |
| **Pithus** | ✅ Sim | Web | Análise | Sandbox público para APKs | https://beta.pithus.org/ |
| **App Manager** | ✅ Sim | Android | Auditoria | Inspeção avançada de apps Android | F-Droid |
| **Bouncer** | ❌ Não | Android | Permissões | Concede permissões temporárias | Play Store |
| **AppCensus** | — | Web | Análise | Estudos sobre rastreio em apps mobile | https://appcensus.io/ |
| **Privacy Indicator (iOS 14+/Android 12+)** | — | Nativo | UI | Indicadores nativos de mic/câmera/clipboard | — |
| **Oversight (macOS)** | ✅ Sim | macOS | Mic/cam | Notifica quando mic/câmera são usados | https://objective-see.org/products/oversight.html |
| **ReiKey (macOS)** | ✅ Sim | macOS | Keyloggers | Detecta keyloggers no macOS | https://objective-see.org/products/reikey.html |
| **KnockKnock (macOS)** | ✅ Sim | macOS | Persistência | Verifica softwares persistentes | https://objective-see.org/products/knockknock.html |
| **Autoruns (Sysinternals)** | ❌ Não | Windows | Persistência | Lista tudo que inicia com o Windows | — |
| **Process Hacker / System Informer** | ✅ Sim | Windows | Monitor | Substituto avançado do Task Manager | https://systeminformer.sourceforge.io/ |
| **HiddenVM Analyzer** | ✅ Sim | Multi | VM detection | Verifica detecção de VM por malware | — |

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

## 58. COMPARTILHAMENTO DE TELA E ACESSO REMOTO SEGURO

### [Camada 4]

| Ferramenta | Open-Source | Plataformas | Tipo | Diferencial | Link |
|---|---|---|---|---|---|
| **RustDesk** | ✅ Sim | Multi | Acesso remoto | Alternativa FOSS ao TeamViewer/AnyDesk, auto-hospedável | https://rustdesk.com/ |
| **MeshCentral** | ✅ Sim | Multi | Acesso remoto | Servidor web auto-hospedado para gerência remota | https://meshcentral.com/ |
| **Apache Guacamole** | ✅ Sim | Web | Gateway | Acesso a SSH/RDP/VNC via navegador | https://guacamole.apache.org/ |
| **TigerVNC / TightVNC** | ✅ Sim | Multi | VNC | Implementações VNC clássicas (use com SSH tunnel) | https://tigervnc.org/ |
| **NoMachine** | ❌ Não | Multi | Remote desktop | Performance alta, gratuito para uso pessoal | https://www.nomachine.com/ |
| **xrdp** | ✅ Sim | Linux | RDP | Servidor RDP para Linux | https://www.xrdp.org/ |
| **AnyDesk** | ❌ Não | Multi | Remote desktop | Comercial popular | — |
| **TeamViewer** | ❌ Não | Multi | Remote desktop | Comercial popular. ⚠️ Histórico de incidentes | — |
| **Chrome Remote Desktop** | ❌ Não | Multi | Remote desktop | Simples, requer conta Google | — |
| **OpenSSH (ssh -X / sshfs)** | ✅ Sim | Multi | SSH/X11 | Túneis seguros e GUI remota | https://www.openssh.com/ |
| **Mosh** | ✅ Sim | Multi | SSH resiliente | SSH para conexões instáveis | https://mosh.org/ |
| **Tactical RMM** | ✅ Sim | Multi | RMM | Ferramenta auto-hospedada de RMM | https://docs.tacticalrmm.com/ |

---

