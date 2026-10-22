# Aula — Mineração DTC com ScrollStash via MCP

## Objetivo
Fazer o aluno conectar o ScrollStash ao Claude Code e/ou Codex e sair minerando marcas DTC, criativos e funis em linguagem natural.

MCP:
`https://mcp.scrollstash.com/mcp`

O login é feito pelo navegador com conta gratuita ScrollStash. Não é necessário colar API key.

---

# CLAUDE CODE

No terminal:

```bash
claude mcp add --transport http scrollstash https://mcp.scrollstash.com/mcp
```

Depois abra o Claude Code e rode:

```
/mcp
```

Faça login no navegador quando solicitado.

Para deixar disponível em todos os projetos, use escopo de usuário conforme a CLI instalada.

Verificar:

```bash
claude mcp list
```

---

# CODEX

No terminal:

```bash
codex mcp add scrollstash --url https://mcp.scrollstash.com/mcp
```

Verificar:

```bash
codex mcp list
```

Se o servidor exigir autenticação, concluir o fluxo de login/autorização apresentado pelo cliente.

---

# PRIMEIROS PROMPTS

## 1. Descobrir marcas
"Encontre marcas DTC de health & beauty relacionadas a sono, relaxamento e qualidade de vida. Priorize marcas com atividade recente observada."

## 2. Analisar marca
"Analise a estratégia observada de anúncios da marca X: formatos, CTAs, landers e tipos de funil."

## 3. Minerar funil
"Mostre as principais páginas de destino observadas da marca X e classifique quais parecem PDP, landing page, quiz ou advertorial."

## 4. Minerar ângulos
"Pesquise os anúncios da marca X e organize os hooks, dores, promessas e CTAs recorrentes."

## 5. Comparar concorrentes
"Compare X e Y em formatos de anúncio, CTAs, landers e profundidade de funil."

## 6. Descobrir unknown players
"Encontre anunciantes de skincare com quiz, onboarding ou funil de landing page."

---

# COMO USAR NA METODOLOGIA ECOMGLOBAL

## MINERAÇÃO
ScrollStash
↓
marca
↓
produto
↓
anúncios
↓
lander
↓
dor
↓
ângulo

## MODELAGEM
Minerador DTC
↓
Especialista em Advertorial
↓
Estrategista de Criativos
↓
Produtor de Vídeo

---

# LEITURA CORRETA DOS DADOS

ScrollStash é uma ferramenta de inteligência de anúncios e landers.

Não afirmar que:
- marca é lucrativa porque possui muitos anúncios
- anúncio é vencedor porque ficou ativo por muito tempo
- marca gastou mais porque possui mais anúncios
- lander converte melhor porque aparece mais vezes

Esses sinais servem para **priorizar o que merece mineração**.

---

# EXERCÍCIO DA AULA

Cada aluno deve sair com:

1. 1 categoria DTC escolhida
2. 10 marcas encontradas
3. 3 marcas aprofundadas
4. 10 ângulos mapeados
5. 5 landers salvas
6. 1 advertorial escolhido para modelagem
7. 10 ideias de criativo
8. 3 hipóteses de oferta

Depois encaminhar o material para os agentes 17, 18, 19 e 20.
