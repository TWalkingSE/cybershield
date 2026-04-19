# CYBERSHIELD — Base de Conhecimento: Ferramentas de Segurança Digital e Privacidade

> **Versão:** 4.0 | **Atualização:** Abril 2026
> **Fonte primária:** "Proteja-se Online: Dicas e Softwares Essenciais para Sua Segurança Digital" (TWalking, 1ª Edição, Janeiro 2025)
> **Fontes complementares:** PrivacyGuides.org, PrivacyTools.io, EFF, awesome-selfhosted, auditorias independentes, documentação oficial das ferramentas.

---

## 11. SISTEMAS OPERACIONAIS SEGUROS

### [Transversal — Múltiplas Camadas]

| SO | Open-Source | Base | Nível | Diferencial |
|---|---|---|---|---|
| **Tails** | ✅ Sim | Debian | Avançado | Live OS que roda de USB, roteia TODO tráfego via Tor, amnésico (sem rastros), criptografia LUKS |
| **Whonix** | ✅ Sim | Debian | Avançado | VM dupla (Gateway + Workstation), anonimato via Tor, isolamento de rede por design |
| **Qubes OS** | ✅ Sim | Xen hypervisor | Avançado | Segurança por compartimentalização (qubes/VMs isoladas), integração Whonix |
| **GrapheneOS** | ✅ Sim | AOSP | Avançado | Android sem Google, hardened, perfis isolados, apenas para Pixel |
| **CalyxOS** | ✅ Sim | AOSP | Intermediário | Android com microG (compatibilidade Google limitada), Datura Firewall |
| **LineageOS** | ✅ Sim | AOSP | Intermediário | Android custom ROM, ampla compatibilidade de dispositivos, sem Google |
| **Linux (geral)** | ✅ Sim | Variado | Todos | Open-source, customizável, AppArmor/SELinux, sem telemetria. Distribuições recomendadas: Fedora, Debian, Arch |
| **OpenBSD** | ✅ Sim | BSD | Avançado | Segurança por padrão, código auditado, criptografia forte, ASLR avançado |
| **Kicksecure** | ✅ Sim | Debian | Intermediário | Base do Whonix, hardening Debian sem necessariamente usar Tor |
| **Qubes-Whonix** | ✅ Sim | Xen + Debian | Avançado | Whonix rodando como qubes dentro do Qubes OS (combo máximo) |
| **DivestOS** | ✅ Sim | LineageOS fork | Intermediário | Android focado em privacidade para dispositivos antigos |
| **/e/OS** | ✅ Sim | LineageOS fork | Intermediário | Android desgooglificado com serviços Murena (alternativa amigável) |
| **iodeOS** | ✅ Sim | LineageOS fork | Intermediário | Foca em bloqueio de rastreadores em nível de sistema |
| **PureOS** | ✅ Sim | Debian | Intermediário | SO da Purism (Librem 5), endossado pela FSF |
| **postmarketOS** | ✅ Sim | Alpine | Avançado | Linux real para celulares (suporte 10+ anos por dispositivo) |
| **Parrot Security OS** | ✅ Sim | Debian | Avançado | Pentesting + privacidade, modo anonsurf integrado |
| **Kodachi** | ✅ Sim | Debian | Avançado | Live OS focado em anonimato, VPN+Tor+DNSCrypt encadeados |
| **Subgraph OS** | ✅ Sim | Debian | Avançado | Sandboxing por aplicação (Oz), kernel hardening (Grsecurity) |
| **Heads** | ✅ Sim | Debian | Avançado | Alternativa libre a Tails (sem blobs) |
| **Septor** | ✅ Sim | Debian | Intermediário | KDE + Tor por padrão, alternativa polõo ao Tails |
| **Alpine Linux** | ✅ Sim | musl/BusyBox | Avançado | Mínimo, hardened (PaX/grsec histórico), popular em containers |

---

## 20. MÁQUINAS VIRTUAIS E ISOLAMENTO

### [Transversal — Múltiplas Camadas]

| Ferramenta | Open-Source | Tipo | Diferencial |
|---|---|---|---|
| **VirtualBox** | ✅ Sim | Hypervisor tipo 2 | Gratuito, multiplataforma, fácil de usar |
| **KVM/QEMU** | ✅ Sim | Hypervisor tipo 1 (Linux) | Performance nativa, integração com libvirt |
| **Whonix** | ✅ Sim | VM pré-configurada | Gateway Tor + Workstation isolada |
| **VMware Workstation** | ❌ Não | Hypervisor tipo 2 | Performance profissional, snapshots avançados |
| **Hyper-V** | ❌ Não | Hypervisor tipo 1 (Windows) | Nativo Windows Pro/Enterprise, integração WSL2 |
| **Proxmox VE** | ✅ Sim | Hypervisor tipo 1 | Plataforma de virtualização empresarial baseada em KVM/LXC |
| **XCP-ng** | ✅ Sim | Hypervisor tipo 1 | Fork open-source do Citrix Hypervisor |
| **GNOME Boxes** | ✅ Sim | Linux | GUI simples para KVM |
| **virt-manager** | ✅ Sim | Linux | GUI clássica para libvirt/KVM |
| **UTM** | ✅ Sim | macOS, iOS | Frontend de QEMU para Apple Silicon |
| **Multipass** | ✅ Sim | Multi | VMs Ubuntu rápidas via CLI |
| **Vagrant** | ✅ Sim | Multi | Provisionamento de VMs reproduzível |
| **Docker / Podman** | ✅ Sim | Multi | Containerização; Podman é daemonless e rootless |
| **LXC / LXD / Incus** | ✅ Sim | Linux | Containers de sistema (não de aplicação) |

---

## 31. PRIVACIDADE NO ANDROID (APPS E CONFIGURAÇÃO)

### [Transversal — Múltiplas Camadas]

### 31.1 Lojas Alternativas e Desgooglificação

| Ferramenta | Open-Source | Diferencial | Link |
|---|---|---|---|
| **F-Droid** | ✅ Sim | Loja de apps exclusivamente FOSS (Free and Open Source Software) | https://f-droid.org/ |
| **Aurora Store** | ✅ Sim | Cliente anônimo para Google Play Store (sem conta Google) | https://auroraoss.com/ |
| **Obtainium** | ✅ Sim | Obtém APKs diretamente dos repositórios (GitHub, GitLab), sem loja intermediária | https://github.com/ImranR98/Obtainium |
| **Droid-ify** | ✅ Sim | Cliente F-Droid moderno com Material Design 3 | https://github.com/Droid-ify/client |

### 31.2 Firewalls e Controle de Rede

| Ferramenta | Open-Source | Root | Diferencial | Link |
|---|---|---|---|---|
| **NetGuard** | ✅ Sim | ❌ Não | Firewall sem root via VPN local, bloqueia acesso à internet por app | https://netguard.me/ |
| **AFWall+** | ✅ Sim | ✅ Sim | Firewall baseado em iptables, controle granular por app/UID | https://github.com/ukanth/afwall |
| **RethinkDNS** | ✅ Sim | ❌ Não | Firewall + DNS + bloqueio de rastreadores, tudo em um | https://rethinkdns.com/ |
| **TrackerControl** | ✅ Sim | ❌ Não | Monitora e bloqueia rastreadores em tempo real, baseado no TrackerDB | https://trackercontrol.org/ |
| **Blokada** | ✅ Sim | ❌ Não | Bloqueador de anúncios e rastreadores no nível de DNS | https://blokada.org/ |

### 31.3 Isolamento e Perfis

| Ferramenta | Open-Source | Diferencial |
|---|---|---|
| **Shelter** | ✅ Sim | Cria perfil de trabalho isolado (Work Profile) para apps, usando funcionalidade nativa Android |
| **Insular** | ✅ Sim | Fork do Island, isola apps em sandbox usando perfil de trabalho |

### 31.4 Teclados Seguros

| Ferramenta | Open-Source | Diferencial | Link |
|---|---|---|---|
| **OpenBoard** | ✅ Sim | Teclado FOSS baseado no AOSP, sem conexão à internet | https://github.com/openboard-team/openboard |
| **HeliBoard** | ✅ Sim | Fork ativo do OpenBoard com melhorias, sem telemetria | https://github.com/Helium314/HeliBoard |
| **FlorisBoard** | ✅ Sim | Teclado moderno FOSS, extensível, em desenvolvimento ativo | https://florisboard.org/ |
| **AnySoftKeyboard** | ✅ Sim | Teclado FOSS com suporte a 200+ idiomas, sem rastreamento | https://anysoftkeyboard.github.io/ |

### 31.5 Outros Apps Android para Privacidade

| Ferramenta | Função | Link |
|---|---|---|
| **Scrambled Exif** | Remove metadados de fotos antes de compartilhar | F-Droid |
| **Fake GPS** | Simula localização GPS | Play Store |
| **Orbot** | Proxy Tor para Android (roteia apps pela rede Tor) | https://orbot.app/ |
| **NewPipe** | Cliente YouTube sem rastreamento Google, sem conta necessária | https://newpipe.net/ |
| **Organic Maps** | Mapas offline baseados em OpenStreetMap, sem rastreamento | https://organicmaps.app/ |
| **InviZible Pro** | DNSCrypt + Tor + I2P combinados em um app | F-Droid |
| **Exodus Privacy** | Auditoria de rastreadores e permissões em apps Android | https://exodus-privacy.eu.org/ |
| **TrackerControl** | Bloqueio de rastreadores em apps em tempo real | https://trackercontrol.org/ |
| **Warden** | Detecção de stalkerware em Android | F-Droid |
| **Hypatia** | Scanner antimalware FOSS para Android | F-Droid |
| **Briar** | Mensageria P2P offline-first (Tor/Wi-Fi/BT) | https://briarproject.org/ |
| **AntennaPod** | Cliente de podcasts FOSS sem rastreio | https://antennapod.org/ |
| **OsmAnd** | Mapas offline OpenStreetMap | https://osmand.net/ |
| **LibreTube** | Front-end YouTube via Piped sem Google | F-Droid |
| **NewPipe Sponsorblock** | NewPipe + SponsorBlock | F-Droid |
| **Tor Browser (Android)** | Versão oficial Tor para Android | https://www.torproject.org/ |
| **Bitwarden / KeePassDX** | Gerenciamento de senhas no Android | F-Droid / Play |
| **Aegis Authenticator** | TOTP com backup criptografado | https://getaegis.app/ |
| **DAVx⁵** | Sync CalDAV/CardDAV | https://www.davx5.com/ |
| **K-9/Thunderbird Mobile** | Cliente de e-mail FOSS | https://k9mail.app/ |
| **Document Viewer** | PDF reader minimalista FOSS | F-Droid |
| **Secure Camera** | Câmera com remoção automática de EXIF (GrapheneOS) | — |
| **Tasks.org** | Lista de tarefas FOSS com sync DAV | https://tasks.org/ |

---

## 32. PRIVACIDADE NO iOS

### [Transversal — Múltiplas Camadas]

| Ferramenta/Configuração | Tipo | Diferencial |
|---|---|---|
| **Safari** (hardened) | Navegador | Anti-fingerprinting nativo, Intelligent Tracking Prevention, isola cookies |
| **Lockdown Privacy** | Firewall | Firewall on-device para iOS, bloqueia rastreadores, open-source |
| **AdGuard Pro** | DNS/Bloqueador | Bloqueio de anúncios e rastreadores via DNS no nível do sistema |
| **Apple Mail + S/MIME** | E-mail | Suporte nativo a S/MIME para criptografia de e-mail |
| **Apple Hide My Email** | Aliases | Aliases de e-mail integrados ao iCloud+ |
| **iCloud Private Relay** | Proxy | Proxy de privacidade da Apple para Safari (oculta IP de sites) |
| **Brave (iOS)** | Navegador | Bloqueio nativo de rastreadores e anúncios |
| **Signal (iOS)** | Mensageiro | E2EE por padrão |
| **Orbot (iOS)** | Proxy Tor | Roteia tráfego via Tor no iOS |
| **Metapho** | Metadados | Visualiza e remove metadados de fotos no iPhone |
| **ProtonVPN (iOS)** | VPN | VPN open-source com plano gratuito |
| **1Blocker / Wipr / AdGuard** | Content blocker | Content blockers nativos do Safari |
| **Better Blocker** | Content blocker | Content blocker focado em ética/privacidade |
| **Firefox Focus (iOS)** | Navegador | Apaga sessão ao sair, usa WebKit |
| **Onion Browser** | Navegador Tor | Cliente Tor oficial para iOS |
| **Strongbox** | Senhas | Compatível com KeePass, integração iCloud |
| **KeePassium** | Senhas | Cliente KeePass moderno para iOS |
| **Raivo OTP / Tofu / OTP Auth** | 2FA | Apps TOTP nativos com backup iCloud |
| **DAVx⁵ alternatives (CardBook/CalDAV-Sync)** | Sync DAV | Sync de calendário/contatos com servidor próprio |
| **Stealth iCloud Backup encryption (Advanced Data Protection)** | Configuração | Habilitar ADP no iCloud para E2EE de backups (iOS 16.3+) |

> **Dica iOS:** Desative: Siri & Ditado (dados enviados à Apple), Analytics (Configurações > Privacidade > Analytics), Personalização de Anúncios, Localização para apps desnecessários.

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

