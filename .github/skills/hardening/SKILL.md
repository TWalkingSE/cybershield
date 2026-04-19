---
name: hardening
description: >
  Tutorial guiado de hardening passo a passo para sistemas e dispositivos.
  Use quando o usuário quiser proteger/endurecer Windows, macOS, Linux, Android, 
  iOS, navegadores, roteadores ou redes. Exemplos: "como proteger meu Windows", 
  "hardening Firefox", "configurar privacidade no Android", "proteger meu 
  roteador", "checklist de segurança", "passo a passo de proteção".
---

# Hardening Passo a Passo

## Fluxo

1. Pergunte: qual sistema? (Windows, macOS, Linux, Android, iOS, navegador, rede)
2. Entregue checklist numerada organizada por prioridade

## Formato

Organize em 3 níveis de prioridade:

```
🔒 HARDENING: [Sistema]

🔴 CRÍTICO (faça agora):
1. [passo] — [por que é importante]
2. ...

🟡 RECOMENDADO (faça esta semana):
1. [passo] — [benefício]
2. ...

🟢 AVANÇADO (para quem quer ir além):
1. [passo] — [trade-off]
2. ...

⏱️ Tempo estimado: [X minutos para crítico, Y para recomendado]
```

## Sistemas Cobertos

### Windows
- Crítico: Windows Update, BitLocker, Windows Hello/PIN, firewall ativo, remover bloatware
- Recomendado: desativar telemetria (O&O ShutUp10), DNS criptografado, Portmaster/simplewall
- Avançado: LAPS, AppLocker, Credential Guard, conta sem admin para uso diário

### macOS
- Crítico: FileVault, Gatekeeper, firewall nativo, atualizações automáticas
- Recomendado: Little Snitch/LuLu, DNS criptografado, desativar Siri/telemetria
- Avançado: full-disk encryption via Terminal, audit logs, Lockdown Mode

### Linux
- Crítico: LUKS, firewall (ufw/nftables), atualizações, sudo sem root
- Recomendado: AppArmor/SELinux, fail2ban, DNS criptografado, auditd
- Avançado: Secure Boot, AIDE/Tripwire, sandboxing (Firejail/Bubblewrap), kernel hardening

### Android
- Crítico: tela de bloqueio forte, criptografia ativa, atualizações, revisar permissões
- Recomendado: GrapheneOS/CalyxOS, F-Droid, DNS privado, desativar localização desnecessária
- Avançado: NetGuard/RethinkDNS, Shelter (perfil de trabalho), teclado seguro (HeliBoard), Orbot

### iOS
- Crítico: Face ID/Touch ID, atualizações, Find My, revisar permissões de apps
- Recomendado: Lockdown Mode, Safari hardened, desativar tracking de anúncios, iCloud+
- Avançado: Lockdown Privacy, DNS criptografado via perfil, AdGuard Pro

### Navegador (Firefox)
- Crítico: HTTPS-Only, uBlock Origin, senha mestre, limpar dados ao sair
- Recomendado: Arkenfox user.js, containers, DNS over HTTPS, desabilitar WebRTC
- Avançado: about:config manual, NoScript, Canvas/Font fingerprint protection

### Rede/Roteador
- Crítico: WPA3, senha forte do admin, firmware atualizado, desativar WPS
- Recomendado: Pi-hole/AdGuard Home, DNS criptografado no roteador, guest network
- Avançado: OpenWrt/pfSense, VLAN para IoT, IDS/IPS, segmentação de rede
