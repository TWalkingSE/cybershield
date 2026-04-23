# CYBERSHIELD — Base de Conhecimento: Ferramentas de Segurança Digital e Privacidade

> **Versão:** 4.0 | **Atualização:** Abril 2026
> **Fonte primária:** "Proteja-se Online: Dicas e Softwares Essenciais para Sua Segurança Digital" (TWalking, 1ª Edição, Janeiro 2025)
> **Fontes complementares:** PrivacyGuides.org, PrivacyTools.io, EFF, awesome-selfhosted, auditorias independentes, documentação oficial das ferramentas.

---

## 12. ALIASES DE E-MAIL

### [Camada 4 — Aplicação]

| Serviço | Open-Source | Plano Gratuito | Diferencial | Link |
|---|---|---|---|---|
| **SimpleLogin** | ✅ Sim | 10 aliases | Open-source, integrado ao Proton Mail, auto-hospedável | https://simplelogin.io/ |
| **addy.io** (ex-AnonAddy) | ✅ Sim | Ilimitado (subdomínio) | Open-source, auto-hospedável, aliases ilimitados no plano gratuito (com domínio compartilhado) | https://addy.io/ |
| **Firefox Relay** | ✅ Sim | 5 aliases | Integração com Firefox, da Mozilla | https://relay.firefox.com/ |
| **Apple Hide My Email** | ❌ Não | Com iCloud+ | Integrado ao ecossistema Apple, gera aliases aleatórios | — |
| **SpamGourmet** | ✅ Sim | Gratuito | Aliases auto-destrutivos (limita quantidade de e-mails recebidos), minimalista | https://www.spamgourmet.com/ |
| **DuckDuckGo Email Protection** | ❌ Não | Gratuito | Aliases @duck.com, remove rastreadores de e-mail antes de encaminhar | https://duckduckgo.com/email |
| **Erine.email** | ✅ Sim | Gratuito | Aliases descartáveis com base em desafios de prova | https://erine.email/ |
| **Forward Email** | ✅ Sim | Grat. + pago | Forwarding criptografado, auto-hospedado, suporta domínio próprio | https://forwardemail.net/ |
| **33mail** | ❌ Não | Gratuito | Subdomínio grátis, ilimitados aliases | https://33mail.com/ |
| **EmailOnDeck** | ❌ Não | Gratuito | E-mails temporários (10 minutos), sem cadastro | https://www.emailondeck.com/ |
| **Mail.tm** | ❌ Não | Gratuito | Mailbox temporária com API pública | https://mail.tm/ |
| **Guerrilla Mail** | ❌ Não | Gratuito | Mailbox descartável clássica (1h) | https://www.guerrillamail.com/ |

---

## 13. APLICATIVOS DE MENSAGERIA SEGURA

### [Camada 4 — Aplicação]

| App | Open-Source | E2EE | Registro | Diferencial | Link |
|---|---|---|---|---|---|
| **Signal** | ✅ Sim | ✅ Padrão | Número de telefone | Padrão-ouro de E2EE (protocolo Signal), metadados mínimos, sealed sender | https://signal.org/ |
| **SimpleX Chat** | ✅ Sim | ✅ Padrão | Sem identificador | SEM identificador de usuário (nem número, nem username), descentralizável, metadados mínimos | https://simplex.chat/ |
| **Session** | ✅ Sim | ✅ Padrão | Session ID (sem telefone) | Rede descentralizada (Oxen), onion routing, sem número de telefone | https://getsession.org/ |
| **Briar** | ✅ Sim | ✅ Padrão | Sem servidor central | P2P via Tor/Wi-Fi/Bluetooth, funciona sem internet, ideal para ativistas | https://briarproject.org/ |
| **Element (Matrix)** | ✅ Sim | ✅ (Megolm) | Conta Matrix | Protocolo federado (Matrix), auto-hospedável, rooms criptografadas | https://element.io/ |
| **Wire** | ✅ Sim | ✅ Padrão | E-mail ou telefone | E2EE por padrão, foco corporativo, Suíça. ⚠️ Armazena metadados (quem fala com quem). | https://wire.com/ |
| **Threema** | ✅ Sim (cliente) | ✅ Padrão | Threema ID (sem telefone) | Suíça, sem número de telefone obrigatório, pago (sem modelo de anúncios) | https://threema.ch/ |
| **Telegram** | Parcial (cliente) | ⚠️ Apenas Secret Chats | Número de telefone | Chats normais NÃO são E2EE. Secret Chats são E2EE mas não sincronizam entre dispositivos. ⚠️ Servidor proprietário. | https://telegram.org/ |
| **WhatsApp** | ❌ Não | ✅ (Signal protocol) | Número de telefone | E2EE em mensagens e chamadas, mas backups em iCloud/Drive nem sempre são E2EE; metadados extensos coletados pela Meta | https://whatsapp.com/ |
| **Molly** | ✅ Sim | ✅ Padrão | Número de telefone | Fork hardened do Signal para Android (cofre criptografado, bloqueio biométrico) | https://molly.im/ |
| **DeltaChat** | ✅ Sim | ✅ (Autocrypt) | E-mail | Mensageria sobre IMAP/SMTP com PGP automático (Autocrypt), usa qualquer provedor de e-mail | https://delta.chat/ |
| **Status** | ✅ Sim | ✅ Padrão | Chave Ethereum | Mensageria descentralizada, integração com carteira ETH, P2P via Whisper | https://status.app/ |
| **Berty** | ✅ Sim | ✅ Padrão | Sem identificador | Mensageria P2P sem servidores, BLE/Wi-Fi/Internet | https://berty.tech/ |
| **Jami** | ✅ Sim | ✅ Padrão | Sem servidor central | Mensageria/chamadas P2P (DHT OpenDHT), GNU project | https://jami.net/ |
| **Cwtch** | ✅ Sim | ✅ Padrão | Sem identificador | Mensageria metadata-resistant via Tor onion services | https://cwtch.im/ |
| **XMPP (Conversations, Gajim, Dino)** | ✅ Sim | ✅ (OMEMO) | JID | Protocolo federado XMPP com OMEMO E2EE | https://conversations.im/ |
| **Mattermost** | ✅ Sim | Parcial | Conta em servidor | Slack open-source, auto-hospedado, ideal para equipes | https://mattermost.com/ |
| **Rocket.Chat** | ✅ Sim | Parcial | Conta em servidor | Slack open-source, federação EE, auto-hospedado | https://www.rocket.chat/ |
| **Revolt** | ✅ Sim | ❌ | Conta | Alternativa FOSS ao Discord, em desenvolvimento | https://revolt.chat/ |

---

## 17. SEGURANÇA DE E-MAIL (PROVEDORES)

### [Camada 4 — Aplicação]

| Provedor | Open-Source | E2EE | Jurisdição | Diferencial | Link |
|---|---|---|---|---|---|
| **Proton Mail** | ✅ Sim | ✅ Nativo | Suíça | E2EE por padrão, zero-access encryption, calendario e drive integrados. ⚠️ Obrigado a registrar IP sob ordem judicial suíça (2021). | https://proton.me/mail |
| **Tuta** (ex-Tutanota) | ✅ Sim | ✅ Nativo | Alemanha | E2EE com protocolo próprio, calendário criptografado, plano gratuito | https://tuta.com/ |
| **Mailfence** | ❌ Não | ✅ (PGP) | Bélgica | PGP integrado, calendário, documentos, assinaturas digitais | https://mailfence.com/ |
| **Posteo** | ❌ Não | ✅ (PGP via Mailvelope) | Alemanha | Pagamento anônimo, energia renovável, €1/mês | https://posteo.de/ |
| **Mailbox.org** | Parcial | ✅ (PGP) | Alemanha | PGP server-side opcional, calendário, drive, €1-9/mês | https://mailbox.org/ |
| **StartMail** | ❌ Não | ✅ (PGP) | Holanda | Da Startpage, PGP integrado, aliases descartáveis | https://www.startmail.com/ |
| **CounterMail** | ❌ Não | ✅ Nativo | Suécia | OpenPGP forte, servidores diskless, jurisdição sueca | https://countermail.com/ |
| **Disroot** | ✅ Sim | ✅ (PGP) | Holanda | Coletivo sem fins lucrativos, ecossistema completo (mail, cloud, pad) | https://disroot.org/ |
| **Riseup** | ✅ Sim | ✅ | EUA (ativismo) | Provedor para ativistas, requer convite, sem logs | https://riseup.net/ |
| **Skiff Mail** | ⚠️ Descontinuado | ⚠️ Encerrado | EUA | ⚠️ ALERTA: Adquirido pela Notion em fevereiro 2024 e encerrado em abril 2024. Não use. Alternativa: Tuta ou Proton Mail. | https://skiff.com/ |
| **Soverin** | ❌ Não | ⚠️ | Holanda | Foco simplicidade + domínio próprio | https://soverin.net/ |
| **Runbox** | ❌ Não | ⚠️ (TLS) | Noruega | 100% energia renovável, jurisdição forte | https://runbox.com/ |
| **Kolab Now** | ✅ Sim | ⚠️ (TLS) | Suíça | Suite colaborativa (mail/cal/contacts/files) | https://kolabnow.com/ |

### 17.1 Servidores de E-mail Auto-Hospedados

| Ferramenta | Tipo | Diferencial |
|---|---|---|
| **Mailcow** | Stack Docker | Solução completa (Postfix, Dovecot, Rspamd, SoGo) |
| **Mail-in-a-Box** | Bundle | Setup automatizado em Ubuntu |
| **Mailu** | Stack Docker | Stack modular, antispam integrado |
| **Modoboa** | Suite Python | Painel administrativo amigável |
| **Stalwart Mail Server** | Tudo-em-um | Servidor Rust moderno (SMTP/IMAP/JMAP) com antispam embutido |
| **Maddy** | Tudo-em-um | Servidor SMTP+IMAP em Go, configuração simples |

---

## 23. NOTIFICAÇÕES PUSH E ALTERNATIVAS

### [Camada 4 — Aplicação]

| Ferramenta | Tipo | Diferencial |
|---|---|---|
| **UnifiedPush** | Protocolo | Alternativa descentralizada ao Google FCM/Apple APNs para push notifications |
| **ntfy** | Servidor de notificações | Open-source, auto-hospedável, sem Google/Apple |

> ⚠️ **RISCO:** Google FCM e Apple APNs podem ser usados para rastreamento. Governos já solicitaram dados de notificações push a Google e Apple.

---

## 25. TRANSFERÊNCIA SEGURA DE ARQUIVOS

### [Camada 4 — Aplicação / Camada 2 — Internet]

| Ferramenta | Open-Source | Plataformas | Tipo | Diferencial | Link |
|---|---|---|---|---|---|
| **OnionShare** | ✅ Sim | Windows, macOS, Linux | P2P via Tor | Compartilha arquivos via serviço onion temporário, sem servidor intermediário, anônimo | https://onionshare.org/ |
| **Magic Wormhole** | ✅ Sim | Windows, macOS, Linux | P2P/CLI | Transferência E2EE com código curto falado, PAKE (SPAKE2), sem upload para nuvem | https://magic-wormhole.readthedocs.io/ |
| **Croc** | ✅ Sim | Windows, macOS, Linux | P2P/CLI | Similar ao Magic Wormhole, escrito em Go, suporta múltiplos arquivos e retomada | https://github.com/schollz/croc |
| **Wormhole.app (Send)** | ✅ Sim | Web | Navegador | E2EE via navegador, até 10GB, link auto-expirante, baseado no Firefox Send descontinuado | https://wormhole.app/ |
| **LocalSend** | ✅ Sim | Windows, macOS, Linux, Android, iOS | Rede local | AirDrop open-source multiplataforma, sem internet, criptografia TLS | https://localsend.org/ |
| **PairDrop** | ✅ Sim | Web | Rede local/Web | Fork do Snapdrop, compartilhamento P2P via navegador na mesma rede | https://pairdrop.net/ |
| **Tresorit Send** | ❌ Não | Web | Nuvem E2EE | Compartilhamento E2EE com controle de acesso, até 5GB gratuito | https://send.tresorit.com/ |
| **Keybase Filesystem** | ✅ Sim | Windows, macOS, Linux | P2P/Nuvem | Sistema de arquivos criptografado com identidade verificável | https://keybase.io/ |
| **RetroShare** | ✅ Sim | Windows, macOS, Linux | P2P | Comunicação descentralizada P2P com compartilhamento de arquivos, OpenPGP | https://retroshare.cc/ |
| **Syncthing** | ✅ Sim | Windows, macOS, Linux, Android | P2P | Sincronização contínua entre dispositivos, E2EE, sem servidor central | https://syncthing.net/ |
| **KDE Connect** | ✅ Sim | Multi | Rede local | Compartilhamento, clipboard, controle remoto entre dispositivos | https://kdeconnect.kde.org/ |
| **Warpinator** | ✅ Sim | Linux, Android | Rede local | Clône open-source do Nitroshare/AirDrop, do Linux Mint | https://github.com/linuxmint/warpinator |
| **ShareDrop** | ✅ Sim | Web | Rede local | AirDrop via WebRTC entre dispositivos da mesma rede | https://www.sharedrop.io/ |
| **Send (Tuta)** | Parcial | Web | E2EE | Sucessor inspirado no Firefox Send, planos pagos | https://tuta.com/ |
| **Bitwarden Send** | ✅ Sim | Web/App | E2EE | Texto/arquivo E2EE com expiração, integrado ao Bitwarden | https://bitwarden.com/products/send/ |

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

## 28. CLIENTES DE E-MAIL SEGUROS

### [Camada 4 — Aplicação]

| Cliente | Open-Source | Plataformas | Diferencial | Link |
|---|---|---|---|---|
| **Thunderbird** | ✅ Sim | Windows, macOS, Linux | Cliente completo, suporte nativo a OpenPGP (desde v78), calendário integrado | https://www.thunderbird.net/ |
| **K-9 Mail → Thunderbird Mobile** | ✅ Sim | Android | Renomeado para Thunderbird Mobile, OpenPGP via OpenKeychain | https://k9mail.app/ |
| **FairEmail** | ✅ Sim | Android | Focado em privacidade, sem rastreamento, suporte PGP, design material | https://email.faircode.eu/ |
| **Canary Mail** | ❌ Não | macOS, iOS, Android, Windows | PGP integrado, SecureSend (E2EE para não-PGP), IA local | https://canarymail.io/ |
| **Apple Mail** | ❌ Não | macOS, iOS | S/MIME nativo, integrado ao ecossistema Apple | — |
| **Mailvelope** | ✅ Sim | Extensão (Chrome, Firefox, Edge) | Adiciona PGP a qualquer webmail (Gmail, Outlook, Yahoo) | https://mailvelope.com/ |
| **Claws Mail** | ✅ Sim | Multi | Cliente leve em GTK, suporte a PGP via plugins | https://www.claws-mail.org/ |
| **Evolution** | ✅ Sim | Linux | Cliente GNOME completo, S/MIME, PGP, calendar | https://wiki.gnome.org/Apps/Evolution |
| **Geary** | ✅ Sim | Linux | Cliente GNOME minimalista | https://wiki.gnome.org/Apps/Geary |
| **Mutt / NeoMutt** | ✅ Sim | Multi (CLI) | Cliente terminal clássico, altamente customizável | https://neomutt.org/ |
| **aerc** | ✅ Sim | Multi (CLI) | Cliente terminal moderno em Go | https://aerc-mail.org/ |
| **Betterbird** | ✅ Sim | Multi | Fork “melhorado” do Thunderbird | https://www.betterbird.eu/ |
| **Outlook** | ❌ Não | Multi | Suporta S/MIME e Microsoft Purview | — |

---

## 29. VIDEOCONFERÊNCIA E CHAMADAS SEGURAS

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | E2EE | Diferencial | Link |
|---|---|---|---|---|
| **Jitsi Meet** | ✅ Sim | ✅ (opcional) | Videoconferência sem conta, auto-hospedável, sem limite de participantes | https://meet.jit.si/ |
| **Signal (chamadas)** | ✅ Sim | ✅ Nativo | Chamadas de voz e vídeo E2EE, grupo até 40 pessoas | https://signal.org/ |
| **Element (Matrix)** | ✅ Sim | ✅ (Megolm) | Chamadas via protocolo Matrix, federado, auto-hospedável | https://element.io/ |
| **Wire** | ✅ Sim | ✅ Nativo | Chamadas E2EE, conferências, foco corporativo, Suíça | https://wire.com/ |
| **Brave Talk** | ❌ Não | ✅ (opcional) | Integrado ao Brave, baseado em Jitsi, chamadas gratuitas sem conta | https://talk.brave.com/ |
| **Mumble** | ✅ Sim | ✅ Sim | VoIP de baixa latência, criptografia forte, auto-hospedável, ideal para comunidades | https://www.mumble.info/ |
| **BigBlueButton** | ✅ Sim | Parcial | Plataforma de webconferência open-source, foco educacional, auto-hospedada | https://bigbluebutton.org/ |
| **Nextcloud Talk** | ✅ Sim | ✅ (1:1) | Chamadas integradas ao Nextcloud, auto-hospedado | https://nextcloud.com/talk/ |
| **Galene** | ✅ Sim | ⚠️ | SFU SFU leve em Go, auto-hospedado | https://galene.org/ |
| **Linphone** | ✅ Sim | ✅ (ZRTP) | Cliente SIP/VoIP com criptografia ZRTP | https://linphone.org/ |
| **Tox / qTox** | ✅ Sim | ✅ Padrão | Chamadas P2P E2EE sem servidores centrais | https://qtox.github.io/ |
| **Element Call** | ✅ Sim | ✅ (Megolm) | Chamadas em grupo nativas no Matrix | https://element.io/ |

---

