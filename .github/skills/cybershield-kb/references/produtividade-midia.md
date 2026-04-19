# CYBERSHIELD — Base de Conhecimento: Ferramentas de Segurança Digital e Privacidade

> **Versão:** 4.0 | **Atualização:** Abril 2026
> **Fonte primária:** "Proteja-se Online: Dicas e Softwares Essenciais para Sua Segurança Digital" (TWalking, 1ª Edição, Janeiro 2025)
> **Fontes complementares:** PrivacyGuides.org, PrivacyTools.io, EFF, awesome-selfhosted, auditorias independentes, documentação oficial das ferramentas.

---

## 14. GERENCIAMENTO DE METADADOS

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Plataformas | Tipo | Diferencial | Link |
|---|---|---|---|---|---|
| **ExifTool** | ✅ Sim | Windows, macOS, Linux | CLI | Padrão da indústria, lê/edita metadados de 400+ formatos de arquivo | https://exiftool.org/ |
| **mat2** | ✅ Sim | Linux | CLI | Remove metadados de imagens, documentos, áudio, vídeo | https://0xacab.org/jfrber/mat2 |
| **Scrambled Exif** | ✅ Sim | Android | App | Remove metadados de fotos antes de compartilhar | F-Droid |
| **Metapho** | ❌ Não | iOS | App | Visualiza e remove metadados de fotos no iPhone | App Store |
| **ImageOptim** | ✅ Sim | macOS | App | Otimiza imagens removendo metadados e comprimindo | https://imageoptim.com/ |
| **GIMP** | ✅ Sim | Windows, macOS, Linux | Editor | Editor de imagem completo, permite remover/editar metadados ao exportar | https://www.gimp.org/ |
| **MetaCleaner** | ❌ Não | Web | Web | Limpeza de metadados online (PDF, imagens, Office) | https://www.metacleaner.com/ |
| **PDF Metadata Editor** | ✅ Sim | Multi | Desktop | Edita metadados de PDFs em batch | https://broken-by.me/pdf-metadata-editor/ |
| **jhead** | ✅ Sim | Multi (CLI) | CLI | Visualiza/edita EXIF de JPEGs | https://www.sentex.ca/~mwandel/jhead/ |
| **MediaInfo** | ✅ Sim | Multi | Desktop/CLI | Análise técnica de vídeo/áudio (codecs, metadados) | https://mediaarea.net/MediaInfo |
| **mat2 web** | ✅ Sim | Web | Web | Versão web auto-hospedada do mat2 | https://0xacab.org/jvoisin/mat2-web |

---

## 15. FERRAMENTAS ANTI-PHISHING

### [Camada 4 — Aplicação]

| Ferramenta | Tipo | Diferencial | Link |
|---|---|---|---|
| **VirusTotal** | Scanner de URL/arquivo | Analisa URLs e arquivos contra 70+ engines antivírus | https://www.virustotal.com/ |
| **PhishTank** | Base de dados colaborativa | Comunidade que reporta e verifica sites de phishing | https://phishtank.org/ |
| **URLVoid** | Verificador de reputação | Analisa URLs contra 30+ fontes de blacklist | https://www.urlvoid.com/ |
| **dnstwist** | Detector de typosquatting | Identifica domínios similares usados para phishing | https://dnstwist.it/ |
| **Google Phishing Quiz** | Educacional | Treinamento interativo para reconhecer phishing | https://phishingquiz.withgoogle.com/ |
| **Phishing.org** | Educacional | Recursos e alertas sobre ataques de phishing | https://www.phishing.org/ |
| **LeilãoSeguro** | Verificação de comércio | Verificação de segurança de sites de leilão/e-commerce (Brasil) | https://www.leilaoseguro.org.br/ |

---

## 22. PRIVACIDADE DE FOTOS E ARMAZENAMENTO

### [Camada 4 — Aplicação]

| Serviço | Open-Source | E2EE | Diferencial | Link |
|---|---|---|---|---|
| **Ente Photos** | ✅ Sim | ✅ Nativo | Alternativa ao Google Photos com E2EE, auto-hospedável | https://ente.io/ |
| **Stingle Photos** | ✅ Sim | ✅ Nativo | Backup E2EE de fotos e vídeos | https://stingle.org/ |
| **Cryptee** | ✅ Sim | ✅ Nativo | Documentos + fotos criptografados, Estônia | https://crypt.ee/ |
| **Immich** | ✅ Sim | Parcial (E2EE em desenvolvimento) | Auto-hospedado, ML local (faces/objetos), substituto direto do Google Photos | https://immich.app/ |
| **PhotoPrism** | ✅ Sim | ⚠️ (em disco) | Auto-hospedado, IA local de classificação, Go | https://photoprism.app/ |
| **LibrePhotos** | ✅ Sim | ⚠️ | Auto-hospedado, reconhecimento facial, mapas | https://github.com/LibrePhotos/librephotos |
| **Piwigo** | ✅ Sim | ⚠️ | Galeria web clássica, organização flexível | https://piwigo.org/ |
| **Lychee** | ✅ Sim | ⚠️ | Galeria minimalista PHP | https://lycheeorg.github.io/ |

---

## 26. NOTAS E DOCUMENTOS CRIPTOGRAFADOS

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | E2EE | Plataformas | Diferencial | Link |
|---|---|---|---|---|---|
| **Standard Notes** | ✅ Sim | ✅ Nativo | Windows, macOS, Linux, Android, iOS, Web | Notas E2EE, extensível com editores, 100% criptografado | https://standardnotes.com/ |
| **Joplin** | ✅ Sim | ✅ (com sync E2EE) | Windows, macOS, Linux, Android, iOS | Alternativa ao Evernote, Markdown, sync com Nextcloud/OneDrive/Dropbox | https://joplinapp.org/ |
| **Notesnook** | ✅ Sim | ✅ Nativo | Windows, macOS, Linux, Android, iOS, Web | Notas E2EE com editor rico, zero-knowledge, plano gratuito generoso | https://notesnook.com/ |
| **Obsidian** | ❌ Não | ⚠️ (com Sync pago) | Windows, macOS, Linux, Android, iOS | Vault local em Markdown, graph view, plugins extensivos. Dados locais por padrão. | https://obsidian.md/ |
| **Logseq** | ✅ Sim | ⚠️ (local) | Windows, macOS, Linux, Android, iOS | Outliner + graph, dados locais, sync via Git ou Logseq Sync | https://logseq.com/ |
| **Cryptee** | ✅ Sim | ✅ Nativo | Web | Documentos + fotos criptografados, Estônia | https://crypt.ee/ |
| **CryptPad** | ✅ Sim | ✅ Nativo | Web | Documentos colaborativos E2EE (docs, planilhas, kanban, formulários), auto-hospedável | https://cryptpad.org/ |
| **Trilium Notes** | ✅ Sim | ⚠️ (local/auto-hospedado) | Windows, macOS, Linux, Web | Base de conhecimento hierárquica, auto-hospedável, relações entre notas | https://github.com/zadam/trilium |
| **AnyType** | ✅ Sim | Multi | E2EE local-first com sync P2P | https://anytype.io/ |
| **SilverBullet** | ✅ Sim | Web | Notas Markdown extensível, auto-hospedado | https://silverbullet.md/ |
| **AppFlowy** | ✅ Sim | Multi | Alternativa FOSS ao Notion | https://appflowy.io/ |
| **Affine** | ✅ Sim | Multi | Alternativa moderna a Notion/Miro com edição local | https://affine.pro/ |
| **Memos** | ✅ Sim | Web/Mobile | Microblog/notas auto-hospedado | https://www.usememos.com/ |
| **Outline** | ✅ Sim | Web | Wiki para times auto-hospedado | https://www.getoutline.com/ |
| **BookStack** | ✅ Sim | Web | Wiki/documentação organizada em livros/capítulos | https://www.bookstackapp.com/ |
| **HedgeDoc** | ✅ Sim | Web | Markdown colaborativo em tempo real | https://hedgedoc.org/ |
| **Etherpad** | ✅ Sim | Web | Editor colaborativo clássico | https://etherpad.org/ |

---

## 27. PASTEBINS CRIPTOGRAFADOS

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Diferencial | Link |
|---|---|---|---|
| **PrivateBin** | ✅ Sim | Pastebin minimalista E2EE, auto-hospedável, zero-knowledge, auto-destruição | https://privatebin.info/ |
| **0bin** | ✅ Sim | Pastebin criptografado client-side, chave na URL (nunca enviada ao servidor) | https://0bin.net/ |
| **Defuse.ca** | ✅ Sim | Pastebin criptografado por pesquisador de segurança, burn-after-reading | https://defuse.ca/pastebin.htm |
| **TheSecureNote** | ❌ Não | AES-256-GCM, auto-destruição, compartilhamento via QR | https://thesecurenote.com/ |

---

## 36. CALENDÁRIOS E CONTATOS SEGUROS

### [Camada 4 — Aplicação]

| Serviço | Open-Source | E2EE | Diferencial | Link |
|---|---|---|---|---|
| **Proton Calendar** | ✅ Sim | ✅ Nativo | Calendário E2EE integrado ao ecossistema Proton, Suíça | https://proton.me/calendar |
| **Tuta Calendar** | ✅ Sim | ✅ Nativo | Calendário criptografado integrado ao Tuta Mail | https://tuta.com/ |
| **EteSync** | ✅ Sim | ✅ Nativo | Sync E2EE de calendário, contatos e tarefas, auto-hospedável | https://www.etesync.com/ |
| **Nextcloud Calendar/Contacts** | ✅ Sim | ⚠️ (em disco) | CalDAV/CardDAV auto-hospedável, integrado ao Nextcloud | https://nextcloud.com/ |
| **Radicale** | ✅ Sim | ⚠️ (em disco) | Servidor CalDAV/CardDAV leve e simples, auto-hospedável | https://radicale.org/ |
| **DAVx⁵** | ✅ Sim | — (cliente) | App Android para sync CalDAV/CardDAV com qualquer servidor | https://www.davx5.com/ |
| **Baikal** | ✅ Sim | ⚠️ | Servidor leve CalDAV/CardDAV em PHP | https://sabre.io/baikal/ |
| **Mailfence Calendar** | ❌ Não | ⚠️ | Calendário integrado ao Mailfence | https://mailfence.com/ |
| **Murena Cloud (incl. cal)** | ✅ Sim | ⚠️ | Suite tipo Google integrada ao /e/OS | https://murena.com/ |
| **Disroot Calendar** | ✅ Sim | ⚠️ | CalDAV via Nextcloud do coletivo Disroot | https://disroot.org/ |

---

## 39. OFFICE SUITES E COLABORAÇÃO PRIVADA

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Plataformas | Diferencial | Link |
|---|---|---|---|---|
| **LibreOffice** | ✅ Sim | Multi | Suite office completa, sem telemetria, padrão ODF | https://www.libreoffice.org/ |
| **OnlyOffice Docs** | ✅ Sim | Multi + Web | Edição colaborativa, alta compatibilidade com OOXML, auto-hospedado | https://www.onlyoffice.com/ |
| **Collabora Online** | ✅ Sim | Web | LibreOffice em browser, integra com Nextcloud | https://www.collaboraonline.com/ |
| **CryptPad** | ✅ Sim | Web | Suite colaborativa E2EE (docs, planilhas, kanban, formulários) | https://cryptpad.org/ |
| **EtherCalc** | ✅ Sim | Web | Planilha colaborativa em tempo real | https://ethercalc.net/ |
| **HedgeDoc** | ✅ Sim | Web | Notas Markdown colaborativas | https://hedgedoc.org/ |
| **Nextcloud Office** | ✅ Sim | Web | Edição colaborativa via Collabora ou OnlyOffice | https://nextcloud.com/ |
| **Apache OpenOffice** | ✅ Sim | Multi | Antecessor do LibreOffice (manutenção lenta) | https://www.openoffice.org/ |
| **Calligra Suite** | ✅ Sim | Multi | Suite KDE com Words, Sheets, Stage | https://calligra.org/ |
| **WPS Office** | ❌ Não | Multi | Compatibilidade Office. ⚠️ Telemetria, base na China | https://www.wps.com/ |
| **AbiWord** | ✅ Sim | Multi | Processador de texto leve | https://www.abisource.com/ |
| **Gnumeric** | ✅ Sim | Linux | Planilha leve e precisa | http://www.gnumeric.org/ |

---

## 40. EDITORES E FERRAMENTAS DE PDF SEGURAS

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Plataformas | Diferencial | Link |
|---|---|---|---|---|
| **PDF Arranger** | ✅ Sim | Multi | Reorganiza/extrai/divide páginas (GUI sobre pikepdf) | https://github.com/pdfarranger/pdfarranger |
| **Stirling-PDF** | ✅ Sim | Web (auto-hospedado) | Suite PDF completa local (split, merge, OCR, redact) | https://github.com/Stirling-Tools/Stirling-PDF |
| **PDF.js** | ✅ Sim | Web | Renderizador PDF do Mozilla, sem plugins externos | https://mozilla.github.io/pdf.js/ |
| **qpdf** | ✅ Sim | CLI | Manipulação avançada de PDF, criptografia, lineariza | https://qpdf.sourceforge.io/ |
| **pdftk** | ✅ Sim | CLI | Toolkit clássico para PDF | — |
| **Sumatra PDF** | ✅ Sim | Windows | Leitor PDF leve sem telemetria | https://www.sumatrapdfreader.org/ |
| **Okular** | ✅ Sim | Multi | Leitor KDE, suporte a anotações, sem telemetria | https://okular.kde.org/ |
| **Xournal++** | ✅ Sim | Multi | Anotações e assinatura em PDFs | https://xournalpp.github.io/ |
| **PDF Redact Tools** | ✅ Sim | CLI | Redação segura de PDFs (Freedom of the Press) | https://github.com/firstlookmedia/pdf-redact-tools |
| **Redacter** | ✅ Sim | CLI | Redação automatizada via OCR | — |
| **ExifTool (PDF)** | ✅ Sim | CLI | Remove metadados de PDFs | https://exiftool.org/ |
| **Adobe Acrobat (Redact)** | ❌ Não | Windows, macOS | Redação verificada em padrão DoD; ⚠️ telemetria | https://www.adobe.com/ |
| **Foxit Reader** | ❌ Não | Multi | Alternativa ao Adobe; ⚠️ telemetria/anúncios | https://www.foxit.com/ |
| **PDFsam Basic** | ✅ Sim | Multi | Split, merge, rotate de PDFs | https://pdfsam.org/ |
| **PrivacyByDefault Redactor** | — | Web | Use offline. ⚠️ Cuidado com PDFs sensíveis em web tools |

---

## 41. TRADUTORES E FERRAMENTAS LINGUÍSTICAS PRIVADAS

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Tipo | Diferencial | Link |
|---|---|---|---|---|
| **LibreTranslate** | ✅ Sim | Web/API | Tradução open-source auto-hospedável | https://libretranslate.com/ |
| **Argos Translate** | ✅ Sim | Local | Tradução offline desktop/CLI baseada em modelos OpenNMT | https://www.argosopentech.com/ |
| **Bergamot Translate** | ✅ Sim | Local | Tradução in-browser do Mozilla (Firefox Translate) | https://browser.mt/ |
| **Mozilla Translate (Firefox)** | ✅ Sim | Browser | Tradução local nativa no Firefox | — |
| **DeepL** | ❌ Não | Web/Desktop | Alta qualidade. ⚠️ Texto enviado ao servidor | https://www.deepl.com/ |
| **NLLB-200** | ✅ Sim | Modelo | Modelo Meta open-source para 200 idiomas (uso local) | — |
| **OpenNMT** | ✅ Sim | Framework | Treinamento de modelos próprios | https://opennmt.net/ |
| **LanguageTool** | ✅ Sim | Multi | Corretor gramatical auto-hospedável | https://languagetool.org/ |
| **Vosk** | ✅ Sim | Local | Reconhecimento de fala offline para 20+ idiomas | https://alphacephei.com/vosk/ |

---

## 42. MÍDIA: STREAMING, VÍDEO E MÚSICA PRIVADOS

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Tipo | Diferencial | Link |
|---|---|---|---|---|
| **Jellyfin** | ✅ Sim | Servidor de mídia | Substituto FOSS ao Plex/Emby, sem rastreio | https://jellyfin.org/ |
| **Kodi** | ✅ Sim | Player | Centro de mídia clássico | https://kodi.tv/ |
| **Plex** | ❌ Não | Servidor | Popular. ⚠️ Telemetria e exigência de conta | — |
| **Emby** | Parcial | Servidor | Antecessor do Jellyfin (closed após v3.6) | — |
| **Funkwhale** | ✅ Sim | Streaming música | Fediverso, federado | https://funkwhale.audio/ |
| **Navidrome** | ✅ Sim | Streaming música | Servidor leve compatível com Subsonic | https://www.navidrome.org/ |
| **Airsonic-Advanced / Gonic** | ✅ Sim | Streaming música | Forks ativos do Subsonic | https://github.com/airsonic-advanced |
| **Mopidy** | ✅ Sim | Streaming música | Player extensível com plugins | https://mopidy.com/ |
| **Music Assistant** | ✅ Sim | Player/HA | Integração com Home Assistant | https://www.music-assistant.io/ |
| **mpv** | ✅ Sim | Player vídeo | Player minimalista poderoso | https://mpv.io/ |
| **VLC** | ✅ Sim | Player vídeo | Player universal, sem telemetria | https://www.videolan.org/ |
| **Audacious / Strawberry / Clementine** | ✅ Sim | Player áudio | Players desktop FOSS | — |
| **NewPipe / LibreTube / Piped / Invidious** | ✅ Sim | Frontend YouTube | Acesso ao YouTube sem rastreio Google | — |
| **FreeTube** | ✅ Sim | Frontend YouTube desktop | Cliente desktop com sponsorblock | https://freetubeapp.io/ |
| **yt-dlp** | ✅ Sim | CLI | Download de mídia de centenas de sites | https://github.com/yt-dlp/yt-dlp |
| **Tubular** | ✅ Sim | Android | Fork do NewPipe com SponsorBlock e ReturnYoutubeDislike | F-Droid |

---

## 43. REDES SOCIAIS E MICROBLOGGING ALTERNATIVOS

### [Camada 4 — Aplicação]

| Plataforma | Open-Source | Tipo | Diferencial | Link |
|---|---|---|---|---|
| **Mastodon** | ✅ Sim | Microblog federado | Maior rede do Fediverso, ActivityPub | https://joinmastodon.org/ |
| **Pleroma / Akkoma** | ✅ Sim | Microblog federado | Servidores leves alternativos a Mastodon | https://akkoma.social/ |
| **Misskey / Sharkey / Firefish** | ✅ Sim | Microblog federado | Forks com recursos extras (reactions, drive) | https://misskey-hub.net/ |
| **GoToSocial** | ✅ Sim | Microblog federado | Servidor leve em Go para single-user | https://gotosocial.org/ |
| **Lemmy** | ✅ Sim | Agregador (Reddit-like) | Comunidades federadas via ActivityPub | https://join-lemmy.org/ |
| **Kbin / Mbin** | ✅ Sim | Agregador federado | Mistura Reddit + microblog | https://kbin.pub/ |
| **Friendica** | ✅ Sim | Rede social federada | Estilo Facebook, conecta-se a múltiplos protocolos | https://friendi.ca/ |
| **Diaspora\*** | ✅ Sim | Rede social federada | Pioneiro federado, pods independentes | https://diasporafoundation.org/ |
| **Bluesky / AT Proto** | ✅ Sim | Microblog | Rede com protocolo AT, federação em desenvolvimento | https://bsky.app/ |
| **Nostr (Damus, Amethyst, etc.)** | ✅ Sim | Protocolo P2P | Notas e relays simples, identidade por chave | https://nostr.com/ |
| **Hubzilla** | ✅ Sim | Rede social/CMS | Identidade nômade entre servidores | https://hubzilla.org/ |
| **Movim** | ✅ Sim | Rede social XMPP | Microblog sobre XMPP | https://movim.eu/ |

---

## 44. PLATAFORMAS DE VÍDEO ALTERNATIVAS

### [Camada 4 — Aplicação]

| Plataforma | Open-Source | Tipo | Diferencial | Link |
|---|---|---|---|---|
| **PeerTube** | ✅ Sim | Federado P2P | Alternativa federada ao YouTube com WebTorrent | https://joinpeertube.org/ |
| **Odysee / LBRY** | Parcial | Blockchain | Vídeos descentralizados via LBRY | https://odysee.com/ |
| **Tilvids** | ✅ Sim | Instância PeerTube | Curadoria de canais | https://tilvids.com/ |
| **Invidious** | ✅ Sim | Frontend YouTube | Proxy web sem JS/cookies do Google | https://invidious.io/ |
| **Piped** | ✅ Sim | Frontend YouTube | Frontend moderno para YouTube | https://piped.video/ |
| **Hyperpipe** | ✅ Sim | Frontend YT Music | Cliente YouTube Music sem rastreio | https://hyperpipe.surge.sh/ |
| **NewPipe / LibreTube** | ✅ Sim | Android | Clientes Android sem Google | — |
| **Owncast** | ✅ Sim | Live streaming | Servidor próprio para streaming ao vivo | https://owncast.online/ |
| **DTube** | ✅ Sim | Blockchain | Vídeos via Hive blockchain + IPFS | https://d.tube/ |

---

## 45. HOSPEDAGEM DE CÓDIGO E COLABORAÇÃO

### [Camada 4 — Aplicação]

| Plataforma | Open-Source | Tipo | Diferencial | Link |
|---|---|---|---|---|
| **Codeberg** | ✅ Sim | Hosting Git | Forge sem fins lucrativos, baseado em Forgejo | https://codeberg.org/ |
| **Forgejo** | ✅ Sim | Auto-hospedado | Fork comunitário do Gitea | https://forgejo.org/ |
| **Gitea** | ✅ Sim | Auto-hospedado | Forge leve em Go | https://gitea.io/ |
| **GitLab CE** | ✅ Sim | Auto-hospedado | DevOps completo, CI/CD integrado | https://about.gitlab.com/ |
| **SourceHut** | ✅ Sim | Hosting/Auto | Foco em correio + listas + builds | https://sourcehut.org/ |
| **Gogs** | ✅ Sim | Auto-hospedado | Antecessor leve do Gitea | https://gogs.io/ |
| **Disroot Git (Forgejo)** | ✅ Sim | Hosting | Coletivo Disroot | https://git.disroot.org/ |
| **Tildegit / Notabug** | ✅ Sim | Hosting | Comunidades alternativas | — |
| **Radicle** | ✅ Sim | P2P | Forge P2P descentralizada com identidade criptográfica | https://radicle.xyz/ |
| **Fossil SCM** | ✅ Sim | SCM/forge | SCM + wiki + tickets em um único binário | https://fossil-scm.org/ |

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

## 51. APPS DE SAÚDE, FITNESS E PERÍODO PRIVADOS

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Plataformas | Tipo | Diferencial | Link |
|---|---|---|---|---|---|
| **Drip** | ✅ Sim | Android, iOS | Ciclo menstrual | Dados 100% locais, sem nuvem (importante pós-Roe v Wade) | https://dripapp.org/ |
| **Periodical** | ✅ Sim | Android | Ciclo menstrual | Local, simples, sem rastreio | F-Droid |
| **Euki** | ✅ Sim | Android, iOS | Saúde reprodutiva | Local, multilíngue | https://eukiapp.com/ |
| **OpenScale** | ✅ Sim | Android | Balança/peso | Funciona offline, suporta balanças BLE | F-Droid |
| **OpenTracks** | ✅ Sim | Android | Atividade | Registro de atividades sem nuvem | F-Droid |
| **FitoTrack** | ✅ Sim | Android | Atividade | Registro local de exercícios | F-Droid |
| **Forrunners** | ✅ Sim | Multi | Corrida | Ferramenta para Garmin sem cloud | — |
| **Gadgetbridge** | ✅ Sim | Android | Wearables | Cliente para wearables (Mi Band, Pebble, Amazfit, etc.) sem app proprietário | https://gadgetbridge.org/ |
| **Loop Habit Tracker** | ✅ Sim | Android | Hábitos | Tracker local de hábitos | F-Droid |
| **Daylio (alternativa FOSS: Mood Diary)** | Parcial | Multi | Humor | Diário de humor local | — |
| **AntennaPod** | ✅ Sim | Android | Podcasts | Sem rastreio | https://antennapod.org/ |
| **OpenFoodFacts** | ✅ Sim | Multi | Alimentos | Base aberta de produtos alimentares | https://world.openfoodfacts.org/ |

---

## 52. LEITORES DE FEED (RSS) E READ-IT-LATER

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Plataformas | Tipo | Diferencial | Link |
|---|---|---|---|---|---|
| **FreshRSS** | ✅ Sim | Auto-hospedado | Servidor RSS | Leve, multi-usuário, API Fever/GReader | https://freshrss.org/ |
| **Tiny Tiny RSS** | ✅ Sim | Auto-hospedado | Servidor RSS | Clássico veterano | https://tt-rss.org/ |
| **Miniflux** | ✅ Sim | Auto-hospedado | Servidor RSS | Minimalista em Go | https://miniflux.app/ |
| **Newsboat** | ✅ Sim | CLI | Cliente RSS | Cliente terminal rápido | https://newsboat.org/ |
| **NetNewsWire** | ✅ Sim | macOS, iOS | Cliente | Cliente nativo Apple | https://netnewswire.com/ |
| **Feeder** | ✅ Sim | Android | Cliente | Cliente offline-first | F-Droid |
| **Read You** | ✅ Sim | Android | Cliente | Material You moderno | F-Droid |
| **RSS Guard** | ✅ Sim | Multi | Cliente | Suporte a APIs (TT-RSS, Nextcloud News) | https://github.com/martinrotter/rssguard |
| **QuiteRSS / Liferea** | ✅ Sim | Multi | Cliente | Clientes desktop clássicos | — |
| **Wallabag** | ✅ Sim | Auto-hospedado | Read-it-later | Alternativa FOSS ao Pocket | https://www.wallabag.org/ |
| **Omnivore** | ✅ Sim | Multi | Read-it-later | Open-source, anotações | https://omnivore.app/ |
| **Karakeep (ex-Hoarder)** | ✅ Sim | Auto-hospedado | Bookmarks | Salvar links com IA local | https://karakeep.app/ |
| **Linkding** | ✅ Sim | Auto-hospedado | Bookmarks | Bookmark manager simples | https://github.com/sissbruecker/linkding |
| **Shaarli** | ✅ Sim | Auto-hospedado | Bookmarks | Bookmark manager clássico em PHP | https://github.com/shaarli/Shaarli |

---

## 57. HONEYPOTS E DETECÇÃO DE INTRUSÃO PESSOAL

### [Camada 1/3/4]

| Ferramenta | Open-Source | Tipo | Diferencial | Link |
|---|---|---|---|---|
| **Canarytokens** | ✅ Sim | Tokens | Tokens (URL, doc Office, AWS, etc.) que avisam quando acessados | https://canarytokens.org/ |
| **OpenCanary** | ✅ Sim | Honeypot | Versão FOSS dos Canary Tools | https://github.com/thinkst/opencanary |
| **T-Pot** | ✅ Sim | Bundle | Multi-honeypot da Telekom Security | https://github.com/telekom-security/tpotce |
| **Cowrie** | ✅ Sim | SSH/Telnet | Honeypot SSH/Telnet para capturar atacantes | https://github.com/cowrie/cowrie |
| **Dionaea** | ✅ Sim | Multi-protocolo | Honeypot para coletar malware | https://github.com/DinoTools/dionaea |
| **Honeyd** | ✅ Sim | Network | Honeypot virtual de rede clássico | https://www.honeyd.org/ |
| **Glastopf** | ✅ Sim | Web | Honeypot web (legado) | — |
| **HonSSH / Kippo** | ✅ Sim | SSH | Honeypots SSH | — |
| **Suricata + ELK** | ✅ Sim | IDS/Stack | IDS com visualização Elastic | https://suricata.io/ |
| **Wazuh** | ✅ Sim | XDR/SIEM | EDR/HIDS open-source | https://wazuh.com/ |
| **Security Onion** | ✅ Sim | Distro NSM | Distro Linux para NSM/SIEM | https://securityonionsolutions.com/ |
| **OSSEC** | ✅ Sim | HIDS | HIDS clássico | https://www.ossec.net/ |
| **CrowdSec** | ✅ Sim | Colaborativo | Detecção colaborativa de IPs maliciosos | https://www.crowdsec.net/ |
| **Fail2ban** | ✅ Sim | Bloqueio | Bane IPs após tentativas falhas em logs | https://www.fail2ban.org/ |

---

