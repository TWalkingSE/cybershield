# CYBERSHIELD — Base de Conhecimento: Ferramentas de Segurança Digital e Privacidade

> **Versão:** 4.0 | **Atualização:** Abril 2026
> **Fonte primária:** "Proteja-se Online: Dicas e Softwares Essenciais para Sua Segurança Digital" (TWalking, 1ª Edição, Janeiro 2025)
> **Fontes complementares:** PrivacyGuides.org, PrivacyTools.io, EFF, awesome-selfhosted, auditorias independentes, documentação oficial das ferramentas.

---

## 3. BACKUP E ARMAZENAMENTO EM NUVEM

### [Camada 4 — Aplicação]

### 3.1 Nuvem com Foco em Privacidade

| Ferramenta | Open-Source | E2EE | Armazenamento | Diferencial | Link |
|---|---|---|---|---|---|
| **Proton Drive** | ✅ Sim | ✅ Nativo | 1-500 GB+ | E2EE por padrão, ecossistema Proton, Suíça | https://proton.me/drive |
| **Tresorit** | ❌ Não | ✅ Nativo | 200 GB - 4 TB | E2EE, compliance empresarial, Suíça | https://tresorit.com/ |
| **Sync.com** | ❌ Não | ✅ Nativo | 5 GB grátis, até 6 TB | E2EE, zero-knowledge, Canadá | https://www.sync.com/ |
| **Nextcloud** | ✅ Sim | ✅ (com E2EE plugin) | Auto-hospedado | 100% controle do usuário, auto-hospedável | https://nextcloud.com/ |
| **Cryptomator** | ✅ Sim | ✅ Sim | Complementar | Criptografa arquivos antes de enviar para QUALQUER nuvem (Google Drive, Dropbox, etc.) | https://cryptomator.org/ |
| **Filen** | Parcial | ✅ Nativo | 10 GB grat. – 2 TB | E2EE zero-knowledge, Alemanha, sync e drive virtual | https://filen.io/ |
| **MEGA** | Parcial (cliente) | ✅ Nativo | 20 GB grat. – 16 TB | E2EE com chave do usuário, Nova Zelândia. ⚠️ Histórico controverso (Kim Dotcom) | https://mega.io/ |
| **pCloud** | ❌ Não | ✅ Crypto add-on | 10 GB grat. – 2 TB | Pagamento único (lifetime), pCloud Crypto opcional, Suíça | https://www.pcloud.com/ |
| **Internxt** | ✅ Sim | ✅ Nativo | 10 GB grat. – 2 TB | E2EE zero-knowledge, Espanha, integração com IPFS | https://internxt.com/ |
| **Seafile** | ✅ Sim | ✅ (biblioteca) | Auto-hospedado | Sync confiável para equipes, criptografia de bibliotecas | https://www.seafile.com/ |
| **OwnCloud Infinite Scale** | ✅ Sim | Parcial | Auto-hospedado | Reescrita em Go do OwnCloud clássico | https://owncloud.com/ |

### 3.2 Nuvem Geral (sem E2EE nativo — considerar Cryptomator)

| Ferramenta | Criptografia | Armazenamento Gratuito | Diferencial | Link |
|---|---|---|---|---|
| **Google Drive** | AES-256 em repouso, TLS em trânsito. Sem E2EE. | 15 GB | Integração Google Workspace, histórico 30 dias | https://drive.google.com/ |
| **OneDrive** | AES-256, TLS. Personal Vault com camada extra. Sem E2EE. | 5 GB | Integração Windows/Office 365, recuperação ransomware | https://onedrive.live.com/ |
| **Dropbox** | AES-256, TLS. Sem E2EE. | 2 GB | Smart Sync, integração com Slack e Office | https://www.dropbox.com/pt_BR/ |
| **Backblaze** | AES-256, TLS. E2EE com chave privada (opcional). | Ilimitado (backup) | Custo-benefício excepcional, recuperação física (disco enviado) | https://www.backblaze.com/ |
| **IDrive** | AES-256, TLS. E2EE com chave privada (opcional). | 10 GB | Multi-dispositivo, IDrive Express (envio físico), HIPAA compliant | https://www.idrive.com/ |
| **Acronis True Image** | AES-256, E2EE com chave privada. | — (pago) | Backup híbrido (local+nuvem), clone de disco, anti-ransomware integrado (Active Protection) | https://www.acronis.com/pt-br/products/true-image/ |
| **Carbonite** | AES-128/256, TLS. Chave privada opcional. | — (pago) | Armazenamento ilimitado (planos pessoais), interface simples | https://www.carbonite.com/ |

### 3.3 Backup Local (Software)

| Ferramenta | Open-Source | Plataformas | Diferencial |
|---|---|---|---|
| **BorgBackup** | ✅ Sim | Linux, macOS | Deduplicação, compressão, criptografia AES-256, eficiente para backups incrementais |
| **Restic** | ✅ Sim | Windows, macOS, Linux | Multi-backend (local, S3, SFTP, etc.), criptografia por padrão |
| **Kopia** | ✅ Sim | Windows, macOS, Linux | GUI e CLI, snapshots, criptografia, deduplicação |
| **Duplicati** | ✅ Sim | Windows, macOS, Linux | Interface web, suporte a 20+ backends de nuvem, criptografia AES-256 |
| **Vorta** | ✅ Sim | Windows, macOS, Linux | GUI Qt para BorgBackup, agendamento, snapshots |
| **Pika Backup** | ✅ Sim | Linux | GUI GNOME para BorgBackup, simples para usuários domésticos |
| **Deja Dup** | ✅ Sim | Linux | Frontend GNOME para Duplicity, integrado ao Ubuntu |
| **Time Shift** | ✅ Sim | Linux | Snapshots tipo Time Machine, restauração do sistema |
| **rsync** | ✅ Sim | Linux, macOS, Windows (WSL) | CLI clássico para cópias incrementais, base de muitos scripts |
| **Arq Backup** | ❌ Não | Windows, macOS | Backup criptografado para vários provedores de nuvem, pagamento único |
| **Macrium Reflect** | ❌ Não | Windows | Imagem de disco, backup incremental, versão gratuita |
| **Veeam Agent Free** | ❌ Não | Windows, Linux | Backup empresarial em versão gratuita para uso pessoal |

---

## 4. CRIPTOGRAFIA DE DADOS

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Plataformas | Tipo | Diferencial | Link |
|---|---|---|---|---|---|
| **VeraCrypt** | ✅ Sim | Windows, macOS, Linux | Disco/Volume | Criptografia de disco completo, volumes ocultos (deniable encryption), AES/Twofish/Serpent | https://www.veracrypt.fr/ |
| **Cryptomator** | ✅ Sim | Windows, macOS, Linux, Android, iOS | Arquivos/Nuvem | Criptografa arquivos individuais para nuvem, transparente ao usuário | https://cryptomator.org/ |
| **GnuPG (GPG)** | ✅ Sim | Windows, macOS, Linux | Arquivos/E-mail | Criptografia de e-mail (PGP), assinatura digital, padrão OpenPGP | https://gnupg.org/ |
| **age** | ✅ Sim | Windows, macOS, Linux | Arquivos | Criptografia simples e moderna, substituição do GPG para uso cotidiano | https://age-encryption.org/ |
| **BitLocker** | ❌ Não | Windows 10/11 Pro/Enterprise | Disco | Integrado ao Windows, TPM, criptografia AES-128/256. ⚠️ Chave pode ser enviada para conta Microsoft | — |
| **FileVault** | ❌ Não | macOS | Disco | Criptografia de disco nativa do macOS, XTS-AES-128. ⚠️ Chave pode ser armazenada no iCloud | — |
| **LUKS** | ✅ Sim | Linux | Disco | Padrão de criptografia de disco do Linux, AES-256 | — |
| **AxCrypt** | Parcial | Windows, macOS, Android, iOS | Arquivos | Criptografia de arquivos individuais, integração com cloud. ⚠️ Versão gratuita limitada | https://www.axcrypt.net/ |
| **NordLocker** | ❌ Não | Windows, macOS | Arquivos/Nuvem | Criptografia de arquivos com armazenamento em nuvem E2EE, interface simples | https://nordlocker.com/ |
| **7-Zip** | ✅ Sim | Windows, Linux | Arquivos | Compressão + criptografia AES-256, formato 7z | https://www.7-zip.org/ |
| **Tresorit** | ❌ Não | Windows, macOS, Linux, Android, iOS | Nuvem | Armazenamento em nuvem com E2EE, Suíça | https://tresorit.com/ |
| **Picocrypt** | ✅ Sim | Windows, macOS, Linux | Arquivos | Pequeno (~3 MB), XChaCha20, Argon2id, portátil | https://github.com/Picocrypt/Picocrypt |
| **rage** | ✅ Sim | Multi | Arquivos | Implementação em Rust de `age`, suporte a YubiKey | https://github.com/str4d/rage |
| **Kleopatra** | ✅ Sim | Windows, Linux | Chaves PGP/X.509 | GUI para GnuPG, gestão de chaves, cifragem de e-mail | https://www.openpgp.org/software/kleopatra/ |
| **Sequoia PGP** | ✅ Sim | Multi | OpenPGP | Implementação moderna de OpenPGP em Rust | https://sequoia-pgp.org/ |
| **OpenSSL** | ✅ Sim | Multi | Toolkit | Criptografia de arquivos via CLI (`openssl enc`), TLS, certs | https://www.openssl.org/ |
| **Hat.sh** | ✅ Sim | Web | Arquivos | Criptografia client-side no navegador (XChaCha20-Poly1305) | https://hat.sh/ |
| **Tomb** | ✅ Sim | Linux | Volume | Wrapper de LUKS para criar “túmulos” criptografados portáteis | https://www.dyne.org/software/tomb/ |
| **gocryptfs** | ✅ Sim | Linux, macOS | Sistema de arquivos | Filesystem criptografado em userspace, AES-GCM | https://nuetzlich.net/gocryptfs/ |
| **EncFS** | ✅ Sim | Linux, macOS, Windows | Sistema de arquivos | Filesystem criptografado em userspace (⚠️ auditoria 2014 apontou fraquezas) | https://vgough.github.io/encfs/ |

---

## 5. EXCLUSÃO SEGURA DE DADOS

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Plataformas | Tipo | Diferencial | Link |
|---|---|---|---|---|---|
| **BleachBit** | ✅ Sim | Windows, Linux | Arquivos/Sistema | Limpeza de sistema + exclusão segura, padrões Gutmann/DoD | https://www.bleachbit.org/ |
| **Eraser** | ✅ Sim | Windows | Arquivos/Disco | Exclusão segura com agendamento, múltiplos algoritmos (Gutmann, DoD 5220.22-M) | https://eraser.heidi.ie/ |
| **DBAN (Darik's Boot and Nuke)** | ✅ Sim | Boot (qualquer SO) | Disco completo | Apagamento total de disco via boot, ideal para descarte de hardware | https://dban.org/ |
| **shred** | ✅ Sim | Linux/macOS | Arquivos | Comando nativo do Linux para sobrescrita segura de arquivos | — (nativo) |
| **secure-delete (srm)** | ✅ Sim | Linux | Arquivos/Disco | Suite com srm, sfill, sswap, smem para exclusão segura | — |
| **BCWipe** | ❌ Não | Windows | Arquivos/Disco | Apagamento certificado (DoD, NIST), logs de auditoria para compliance | https://www.jetico.com/ |
| **Secure Eraser** | ❌ Não | Windows | Arquivos/Disco | Apagamento seguro com 5 métodos, limpeza de registro e espaço livre | https://www.ascompsoftware.com/ |
| **CCleaner (Wipe)** | ❌ Não | Windows, macOS | Arquivos/Sistema | Limpeza de sistema + exclusão segura (1-35 passagens). ⚠️ Histórico de bundleware | https://www.ccleaner.com/pt-br |
| **WipeFile** | ❌ Não | Windows | Arquivos | Leve, portátil, 14 métodos de apagamento | https://www.gaijin.at/en/software/wipefile |
| **File Shredder** | ❌ Não | Windows | Arquivos | Gratuito, 5 algoritmos de sobrescrita, integração com menu de contexto | https://www.fileshredder.org/ |
| **nwipe** | ✅ Sim | Linux | Disco | Sucessor open-source do DBAN, múltiplos métodos (DoD, Gutmann, PRNG) | https://github.com/martijnvanbrummelen/nwipe |
| **ShredOS** | ✅ Sim | Boot | Disco | Distribuição mínima focada em rodar `nwipe` | https://github.com/PartialVolume/shredos.x86_64 |
| **HDDErase** | ✅ Sim | Boot | Disco/SSD | Usa comando ATA Secure Erase nativo (ideal para SSDs) | — |
| **Parted Magic** | ❌ Não | Boot | Disco/SSD | Conjunto profissional com Secure Erase para SSDs e HDDs | https://partedmagic.com/ |
| **Blancco Drive Eraser** | ❌ Não | Boot/Live | Disco | Padrão corporativo certificado (NIST, DoD), relatórios auditáveis | https://www.blancco.com/ |

---

## 35. SINCRONIZAÇÃO DE ARQUIVOS (P2P)

### [Camada 4 — Aplicação / Camada 3 — Transporte]

| Ferramenta | Open-Source | Plataformas | Diferencial | Link |
|---|---|---|---|---|
| **Syncthing** | ✅ Sim | Windows, macOS, Linux, Android | Sincronização P2P sem nuvem, E2EE, sem servidor central, relay opcional | https://syncthing.net/ |
| **Resilio Sync** | ❌ Não | Windows, macOS, Linux, Android, iOS | Sync P2P baseado em BitTorrent, rápido, planos empresariais | https://www.resilio.com/ |
| **Rclone** | ✅ Sim | Windows, macOS, Linux | CLI para sync com 40+ backends (S3, GDrive, Dropbox, SFTP), criptografia | https://rclone.org/ |
| **Unison** | ✅ Sim | Multi | Sync bidirecional clássico via SSH | https://www.cis.upenn.edu/~bcpierce/unison/ |
| **FreeFileSync** | ✅ Sim | Multi | GUI multiplataforma para sync entre pastas | https://freefilesync.org/ |
| **SyncBackFree** | ❌ Não | Windows | Sync e backup robustos, versão gratuita | https://www.2brightsparks.com/ |
| **Duplicacy** | Parcial | Multi | Backup/sync com lock-free deduplicação | https://duplicacy.com/ |
| **OnionShare Sync (em desenvolvimento)** | ✅ Sim | Multi | Sync via Tor onion services | https://onionshare.org/ |
| **Tailscale Drop / Taildrop** | Parcial | Multi | Compartilhamento rápido entre devices na sua tailnet | https://tailscale.com/kb/1106/taildrop |

---

