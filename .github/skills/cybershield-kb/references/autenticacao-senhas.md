# CYBERSHIELD — Base de Conhecimento: Ferramentas de Segurança Digital e Privacidade

> **Versão:** 4.0 | **Atualização:** Abril 2026
> **Fonte primária:** "Proteja-se Online: Dicas e Softwares Essenciais para Sua Segurança Digital" (TWalking, 1ª Edição, Janeiro 2025)
> **Fontes complementares:** PrivacyGuides.org, PrivacyTools.io, EFF, awesome-selfhosted, auditorias independentes, documentação oficial das ferramentas.

---

## 1. GERENCIADORES DE SENHAS E 2FA

### [Camada 4 — Aplicação]

### 1.1 Gerenciadores de Senhas

| Ferramenta | Open-Source | Plataformas | Diferencial | Link |
|---|---|---|---|---|
| **Bitwarden** | ✅ Sim | Windows, macOS, Linux, Android, iOS, Web, extensões | Open-source, auto-hospedável (Vaultwarden), plano gratuito robusto, auditado | https://bitwarden.com/ |
| **KeePassXC** | ✅ Sim | Windows, macOS, Linux | 100% offline, base de dados local criptografada (AES-256), sem nuvem | https://keepassxc.org/ |
| **1Password** | ❌ Não | Windows, macOS, Linux, Android, iOS, Web | UX premium, Travel Mode, Watchtower (monitoramento de vazamentos) | https://1password.com/pt |
| **Dashlane** | ❌ Não | Windows, macOS, Android, iOS, Web | VPN integrada, monitoramento de dark web, preenchimento automático avançado | https://www.dashlane.com/ |
| **NordPass** | ❌ Não | Windows, macOS, Linux, Android, iOS | Criptografia XChaCha20, scanner de vazamentos, do grupo Nord Security | https://nordpass.com/ |
| **Proton Pass** | ✅ Sim | Windows, macOS, Linux, Android, iOS, Web | Do ecossistema Proton, aliases de e-mail integrados, E2EE | https://proton.me/pass |
| **LastPass** | ❌ Não | Windows, macOS, Android, iOS, Web | ⚠️ ALERTA: Sofreu vazamento grave em 2022 (cofres criptografados roubados). Uso não recomendado. | https://www.lastpass.com/pt |
| **RoboForm** | ❌ Não | Windows, macOS, Android, iOS | Preenchimento de formulários avançado, plano familiar acessível | https://www.roboform.com/br |
| **Zoho Vault** | ❌ Não | Windows, macOS, Android, iOS, Web | Integração com ecossistema Zoho, gestão de senhas corporativas | https://www.zoho.com/pt-br/vault/ |
| **Vaultwarden** | ✅ Sim | Auto-hospedado (Docker) | Servidor compatível com Bitwarden escrito em Rust, leve, ideal para NAS/Raspberry Pi | https://github.com/dani-garcia/vaultwarden |
| **Psono** | ✅ Sim | Auto-hospedado, Web, extensões | Foco corporativo, compartilhamento granular, auditoria | https://psono.com/ |
| **Passbolt** | ✅ Sim | Auto-hospedado, Web, Desktop, Mobile | Gerenciador de senhas para times, baseado em OpenPGP | https://www.passbolt.com/ |
| **pass (Unix Password Store)** | ✅ Sim | Linux, macOS (CLI) | CLI Unix, GPG + Git, filosofia KISS | https://www.passwordstore.org/ |
| **gopass** | ✅ Sim | Windows, macOS, Linux | Sucessor do `pass` em Go, suporte a múltiplos cofres e equipes | https://www.gopass.pw/ |
| **Enpass** | ❌ Não | Windows, macOS, Linux, Android, iOS | Armazenamento local ou em sua própria nuvem (sem servidor próprio) | https://www.enpass.io/ |
| **Strongbox** | Parcial | macOS, iOS | Compatível com KeePass, integração iCloud/Dropbox | https://strongboxsafe.com/ |
| **KeeWeb** | ✅ Sim | Windows, macOS, Linux, Web | Cliente web/desktop compatível com KeePass | https://keeweb.info/ |

### 1.2 Autenticação de Dois Fatores (2FA)

| Ferramenta | Open-Source | Plataformas | Diferencial | Link |
|---|---|---|---|---|
| **Aegis Authenticator** | ✅ Sim | Android | Backup criptografado, importação de outros apps, interface limpa | https://getaegis.app/ |
| **Ente Auth** | ✅ Sim | Android, iOS, Web, Desktop | Backup E2EE em nuvem, multiplataforma, do mesmo time do Ente Photos | https://ente.io/auth/ |
| **Yubico Authenticator** | ✅ Sim | Windows, macOS, Linux, Android, iOS | Requer chave YubiKey física, TOTP armazenado no hardware | https://www.yubico.com/products/yubico-authenticator/ |
| **Authy** | ❌ Não | Windows, macOS, Linux, Android, iOS | Backup em nuvem, multi-dispositivo. ⚠️ Requer número de telefone, código proprietário | https://authy.com/ |
| **Google Authenticator** | ❌ Não | Android, iOS | Simples e funcional. ⚠️ Backup em nuvem NÃO é E2EE; Google pode acessar os códigos | — |
| **Microsoft Authenticator** | ❌ Não | Android, iOS | Integração com ecossistema Microsoft, login sem senha, backup em nuvem | — |
| **2FAS Auth** | ✅ Sim | Android, iOS, extensões | Backup em nuvem opcional, sincronização entre celular e navegador | https://2fas.com/ |
| **Raivo OTP** | ✅ Sim | iOS, macOS | Backup criptografado iCloud, código aberto | https://raivo-otp.com/ |
| **andOTP** | ✅ Sim | Android | Backup criptografado, descontinuado mas amplamente usado (→ migrar para Aegis) | F-Droid |
| **FreeOTP+** | ✅ Sim | Android | Da Red Hat, simples, com backup e import | F-Droid |
| **Stratum (ex-Cotp)** | ✅ Sim | Android | TOTP/HOTP com sincronização autohospedada opcional | F-Droid |
| **OnlyKey** | ✅ Sim (firmware) | Hardware | Chave hardware com TOTP, senhas e FIDO2 em um único dispositivo | https://onlykey.io/ |

---

## 24. CHAVES DE SEGURANÇA FÍSICAS (HARDWARE)

### [Transversal — Múltiplas Camadas]

| Dispositivo | Protocolos | Diferencial |
|---|---|---|
| **YubiKey 5 Series** | FIDO2, U2F, TOTP, PIV, OpenPGP | Padrão da indústria, ampla compatibilidade, USB-A/C/NFC |
| **YubiKey Security Key** | FIDO2, U2F | Versão acessível, focada em FIDO2 |
| **Nitrokey** | FIDO2, OpenPGP, TOTP | Open-source (hardware e firmware), fabricado na Alemanha |
| **SoloKeys** | FIDO2, U2F | Open-source, acessível |
| **OnlyKey** | FIDO2, TOTP, senhas, PGP | Armazena senhas no hardware + 2FA, PIN de proteção |
| **Token2** | FIDO2, TOTP | Acessível, programaável para TOTP fixo |
| **Feitian ePass** | FIDO2, U2F | Linha econômica certificada FIDO |
| **GoTrust Idem Key** | FIDO2, U2F | Acessível, USB-A/C/Lightning |
| **Trustkey** | FIDO2, U2F | Coreano, certificação FIDO L1 |
| **Google Titan Security Key** | FIDO2, U2F | Chave do Google, USB-A/C/NFC |
| **Apple Security Keys** | FIDO2 | Suporte oficial em contas Apple ID (iOS 16.3+) |
| **NitroKey 3** | FIDO2, OpenPGP, OTP | Open-hardware, RISC-V, atualizável |
| **Tillitis TKey** | Customizável | Chave RISC-V open-hardware programável |

## 46. COMPARTILHAMENTO SEGURO DE SENHAS/SEGREDOS

### [Camada 4 — Aplicação]

| Ferramenta | Open-Source | Tipo | Diferencial | Link |
|---|---|---|---|---|
| **Bitwarden Send** | ✅ Sim | Texto/arquivo | Expiração e proteção por senha, integrado ao Bitwarden | https://bitwarden.com/products/send/ |
| **OneTimeSecret** | ✅ Sim | Texto | Burn-after-reading clássico | https://onetimesecret.com/ |
| **PasswordPusher (pwpush)** | ✅ Sim | Texto | Auto-hospedável, expiração configurável | https://pwpush.com/ |
| **Yopass** | ✅ Sim | Texto/arquivo | Em Go, fácil de hospedar | https://github.com/jhaals/yopass |
| **Snappass** | ✅ Sim | Texto | Compartilhamento interno (Pinterest) | https://github.com/pinterest/snappass |
| **Hemmelig** | ✅ Sim | Texto/arquivo | Burn-after-reading com anexos | https://hemmelig.app/ |
| **Vaultwarden Send** | ✅ Sim | Texto/arquivo | Vaultwarden auto-hospedado com Send | https://github.com/dani-garcia/vaultwarden |
| **CryptGeon** | ✅ Sim | Texto/arquivo | Notas seguras com expiração | https://cryptgeon.org/ |
| **PrivateBin (burn)** | ✅ Sim | Texto | Pastebin com burn-after-reading | https://privatebin.info/ |
| **Send.tresorit.com** | ❌ Não | Arquivo | E2EE com controle de acesso | https://send.tresorit.com/ |
| **Firefox Send (descontinuado)** | ✅ Sim (legado) | — | Vários forks hosted (ex: send.vis.ee) | — |

---

## 59. GERENCIAMENTO DE IDENTIDADE E SSO PRIVADO

### [Camada 4]

| Ferramenta | Open-Source | Tipo | Diferencial | Link |
|---|---|---|---|---|
| **Keycloak** | ✅ Sim | IdP/SSO | OIDC/SAML/LDAP, padrão da indústria FOSS | https://www.keycloak.org/ |
| **Authentik** | ✅ Sim | IdP/SSO | UI moderna, fluxos customizáveis | https://goauthentik.io/ |
| **Authelia** | ✅ Sim | SSO/2FA | Camada de auth em frente a reverse proxies | https://www.authelia.com/ |
| **Zitadel** | ✅ Sim | IdP/SSO | OIDC + SaaS auto-hospedável | https://zitadel.com/ |
| **Ory Kratos / Hydra** | ✅ Sim | IdP/Stack | Stack modular para identidade | https://www.ory.sh/ |
| **Casdoor** | ✅ Sim | IdP/SSO | UI completa com social logins | https://casdoor.org/ |
| **LemonLDAP::NG** | ✅ Sim | SSO | SSO veterano francês | https://lemonldap-ng.org/ |
| **FreeIPA** | ✅ Sim | Identity | Identity management para Linux/UNIX | https://www.freeipa.org/ |
| **OpenLDAP** | ✅ Sim | Diretório | LDAP server clássico | https://www.openldap.org/ |
| **Samba AD** | ✅ Sim | AD | Implementação livre de AD | https://www.samba.org/ |
| **vouch-proxy / oauth2-proxy** | ✅ Sim | Proxy auth | Adiciona OIDC a qualquer reverse proxy | https://github.com/oauth2-proxy/oauth2-proxy |
| **Pomerium** | ✅ Sim | ZTNA | Proxy zero-trust com policy engine | https://www.pomerium.com/ |
| **Cloudflare Access (Zero Trust)** | ❌ Não | ZTNA | ZTNA gerenciado | https://www.cloudflare.com/zero-trust/ |
| **passkeys.io / SimpleWebAuthn** | ✅ Sim | WebAuthn | Suporte a passkeys em apps próprios | https://simplewebauthn.dev/ |

---

