# CYBERSHIELD — Base de Conhecimento: Ferramentas de Segurança Digital e Privacidade

> **Versão:** 4.0 | **Atualização:** Abril 2026
> **Fonte primária:** "Proteja-se Online: Dicas e Softwares Essenciais para Sua Segurança Digital" (TWalking, 1ª Edição, Janeiro 2025)
> **Fontes complementares:** PrivacyGuides.org, PrivacyTools.io, EFF, awesome-selfhosted, auditorias independentes, documentação oficial das ferramentas.

---

## 9. NAVEGADORES SEGUROS

### [Camada 4 — Aplicação]

### 9.1 Desktop

| Navegador | Open-Source | Motor | Diferencial | Link |
|---|---|---|---|---|
| **Tor Browser** | ✅ Sim | Firefox/Gecko | Máximo anonimato via rede Tor, anti-fingerprinting uniforme | https://www.torproject.org/ |
| **Mullvad Browser** | ✅ Sim | Firefox/Gecko | Baseado no Tor Browser SEM Tor, anti-fingerprinting máximo, uso com Mullvad VPN | https://mullvad.net/en/browser/ |
| **LibreWolf** | ✅ Sim | Firefox/Gecko | Firefox sem telemetria, pré-configurado para privacidade, uBlock Origin incluído | https://librewolf.net |
| **Firefox** (hardened) | ✅ Sim | Gecko | Com Arkenfox user.js: anti-fingerprinting, sem telemetria. Configuração manual necessária. | https://www.mozilla.org/firefox |
| **Brave** | ✅ Sim | Chromium/Blink | Bloqueio nativo de anúncios/rastreadores, anti-fingerprinting. ⚠️ Incidente links de afiliado (2020, corrigido). BAT/Rewards opcional. | https://brave.com |
| **Ungoogled Chromium** | ✅ Sim | Chromium/Blink | Chromium sem conexões Google, sem telemetria, sem auto-update Google | https://ungoogled-software.github.io/ |
| **DuckDuckGo Privacy Browser** | ✅ Sim | WebKit | Foco em privacidade, bloqueio de rastreadores, Fire Button (limpar tudo). ⚠️ Exceção Microsoft Advertising (2022, mitigado). | https://duckduckgo.com/app |
| **Epic Browser** | ❌ Não | Chromium/Blink | Proxy embutido, sem histórico/cache por padrão, bloqueia fingerprinting | https://www.epicbrowser.com |
| **Waterfox** | ✅ Sim | Gecko | Fork de Firefox sem telemetria, suporte a extensões legacy | https://www.waterfox.net/ |
| **IceCat** | ✅ Sim | Gecko | Versão GNU do Firefox, 100% software livre | https://www.gnu.org/software/gnuzilla/ |
| **Pale Moon** | ✅ Sim | Goanna (fork Gecko) | Foco em customização e desempenho, motor próprio | https://www.palemoon.org/ |
| **Vivaldi** | Parcial | Chromium/Blink | Altamente customizável, bloqueador embutido. ⚠️ UI proprietária | https://vivaldi.com/ |
| **Thorium** | ✅ Sim | Chromium | Chromium otimizado para velocidade e privacidade | https://thorium.rocks/ |
| **Zen Browser** | ✅ Sim | Gecko | Fork moderno de Firefox com workspaces e UI redesenhada | https://zen-browser.app/ |
| **Floorp** | ✅ Sim | Gecko | Firefox com foco em customização, mantido no Japão | https://floorp.app/ |

### 9.2 Mobile (Android)

| Navegador | Diferencial |
|---|---|
| **Tor Browser** | Anonimato máximo via rede Tor |
| **Brave** | Bloqueio nativo de anúncios e rastreadores |
| **Firefox Focus** | Apaga automaticamente o histórico ao sair, bloqueia rastreadores |
| **Bromite** | Chromium com bloqueio de anúncios e anti-fingerprinting (descontinuado → ver Cromite) |
| **Cromite** | Fork do Bromite, manutenção ativa |
| **Mull** | Firefox com configurações de privacidade reforçadas (via DivestOS) |
| **IronFox** | Sucessor do Mull (descontinuado), Firefox endurecido para Android | https://gitlab.com/ironfox-oss/IronFox |
| **Vanadium** | Navegador Chromium endurecido nativo do GrapheneOS |
| **DuckDuckGo Browser (mobile)** | App tudo-em-um com Fire Button e bloqueio de rastreadores |
| **Privacy Browser** | Foco em controle granular de cookies, JavaScript e DOM Storage | https://www.stoutner.com/privacy-browser/ |

### 9.3 Extensões Essenciais para Navegadores

| Extensão | Função | Navegadores |
|---|---|---|
| **uBlock Origin** | Bloqueador de anúncios e rastreadores (FOSS) | Firefox, Chrome, Edge |
| **NoScript** | Bloqueia JavaScript por padrão (whitelist) | Firefox |
| **Canvas Blocker** | Protege contra Canvas fingerprinting | Firefox |
| **HTTPS Everywhere** | Força HTTPS (integrado em muitos navegadores modernos) | Firefox, Chrome |
| **DuckDuckGo Privacy Essentials** | Bloqueio de rastreadores + nota de privacidade | Firefox, Chrome, Edge |
| **Privacy Badger (EFF)** | Bloqueio heurístico de rastreadores baseado em comportamento | Firefox, Chrome, Edge |
| **ClearURLs** | Remove parâmetros de tracking de URLs (utm_, fbclid, etc.) | Firefox, Chrome |
| **Decentraleyes** | Hospeda CDNs localmente para evitar conexões a Google/Cloudflare | Firefox, Chrome |
| **LocalCDN** | Sucessor mais ativo do Decentraleyes | Firefox, Chrome |
| **Cookie AutoDelete** | Apaga cookies ao fechar abas, exceções por domínio | Firefox, Chrome |
| **Multi-Account Containers** | Isola cookies por container (Firefox) | Firefox |
| **Temporary Containers** | Cria container descartável para cada aba | Firefox |
| **Skip Redirect** | Pula redirecionamentos intermediários de tracking | Firefox |
| **SponsorBlock** | Pula trechos patrocinados em vídeos do YouTube | Multi |
| **Snowflake (extensão)** | Transforma seu navegador em proxy para usuários Tor censurados | Firefox, Chrome |
| **JShelter** | Restringe APIs JavaScript usadas para fingerprinting | Firefox, Chrome |
| **CanvasBlocker** | Bloqueia/aleatoriza Canvas fingerprint | Firefox |
| **User-Agent Switcher** | Muda User-Agent para reduzir fingerprint único | Firefox, Chrome |
| **Bitwarden / KeePassXC-Browser** | Auto-fill seguro do gerenciador de senhas | Multi |

### 9.4 Ferramentas de Teste de Fingerprinting

| Ferramenta | Função | Link |
|---|---|---|
| **AmIUnique** | Mostra quão único é seu navegador | https://amiunique.org |
| **BrowserLeaks** | Teste detalhado de vazamentos (WebRTC, Canvas, WebGL, AudioContext) | https://browserleaks.com |
| **Cover Your Tracks (EFF)** | Teste de rastreabilidade do navegador | https://coveryourtracks.eff.org |
| **CreepJS** | Detecção avançada de fingerprinting e spoofing | https://abrahamjuliot.github.io/creepjs/ |
| **DeviceInfo** | Informações detalhadas sobre seu dispositivo/navegador | https://www.deviceinfo.me |

### 9.5 Ferramentas de Segurança Web Geral

| Ferramenta | Função | Link |
|---|---|---|
| **Qualys SSL Labs** | Testa configurações SSL/TLS de servidores | https://www.ssllabs.com/ssltest |
| **Mozilla Observatory** | Análise de segurança de websites | https://observatory.mozilla.org |
| **GoLogin** | Gerenciamento de múltiplos perfis de navegador (anti-fingerprinting) | https://gologin.com |
| **BrowserScan** | Scanner de segurança de navegador | https://browserscan.net |

---

## 10. MOTORES DE BUSCA SEGUROS

### [Camada 4 — Aplicação]

| Motor | Índice Próprio | Jurisdição | Diferencial | Link |
|---|---|---|---|---|
| **DuckDuckGo** | Parcial (usa Bing) | EUA | Mais popular, sem rastreamento, bangs (!g, !w). ⚠️ Exceção Microsoft (2022, mitigada). | https://duckduckgo.com/ |
| **Startpage** | Não (usa Google) | Holanda | Resultados do Google sem rastreamento, modo de visualização anônima | https://www.startpage.com/ |
| **Brave Search** | ✅ Sim | EUA | Índice independente, sem dependência de Google/Bing, Goggles (filtros personalizáveis) | https://search.brave.com |
| **SearXNG** | Meta-busca | Auto-hospedável | Open-source, descentralizado, combina resultados de múltiplos motores, sem rastreamento | https://docs.searxng.org/ |
| **Mojeek** | ✅ Sim | Reino Unido | Índice 100% próprio, sem rastreamento, crawlers independentes | https://www.mojeek.com/ |
| **Qwant** | Parcial (usa Bing) | França | Sediado na UE, conformidade GDPR, sem personalização | https://www.qwant.com/ |
| **MetaGer** | Meta-busca | Alemanha | Organização sem fins lucrativos, visualização anônima de resultados, GDPR | https://metager.org |
| **Swisscows** | Parcial (usa Bing) | Suíça | Filtro de conteúdo adulto, foco familiar, leis de privacidade suíças | https://swisscows.com |
| **Ecosia** | Não (usa Bing) | Alemanha | Planta árvores com receita de anúncios, política de privacidade razoável | https://www.ecosia.org |
| **Oscobo** | Não (usa Bing/Yahoo) | Reino Unido | Sem rastreamento, sem personalização | https://www.oscobo.com |
| **Disconnect Search** | Meta-busca | EUA | Redireciona consultas anonimizadas para Google/Bing/Yahoo | https://search.disconnect.me |
| **Kagi** | ✅ Sim | EUA | Pago, sem anúncios, lenses, IA opcional, bloqueio de domínios | https://kagi.com/ |
| **Whoogle Search** | Meta-busca | Auto-hospedado | Resultados Google sem JS, sem IP do usuário, FOSS | https://github.com/benbusby/whoogle-search |
| **You.com** | ✅ Sim | EUA | IA + busca, modo privado | https://you.com/ |
| **Presearch** | ✅ Sim | Canadá | Descentralizado, recompensa em token PRE | https://presearch.com/ |
| **YaCy** | Meta-busca P2P | Auto-hospedado | Motor descentralizado P2P, cada nó é um crawler | https://yacy.net/ |
| **4get** | Meta-busca | Auto-hospedado | Front-end leve para Google, Bing, etc., sem JS | https://4get.ca/ |
| **LibreY** | Meta-busca | Auto-hospedado | Fork ativo do antigo LibreX | https://github.com/Ahwxorg/LibreY |

---

## 30. FERRAMENTAS DE TESTE DE VAZAMENTO (LEAK TEST)

### [Transversal — Múltiplas Camadas]

| Ferramenta | Tipo | O que testa | Link |
|---|---|---|---|
| **DNS Leak Test** | Web | Vazamento de consultas DNS fora do túnel VPN | https://dnsleaktest.com/ |
| **IPLeak.net** | Web | Vazamento de IP, DNS, WebRTC, geolocalização, torrent IP | https://ipleak.net/ |
| **BrowserLeaks** | Web | WebRTC, Canvas, WebGL, AudioContext, fonts, etc. | https://browserleaks.com/ |
| **Mullvad Connection Check** | Web | IP, DNS, WebRTC, chave de conta Mullvad | https://mullvad.net/check |
| **AmIUnique** | Web | Fingerprint do navegador (quão único você é) | https://amiunique.org/ |
| **Cover Your Tracks (EFF)** | Web | Rastreabilidade do navegador, fingerprinting | https://coveryourtracks.eff.org/ |
| **CreepJS** | Web | Detecção avançada de fingerprinting e tentativas de spoofing | https://abrahamjuliot.github.io/creepjs/ |
| **Qualys SSL Labs** | Web | Configuração SSL/TLS de servidores | https://www.ssllabs.com/ssltest |
| **Mozilla Observatory** | Web | Segurança de headers HTTP de websites | https://observatory.mozilla.org/ |
| **Have I Been Pwned** | Web | Verificar se e-mail/senha foram vazados | https://haveibeenpwned.com/ |
| **';--have i been pwned (Passwords)** | Web | Verificar se uma senha específica apareceu em vazamentos | https://haveibeenpwned.com/Passwords |
| **DeHashed** | Web | Busca em bases de dados vazadas (e-mail, nome, IP, etc.) | https://dehashed.com/ |
| **Mozilla Monitor** | Web | Monitoramento contínuo de vazamentos para seu e-mail | https://monitor.mozilla.org/ |
| **GoLogin** | Desktop | Gerenciamento de múltiplos perfis de navegador (anti-fingerprinting) | https://gologin.com/ |
| **BrowserScan** | Web | Scanner de segurança e fingerprint do navegador | https://browserscan.net/ |
| **DeviceInfo** | Web | Informações detalhadas expostas pelo seu dispositivo/navegador | https://www.deviceinfo.me/ |
| **Panopticlick (legado)** | Web | Predecessor do Cover Your Tracks | https://panopticlick.eff.org/ |
| **WebRTC Leak Test** | Web | Teste isolado de vazamento WebRTC | https://www.expressvpn.com/webrtc-leak-test |
| **DoILeak** | Web | Teste consolidado IP/DNS/WebRTC | https://www.doileak.com/ |
| **Test-IPv6** | Web | Verifica conectividade e vazamentos IPv6 | https://test-ipv6.com/ |
| **What is My IP** | Web | Mostra IP público, DNS, headers | https://whatismyipaddress.com/ |
| **Email Header Analyzer (MXToolbox)** | Web | Analisa headers de e-mail (SPF/DKIM/DMARC) | https://mxtoolbox.com/EmailHeaders.aspx |
| **EmailRep** | Web/API | Reputação de endereços de e-mail | https://emailrep.io/ |
| **HardenedBSD/Kernel hardening checks** | CLI | Verificações de hardening de kernel | — |

---

## 48. BLOQUEADORES DE ANÚNCIOS E RASTREADORES (STANDALONE)

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Plataformas | Tipo | Diferencial | Link |
|---|---|---|---|---|---|
| **uBlock Origin** | ✅ Sim | Navegador | Extensão | Padrão-ouro, eficiente, modo medium/hard | https://ublockorigin.com/ |
| **uBlock Origin Lite** | ✅ Sim | Navegador (MV3) | Extensão | Versão Manifest V3 para Chrome | — |
| **AdGuard (Desktop/Mobile)** | Parcial | Multi | App/Sistema | Filtra em todo o sistema (não só no browser) | https://adguard.com/ |
| **AdGuard Home** | ✅ Sim | Servidor | DNS | Bloqueio em rede | https://adguard.com/adguard-home/ |
| **Pi-hole** | ✅ Sim | Servidor | DNS | Sinkhole DNS clássico | https://pi-hole.net/ |
| **Blokada** | ✅ Sim | Android, iOS | App | DNS local, planos pagos com cloud | https://blokada.org/ |
| **DNS66** | ✅ Sim | Android | App | Bloqueio via DNS local sem root (descontinuado oficial, ainda funcional) | F-Droid |
| **NetGuard + filtro** | ✅ Sim | Android | Firewall | Firewall + filtro DNS por app | https://netguard.me/ |
| **RethinkDNS** | ✅ Sim | Android | Firewall+DNS | All-in-one moderno | https://rethinkdns.com/ |
| **Brave Shields** | ✅ Sim | Browser | Embutido | Bloqueio nativo no Brave | https://brave.com/ |
| **uMatrix (legado)** | ✅ Sim | Browser | Extensão | Controle granular por origem (descontinuado) | — |

---

## 49. GERENCIADORES DE COOKIES E LIMPEZA DE NAVEGAÇÃO

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Plataformas | Tipo | Diferencial | Link |
|---|---|---|---|---|---|
| **Cookie AutoDelete** | ✅ Sim | Firefox/Chrome | Extensão | Apaga cookies ao fechar aba | https://github.com/Cookie-AutoDelete/Cookie-AutoDelete |
| **Multi-Account Containers** | ✅ Sim | Firefox | Extensão | Isola cookies por container | https://addons.mozilla.org/firefox/addon/multi-account-containers/ |
| **Temporary Containers** | ✅ Sim | Firefox | Extensão | Container descartável por aba | https://github.com/stoically/temporary-containers |
| **Facebook/Google Container** | ✅ Sim | Firefox | Extensão | Isola serviços específicos | — |
| **Forget Me Not** | ✅ Sim | Firefox | Extensão | Limpeza configurável por domínio | — |
| **Self-Destructing Cookies (legado)** | ✅ Sim | Firefox | Extensão | Pioneiro do Cookie AutoDelete | — |
| **BleachBit** | ✅ Sim | Multi | Desktop | Limpa caches, cookies, históricos do sistema | https://www.bleachbit.org/ |
| **PrivaZer** | ❌ Não | Windows | Desktop | Limpeza profunda Windows + sobrescrita | https://privazer.com/ |
| **Tron Script** | ✅ Sim | Windows | Script | Limpeza/manutenção massiva (avançado) | https://www.reddit.com/r/TronScript/ |
| **Stacer** | ✅ Sim | Linux | Desktop | Limpeza/monitoramento Linux | https://oguzhaninan.github.io/Stacer-Web/ |
| **Onyx** | ❌ Não | macOS | Desktop | Manutenção/limpeza macOS | https://www.titanium-software.fr/en/onyx.html |
| **Ferramenta Limpar Dados (Chrome/Firefox)** | — | Browser | Nativo | Cmd+Shift+Del / Ctrl+Shift+Del | — |

---

## 50. MAPAS, NAVEGAÇÃO E LOCALIZAÇÃO PRIVADOS

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Plataformas | Tipo | Diferencial | Link |
|---|---|---|---|---|---|
| **OpenStreetMap (OSM)** | ✅ Sim | Web | Base de mapas | Base livre usada por outras ferramentas | https://www.openstreetmap.org/ |
| **Organic Maps** | ✅ Sim | Android, iOS | Offline | Mapas e navegação OSM sem rastreio | https://organicmaps.app/ |
| **OsmAnd** | ✅ Sim | Android, iOS | Offline | Recursos avançados (rotas, trilhas) | https://osmand.net/ |
| **Magic Earth** | ❌ Não | Multi | App | Navegação amigável com tráfego, política de privacidade decente | https://www.magicearth.com/ |
| **HERE WeGo** | ❌ Não | Multi | App | Mapas offline, base europeia | https://wego.here.com/ |
| **GMaps WV / GMaps Lite** | ✅ Sim | Android | Wrapper | Wrapper privado de Google Maps | F-Droid |
| **Maps.me (legado)** | Parcial | Multi | Offline | Antecessor do Organic Maps | — |
| **Komoot** | ❌ Não | Multi | Trilhas | Trilhas/ciclismo, política razoável | https://www.komoot.com/ |
| **GPSLogger** | ✅ Sim | Android | Logger | Registro privado de trilhas (sem nuvem) | F-Droid |
| **PhonetTrack / OwnTracks** | ✅ Sim | Multi | Localização própria | Compartilhe sua localização via MQTT/HTTPS próprios | https://owntracks.org/ |
| **Traccar** | ✅ Sim | Servidor | Rastreamento | Servidor de rastreamento auto-hospedado | https://www.traccar.org/ |
| **Mozilla Location Service (MLS)** | ✅ Sim | Backend | Geo Wi-Fi | Geolocalização sem Google (descontinuado em 2024 — buscar alternativas) | — |
| **DejaVu (microG)** | ✅ Sim | Android | Geo offline | Backend de localização local | F-Droid |

---

