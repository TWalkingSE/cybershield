# Política de Segurança

## Sobre este projeto

O CyberShield é um conjunto de instruções, skills e base de conhecimento para
configurar IDEs com modo agente como consultor de segurança digital. **Este
repositório não contém software executável** — não há binários, serviços, APIs
ou dependências instaláveis que processem dados de usuários.

Ainda assim, como é um projeto dedicado à segurança digital, levamos a sério
qualquer problema que possa comprometer a qualidade das recomendações,
induzir usuários a práticas inseguras ou expor informações sensíveis.

## Escopo de relatos

Aceitamos relatos para as seguintes categorias:

1. **Recomendações inseguras ou desatualizadas** — ferramenta catalogada com
   histórico de incidente não sinalizado, link oficial incorreto apontando para
   domínio hostil/typosquatting, orientação que reduz a segurança do usuário.
2. **Injeção de instruções maliciosas** — conteúdo em skills ou base de
   conhecimento que possa levar um agente de IA a gerar saídas prejudiciais
   (prompt injection, exfiltração, bypass de guardrails).
3. **Informação sensível vazada** — caso alguma contribuição tenha incluído
   por engano segredos, dados pessoais, tokens ou credenciais.
4. **Uso indevido da marca/identidade** — distribuição de versões modificadas
   que se passem pelo projeto original.

Problemas fora desse escopo (ex.: bugs de formatação, erros de português,
sugestões de novas ferramentas) devem ser abertos como **issues públicas
normais**.

## Como reportar

**Preferido:** use o canal privado do GitHub em
[**Security → Report a vulnerability**](https://github.com/TWalkingSE/cybershield/security/advisories/new)
(GitHub Security Advisories). Isso mantém o relato privado até a correção.

**Alternativa:** se não tiver conta no GitHub, abra uma issue pública
**sem detalhes sensíveis** pedindo um canal privado de contato.

### O que incluir no relato

- Descrição clara do problema e categoria (ver escopo acima).
- Caminho do arquivo afetado (ex.: `.github/skills/cybershield-kb/references/...`).
- Evidências: links, commits, capturas de tela, CVEs, auditorias.
- Impacto estimado (quem é afetado, em qual cenário).
- Sugestão de correção, se tiver.

### O que **não** incluir em issue pública

- Detalhes que permitam explorar o problema antes da correção.
- Dados pessoais de terceiros.
- Credenciais ou segredos.

## Tempo de resposta

Este é um projeto mantido em tempo livre. Compromissos:

| Etapa | Prazo alvo |
|---|---|
| Confirmação de recebimento | até **7 dias** |
| Primeira avaliação / triagem | até **30 dias** |
| Correção ou resposta definitiva | depende da complexidade; atualizamos periodicamente no advisory |

## Divulgação responsável

- Não divulgue publicamente até que a correção esteja publicada, a menos que
  o problema já seja conhecido e explorado ativamente.
- Após a correção, o advisory é publicado com crédito ao relator (se desejado).

## Boas práticas ao usar o projeto

- **Não copie cegamente** as recomendações. Verifique os links oficiais,
  políticas atualizadas e alertas de incidentes antes de adotar qualquer
  ferramenta — a própria base de conhecimento recomenda isso.
- **Mantenha a IDE e os agentes atualizados** — instruções se tornam mais
  eficazes com modelos e IDEs recentes.
- **Considere seu threat model** — o projeto aplica proporcionalidade; nem
  toda recomendação cabe a todos os perfis.

---

*Privacidade não é ter algo a esconder — é um direito fundamental.*
