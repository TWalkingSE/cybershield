---
name: kit-privacidade
description: >
  Montagem de kit personalizado de ferramentas de privacidade e segurança.
  Use quando o usuário quiser um conjunto completo de ferramentas recomendadas, 
  "montar meu kit de segurança", "quais ferramentas usar", "stack de privacidade",
  "setup completo de privacidade", ou pedir recomendações organizadas de 
  ferramentas para seu perfil. Diferente do diagnóstico (que avalia o atual), 
  este skill CONSTRÓI o kit ideal.
---

# Kit de Privacidade Personalizado

## Fluxo

1. Identifique o nível (básico/intermediário/avançado) e modelo de ameaça
2. Monte kit organizado por camada TCP/IP
3. Indique ordem de implementação por prioridade

## Kits por Nível

### Kit Básico (usuário casual)

| Camada | Ferramenta | Por quê |
|---|---|---|
| **Aplicação** | Firefox + uBlock Origin | Bloqueio de trackers nativo |
| **Aplicação** | Bitwarden | Gerenciador de senhas gratuito, auditado |
| **Aplicação** | Signal | Mensageria E2E, open-source |
| **Aplicação** | Proton Mail (free) | E-mail criptografado |
| **Transporte** | ProtonVPN (free) | VPN sem limite de dados |
| **Transversal** | Atualizações automáticas | Patches de segurança |

### Kit Intermediário (profissional consciente)

Tudo do básico, mais:

| Camada | Ferramenta | Por quê |
|---|---|---|
| **Aplicação** | KeePassXC | Senhas offline, controle total |
| **Aplicação** | Aegis Authenticator | 2FA open-source (Android) |
| **Aplicação** | SimpleLogin | Aliases de e-mail |
| **Aplicação** | Quad9 / NextDNS | DNS criptografado |
| **Aplicação** | Standard Notes / Joplin | Notas criptografadas |
| **Transporte** | Mullvad VPN | No-log auditado, pagamento anônimo |
| **Transporte** | Portmaster | Firewall com visualização de conexões |
| **Internet** | Tor Browser (para pesquisa sensível) | Anonimato real |
| **Acesso à Rede** | MAC randomization | Impedir rastreamento por hardware |
| **Transversal** | VeraCrypt | Volumes criptografados |
| **Transversal** | BorgBackup/Restic | Backup criptografado |

### Kit Avançado (alto risco)

Tudo do intermediário, mais:

| Camada | Ferramenta | Por quê |
|---|---|---|
| **Aplicação** | Mullvad Browser | Anti-fingerprinting máximo |
| **Aplicação** | SimpleX Chat | Mensageria sem metadados |
| **Aplicação** | OnionShare | Transferência via Tor |
| **Aplicação** | Ollama / LM Studio | IA 100% local |
| **Aplicação** | CryptPad | Colaboração criptografada |
| **Internet** | Tor + bridges | Bypass de censura |
| **Acesso à Rede** | WPA3 + rede segmentada | Isolamento de IoT |
| **Transversal** | Qubes OS ou Whonix | Compartimentalização |
| **Transversal** | GrapheneOS | Android sem Google |
| **Transversal** | YubiKey | 2FA hardware, FIDO2 |
| **Transversal** | Tails (para operações sensíveis) | SO amnésico via USB |

## Ordem de Implementação

Sempre sugira implementação gradual:
1. 🔴 **Semana 1**: gerenciador de senhas + 2FA + atualizar tudo
2. 🟡 **Semana 2**: navegador seguro + DNS criptografado + VPN
3. 🟢 **Semana 3**: mensageria segura + e-mail seguro + aliases
4. 🔵 **Semana 4+**: criptografia de disco + backup + hardening de SO
