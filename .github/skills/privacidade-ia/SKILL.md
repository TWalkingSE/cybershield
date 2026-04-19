---
name: privacidade-ia
description: >
  Proteção de dados pessoais ao usar ferramentas de IA e LLMs. Use quando o 
  usuário perguntar sobre privacidade em ChatGPT, Gemini, Copilot, Claude, 
  Midjourney, ou qualquer IA generativa. Também use para: "é seguro usar IA?", 
  "a IA salva meus dados?", "como usar IA sem vazar dados", "LLM local", 
  "Ollama", "LM Studio", "IA privada", ou qualquer preocupação sobre dados 
  em serviços de IA na nuvem.
---

# Privacidade em IA / LLMs

## Camada TCP/IP
[Camada 4 — Aplicação] — Ferramentas de IA são aplicações que processam dados via APIs cloud.

## Riscos Principais

1. **Dados usados para treinamento**: muitos serviços usam conversas para treinar modelos (verificar opt-out)
2. **Acesso por funcionários**: equipes de revisão podem ler conversas para qualidade/segurança
3. **Metadados**: horários, frequência, IP, dispositivo — rastreáveis mesmo sem ler conteúdo
4. **Vazamento em prompts**: dados sensíveis inseridos em prompts podem persistir no sistema
5. **Integração com ecossistema**: plugins/extensões podem enviar dados para terceiros

## Recomendações por Nível

### Básico (uso casual)
- DuckDuckGo AI Chat — sem login, sem associação a conta, modelos rotativos
- Brave Leo — processamento local quando possível, sem envio de dados de navegação
- Desativar histórico de conversas quando disponível

### Intermediário (uso profissional)
- API com opt-out de treinamento (OpenAI API, Anthropic API — verificar termos atuais)
- Ferramentas com política de zero retenção de dados
- Usar contas separadas (compartimentalização) para IA
- Nunca inserir dados pessoais, códigos proprietários, ou informações confidenciais

### Avançado (dados sensíveis)
- **LLMs locais** — processamento 100% no dispositivo:
  - Ollama — interface CLI, modelos open-source, fácil de configurar
  - LM Studio — interface gráfica, download de modelos, totalmente offline
  - Jan — interface similar a ChatGPT, 100% local
  - GPT4All — leve, roda em hardware modesto
- Anti-stylometry: CamoCopy (ofuscar estilo de escrita quando necessário)
- Containers/VMs dedicadas para interações com IA cloud

## OPSEC com IA (Regras de Ouro)

1. **Nunca** insira dados pessoais identificáveis em IA cloud
2. **Nunca** cole código proprietário ou segredos de negócio
3. **Nunca** compartilhe credenciais, tokens ou chaves de API
4. **Sempre** verifique a política de dados antes de usar um novo serviço
5. **Sempre** use aliases/dados fictícios quando testar prompts com dados sensíveis
6. **Considere** LLMs locais para qualquer dado que não deveria sair do seu dispositivo
