# CYBERSHIELD — Base de Conhecimento: Ferramentas de Segurança Digital e Privacidade

> **Versão:** 4.0 | **Atualização:** Abril 2026
> **Fonte primária:** "Proteja-se Online: Dicas e Softwares Essenciais para Sua Segurança Digital" (TWalking, 1ª Edição, Janeiro 2025)
> **Fontes complementares:** PrivacyGuides.org, PrivacyTools.io, EFF, awesome-selfhosted, auditorias independentes, documentação oficial das ferramentas.

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

## 18. CRIPTOATIVOS E CARTEIRAS SEGURAS

### [Camada 4 — Aplicação]

### 18.1 Hardware Wallets

| Carteira | Tipo | Diferencial |
|---|---|---|
| **Ledger** (Nano S Plus, Nano X, Stax) | Hardware | Chip seguro (CC EAL5+), suporte a 5.500+ criptoativos |
| **Trezor** (Model One, Model T, Safe 3) | Hardware | Open-source, sem chip seguro proprietário, interface web |
| **Coldcard Mk4** | Hardware | Bitcoin-only, air-gapped via SD/QR, código aberto |
| **BitBox02** | Hardware | Suíça, versões Bitcoin-only e Multi |
| **KeepKey** | Hardware | Open-source, tela grande |
| **Foundation Passport** | Hardware | Bitcoin-only air-gapped, foco em verificação |
| **Jade (Blockstream)** | Hardware | Acessível, integração com Green Wallet |

### 18.2 Software Wallets

| Carteira | Open-Source | Plataformas | Diferencial |
|---|---|---|---|
| **Sparrow Wallet** | ✅ Sim | Windows, macOS, Linux | Bitcoin-only, foco em privacidade, suporte a CoinJoin |
| **Electrum** | ✅ Sim | Windows, macOS, Linux, Android | Bitcoin-only, leve, suporte a hardware wallets |
| **Wasabi Wallet** | ✅ Sim | Windows, macOS, Linux | Bitcoin com CoinJoin nativo (WabiSabi) |
| **Samourai Wallet** | ✅ Sim | Android | Bitcoin com Whirlpool CoinJoin, Stonewall, Stowaway |
| **BlueWallet** | ✅ Sim | Android, iOS, Desktop | Bitcoin + Lightning, multi-carteira |
| **Zeus LN** | ✅ Sim | Android, iOS | Cliente para nó Lightning próprio |
| **Phoenix Wallet** | ✅ Sim | Android, iOS | Lightning self-custodial, abertura automática de canais |
| **Cake Wallet** | ✅ Sim | Multi | Monero/Bitcoin/etc., nó próprio configurável |
| **Monero GUI** | ✅ Sim | Multi | Carteira oficial Monero |
| **Feather Wallet** | ✅ Sim | Multi | Carteira leve Monero, suporte a Tor |
| **MyMonero** | ✅ Sim | Multi | Carteira Monero leve (⚠️ remote node) |

### 18.3 Moedas com Foco em Privacidade

| Moeda | Diferencial |
|---|---|
| **Monero (XMR)** | Transações privadas por padrão (ring signatures, stealth addresses, RingCT) |
| **Zcash (ZEC)** | Transações blindadas opcionais (zk-SNARKs) |
| **Firo (XZC)** | Lelantus Spark, anonimato sem trusted setup |
| **Pirate Chain (ARRR)** | Fork do Zcash com transações blindadas obrigatórias |
| **Dash** | PrivateSend (CoinJoin opcional) |
| **DeroHE** | Smart contracts privados via TLS-like + Stargate |

---

## 19. FERRAMENTAS OSINT / SOCK PUPPET

### [Camada 4 — Aplicação]

### 19.1 Geradores de Identidade Fictícia (para investigação/OSINT)

| Ferramenta | Tipo | Link |
|---|---|---|
| **4Devs** | Gerador de CPF, CNPJ, dados ficcionais (BR) | https://www.4devs.com.br/ |
| **Fake Name Generator** | Perfis completos fictícios | https://www.fakenamegenerator.com/ |
| **DataFakeGenerator** | Dados fictícios variados | http://www.datafakegenerator.com/ |
| **Randus** | Perfis aleatórios | https://randus.org/ |
| **FauxID** | Identidades fictícias | https://fauxid.com/ |
| **NameFake** | Nomes e dados fictícios | https://namefake.com/ |
| **FakeInfo** | Informações fictícias | https://fakeinfo.net/ |
| **UK-OSINT** | Guia para criação de identidades (investigação) | https://www.uk-osint.net/creatingids.html |

### 19.2 Geradores de Imagens (Faces Fictícias)

| Ferramenta | Link |
|---|---|
| **ThisPersonDoesNotExist** | https://thispersondoesnotexist.com/ |
| **WhichFaceIsReal** | https://www.whichfaceisreal.com/ |
| **Generated Photos** | https://generated.photos/ |

### 19.3 Números Temporários

| Serviço | Link |
|---|---|
| **TextNow** | https://www.textnow.com/ |
| **Hushed** | https://hushed.com |
| **BurnerApp** | https://www.burnerapp.com |
| **Blacktel** | https://blacktel.io |
| **OnlineSim** | https://onlinesim.io/ |
| **Fragment** (Telegram) | https://fragment.com/numbers |

### 19.4 Verificação de Exposição (OSINT Defensivo)

| Ferramenta | Tipo | Link |
|---|---|---|
| **Have I Been Pwned** | Verificar se seu e-mail/senha foram vazados | https://haveibeenpwned.com/ |
| **DeHashed** | Busca em bases de dados vazadas | https://dehashed.com/ |
| **Mozilla Monitor** | Monitoramento de vazamentos | https://monitor.mozilla.org/ |

### 19.5 Frameworks e Ferramentas OSINT (Investigativo)

| Ferramenta | Tipo | Diferencial |
|---|---|---|
| **Maltego** | Grafo/Visual | Plataforma clássica de OSINT, transformas comunitárias |
| **SpiderFoot** | Automatizado | 200+ módulos, rastreio automático de alvos |
| **theHarvester** | Recon | Coleta e-mails, subdomínios, hosts |
| **Recon-ng** | Framework | Framework modular Python para reconhecimento |
| **Sherlock** | Username | Busca usernames em 300+ redes sociais |
| **WhatsMyName** | Username | Web/CLI para lookup de usernames |
| **Holehe** | E-mail | Verifica em quais sites um e-mail tem conta |
| **GHunt** | Google | OSINT em contas Google (Gaia ID) |
| **OSINT Framework** | Diretório | Mapa visual de centenas de ferramentas | https://osintframework.com/ |
| **Photon** | Crawler | Crawler rápido para extrair dados de sites |
| **shodan.io** | Buscador | Motor de busca de dispositivos conectados |
| **Censys.io** | Buscador | Indexa hosts e certificados na internet |
| **GreyNoise** | Threat intel | Filtra ruído de scans massivos da internet |
| **EXIF.tools / FotoForensics** | Análise de imagem | Análise forense de imagens |
| **Yandex Reverse Image** | Imagens | Busca reversa muito eficaz para faces |
| **Wayback Machine** | Histórico web | Snapshots históricos de sites | https://web.archive.org/ |

---

## 34. REMOÇÃO DE DADOS PESSOAIS (DATA BROKERS)

### [Camada 4 — Aplicação]

| Serviço | Tipo | Cobertura | Diferencial | Link |
|---|---|---|---|---|
| **Incogni** | Automatizado | EUA, UK, Canadá, Suíça, UE | Remove dados de 180+ data brokers automaticamente, do grupo Surfshark | https://incogni.com/ |
| **DeleteMe** | Automatizado | EUA | Remove dados pessoais de data brokers, relatórios trimestrais | https://joindeleteme.com/ |
| **Privacy Duck** | Manual/Assistido | EUA | Remoção manual assistida, foco em completude | https://www.privacyduck.com/ |
| **Kanary** | Automatizado | EUA | Monitoramento contínuo + remoção de 400+ fontes | https://www.thekanary.com/ |
| **Optery** | Automatizado | EUA | Painel de controle visual, remoção de 300+ data brokers | https://www.optery.com/ |
| **JustDeleteMe** | Diretório/Manual | Global | Diretório de links diretos para deletar contas em serviços web | https://justdeleteme.xyz/ |
| **AccountKiller** | Diretório/Manual | Global | Guias passo a passo para deletar contas online | https://www.accountkiller.com/ |

> **LGPD/GDPR:** Cidadãos brasileiros e europeus podem exercer o direito de exclusão diretamente junto às empresas. Use modelos de solicitação LGPD disponíveis no site da ANPD.

---

## 37. PRIVACIDADE EM IA E LLMs

### [Camada 4 — Aplicação]

| Ferramenta/Prática | Tipo | Diferencial | Link |
|---|---|---|---|
| **DuckDuckGo AI Chat** | Chat IA privado | Acesso anônimo a LLMs (Claude, GPT, Llama), sem armazenamento de conversas | https://duckduckgo.com/aichat |
| **Brave Leo** | Chat IA no navegador | IA integrada ao Brave, conversas não associadas a conta, processamento local quando possível | https://brave.com/leo/ |
| **Ollama** | LLM local | Roda LLMs localmente (Llama, Mistral, Gemma, etc.), sem envio de dados para nuvem | https://ollama.com/ |
| **LM Studio** | LLM local | Interface gráfica para rodar LLMs localmente, chat e API local | https://lmstudio.ai/ |
| **Jan** | LLM local | Cliente open-source para LLMs locais, offline-first | https://jan.ai/ |
| **GPT4All** | LLM local | Roda modelos localmente, gratuito, privado | https://gpt4all.io/ |
| **CamoCopy** | Anonimização de texto | Remove padrões estilísticos (stylometry) do texto antes de postar, protege autoria | https://www.camocopy.com/ |
| **Open WebUI** | Interface local | UI web auto-hospedada para Ollama/llama.cpp, multi-usuário | https://openwebui.com/ |
| **AnythingLLM** | RAG local | Chat com seus documentos sem enviar à nuvem | https://anythingllm.com/ |
| **PrivateGPT** | RAG local | Pipeline RAG 100% offline | https://github.com/zylon-ai/private-gpt |
| **llama.cpp / llamafile** | Inferência local | Execução eficiente de LLMs em CPU/GPU comum | https://github.com/ggerganov/llama.cpp |
| **HuggingChat** | Chat IA aberto | Chat com modelos open-source hospedado pela Hugging Face | https://huggingface.co/chat |
| **Venice.ai** | Chat IA privado | Sem armazenamento de conversas, modelos open-source | https://venice.ai/ |
| **Mistral Le Chat** | Chat IA UE | Empresa francesa, conformidade GDPR | https://chat.mistral.ai/ |
| **Perplexity (modo incógnito)** | Busca IA | Modo que não retém histórico nem treina | https://www.perplexity.ai/ |
| **Whisper.cpp** | STT local | Transcrição de áudio offline com Whisper da OpenAI | https://github.com/ggerganov/whisper.cpp |
| **Piper TTS** | TTS local | Text-to-speech offline de qualidade | https://github.com/rhasspy/piper |
| **Coqui TTS / XTTS** | TTS local | Síntese de voz multilíngue offline | https://github.com/coqui-ai/TTS |

> ⚠️ **RISCO IA:** Todo texto enviado a serviços de IA na nuvem (ChatGPT, Gemini, etc.) pode ser usado para treinamento. Para dados sensíveis, use LLMs locais (Ollama, LM Studio) ou serviços com política explícita de não-treinamento (DuckDuckGo AI Chat, API do Claude).

---

## 47. FERRAMENTAS FORENSES E ANTI-STALKERWARE

### [Transversal]

| Ferramenta | Open-Source | Plataformas | Tipo | Diferencial | Link |
|---|---|---|---|---|---|
| **MVT (Mobile Verification Toolkit)** | ✅ Sim | Android, iOS | Forense | Detecta indicadores de spyware tipo Pegasus, da Amnesty | https://mvt.re/ |
| **iVerify** | ❌ Não | iOS, Android | Forense/EDR | Verifica integridade do dispositivo e ameaças | https://www.iverify.io/ |
| **Stalkerware-Indicators** | ✅ Sim | Multi | Lista | Lista de IOCs da Coalition Against Stalkerware | https://github.com/AssoEchap/stalkerware-indicators |
| **TinyCheck** | ✅ Sim | Linux/RPi | Rede | Box que analisa tráfego de um celular suspeito (Kaspersky) | https://github.com/KasperskyLab/TinyCheck |
| **Warden (Android)** | ✅ Sim | Android | Scanner | Detecção de stalkerware | F-Droid |
| **Autopsy** | ✅ Sim | Multi | Forense | Plataforma forense digital baseada em Sleuth Kit | https://www.autopsy.com/ |
| **The Sleuth Kit (TSK)** | ✅ Sim | Multi | Forense | Conjunto CLI para forense de discos | https://www.sleuthkit.org/ |
| **Volatility 3** | ✅ Sim | Multi | Forense de memória | Framework para análise de RAM | https://www.volatilityfoundation.org/ |
| **Velociraptor** | ✅ Sim | Multi | DFIR | EDR e forense em endpoints distribuídos | https://docs.velociraptor.app/ |
| **GRR Rapid Response** | ✅ Sim | Multi | DFIR | Framework forense remoto (Google) | https://github.com/google/grr |
| **Caine Linux** | ✅ Sim | Live | Distro forense | Distro Linux para investigações | https://www.caine-live.net/ |
| **OSForensics** | ❌ Não | Windows | Forense | Suite forense Windows | https://www.osforensics.com/ |

---

## 54. CRIPTOGRAFIA PÓS-QUÂNTICA E FERRAMENTAS AVANÇADAS

### [Camada 4]

| Ferramenta | Open-Source | Tipo | Diferencial | Link |
|---|---|---|---|---|
| **liboqs** | ✅ Sim | Lib | Biblioteca Open Quantum Safe (Kyber, Dilithium, SPHINCS+) | https://openquantumsafe.org/ |
| **OQS-OpenSSL / OQS-OpenSSH** | ✅ Sim | Fork | OpenSSL/SSH com algoritmos PQC | https://openquantumsafe.org/ |
| **Signal PQXDH** | ✅ Sim | Protocolo | Acordo de chaves híbrido (X25519 + Kyber) já em produção | https://signal.org/docs/specifications/pqxdh/ |
| **PQ3 (Apple iMessage)** | ❌ Não | Protocolo | Acordo PQ híbrido + ratchet em iMessage | — |
| **Cloudflare Post-Quantum TLS** | ✅ Sim | TLS | Suporte experimental em produção | https://blog.cloudflare.com/post-quantum-for-all/ |
| **age + age-plugin-pqc** | ✅ Sim | Arquivos | Plugin PQ para age | — |
| **wolfSSL/wolfCrypt PQ** | Parcial | Lib | Algoritmos PQ em embarcados | — |
| **Botan** | ✅ Sim | Lib | Biblioteca cripto C++ com PQC | https://botan.randombit.net/ |
| **Tink** | ✅ Sim | Lib | Lib do Google com APIs seguras por padrão | https://github.com/tink-crypto/tink |
| **NaCl / libsodium** | ✅ Sim | Lib | API simples para curvas modernas | https://libsodium.org/ |
| **Cryptography.io (Python)** | ✅ Sim | Lib | Lib pythônica recomendada | https://cryptography.io/ |
| **HashiCorp Vault** | ✅ Sim | Cofre | Cofre de segredos para infra, suporte HSM | https://www.vaultproject.io/ |
| **Bitwarden Secrets Manager** | ✅ Sim | Cofre | Secrets para devs/infra | https://bitwarden.com/ |
| **Doppler / Infisical** | Parcial | Cofre | Infisical é open-source | https://infisical.com/ |
| **OpenSSF Sigstore (cosign)** | ✅ Sim | Assinatura | Assinatura keyless de artefatos/SW | https://www.sigstore.dev/ |

---

## 60. FERRAMENTAS DE CONSCIENTIZAÇÃO E EDUCAÇÃO

### [Transversal]

| Recurso | Tipo | Diferencial | Link |
|---|---|---|---|
| **EFF Surveillance Self-Defense** | Guia | Guias de autodefesa digital, em PT-BR | https://ssd.eff.org/pt-br |
| **Privacy Guides** | Diretório | Recomendações curadas de ferramentas | https://www.privacyguides.org/ |
| **Awesome Privacy** | Diretório | Lista colaborativa de ferramentas | https://awesome-privacy.xyz/ |
| **Awesome Selfhosted** | Diretório | Lista de software para auto-hospedagem | https://awesome-selfhosted.net/ |
| **Privacy Tools (clássico)** | Diretório | Listas históricas (use com cautela, datado) | https://www.privacytools.io/ |
| **PRISM Break** | Diretório | Alternativas a serviços vigiados | https://prism-break.org/ |
| **Reset The Net** | Campanha | Campanha histórica EFF | https://resetthenet.org/ |
| **Security Planner (Consumer Reports)** | Quiz | Plano personalizado de segurança | https://securityplanner.consumerreports.org/ |
| **Citizen Lab** | Pesquisa | Pesquisas sobre vigilância e censura | https://citizenlab.ca/ |
| **Access Now Helpline** | Suporte | Linha direta para ativistas em risco | https://www.accessnow.org/help/ |
| **CryptoParty** | Movimento | Workshops presenciais de cripto | https://www.cryptoparty.in/ |
| **Tactical Tech (Data Detox Kit)** | Curso | Curso de "detox" digital | https://datadetoxkit.org/ |
| **Tor Project — Training** | Material | Materiais oficiais para treinamentos | https://community.torproject.org/training/ |
| **CISA Stop Ransomware** | Guia | Guia oficial dos EUA contra ransomware | https://www.cisa.gov/stopransomware |
| **CERT.br** | Guia (BR) | Cartilha de Segurança para Internet | https://cartilha.cert.br/ |
| **gov.br Cibersegurança** | Guia (BR) | Recomendações oficiais do governo brasileiro | https://www.gov.br/governodigital/pt-br/seguranca-e-protecao-de-dados |
| **ANPD (BR)** | Regulador | Modelos LGPD e orientações | https://www.gov.br/anpd/ |
| **HackTricks / PayloadsAllTheThings** | Wiki | Recursos para defensores entenderem ataques | https://book.hacktricks.xyz/ |
| **TryHackMe / HackTheBox / OverTheWire** | Plataforma | Treinamento prático ofensivo/defensivo | https://tryhackme.com/ |
| **OpenSSF Best Practices Badge** | Padrão | Checklist de boas práticas de segurança em SW | https://www.bestpractices.dev/ |
| **OWASP Top 10 / ASVS / Cheat Sheets** | Padrão | Referências obrigatórias para AppSec | https://owasp.org/ |
| **MITRE ATT&CK** | Framework | Framework de táticas e técnicas adversárias | https://attack.mitre.org/ |
| **NIST CSF 2.0** | Framework | Framework de cibersegurança do NIST | https://www.nist.gov/cyberframework |
| **CIS Controls / Benchmarks** | Padrão | Controles e baselines de hardening | https://www.cisecurity.org/ |

---

## DIRETRIZES GERAIS

### Regra 3-2-1 de Backup
Mantenha 3 cópias dos dados, em 2 tipos de mídia diferentes, com 1 cópia offsite.

### Higiene de Senhas
- Use gerenciador de senhas (nunca reutilize senhas)
- Ative 2FA em todas as contas (preferencialmente TOTP ou FIDO2, nunca SMS)
- Senhas com 14+ caracteres, aleatórias

### Modelo de Ameaça
Antes de escolher ferramentas, avalie: Quem são seus adversários? Quais dados proteger? Qual seu nível de tolerância a inconveniência?

### Defense in Depth
Nenhuma ferramenta isolada resolve tudo. Combine: navegador seguro + VPN + DNS criptografado + 2FA + gerenciador de senhas + criptografia de disco.

### Atualizações
Ferramentas desatualizadas são piores do que não tê-las. Mantenha TUDO atualizado.

### Princípio do Menor Privilégio
Apps e usuários devem ter apenas as permissões estritamente necessárias. Revise permissões de apps mensalmente, especialmente em mobile.

### Compartimentalização
Separe identidades por contexto (trabalho, pessoal, financeiro, anonimato). Use perfis de navegador, containers, contas/aliases de e-mail e até dispositivos diferentes quando o modelo de ameaça exigir.

### Verificação de Integridade
Sempre verifique assinaturas GPG/SHA256 de software baixado, especialmente de ferramentas críticas (Tor, Tails, VeraCrypt, sistemas operacionais).

### Plano de Resposta a Incidentes Pessoal
Tenha definido: (1) como revogar acessos rapidamente, (2) lista de contas críticas e onde estão os 2FA backup codes, (3) contato de confiança, (4) procedimento de wipe remoto de dispositivos.

### Avalie a Cadeia de Suprimentos
Prefira ferramentas open-source auditadas, com builds reprodutíveis e múltiplos mantenedores. Desconfie de ferramentas adquiridas recentemente por grandes grupos sem histórico transparente.

### Higiene de Metadados
Lembre-se: o conteúdo pode estar criptografado, mas metadados (quem, quando, onde, com quem) muitas vezes não estão. Considere isso ao escolher ferramentas.

---

