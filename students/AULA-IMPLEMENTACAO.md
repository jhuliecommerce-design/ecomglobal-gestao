# Aula — Implementando o Escritório EcomGlobal no Habblaud

Objetivo da aula:
fazer o mentorado sair da aula com o **Escritório EcomGlobal funcionando no Habblaud**, com a **Isaura** como porta de entrada, os squads conectados e o ScrollStash disponível para mineração DTC.

---

# PARTE 1 — O QUE O ALUNO PRECISA

- computador
- Git instalado
- conta GitHub
- Claude Code, Codex ou os dois
- Docker
- conta gratuita ScrollStash
- link deste repositório:
  `https://github.com/jhuliecommerce-design/ecomglobal-gestao`

---

# PARTE 2 — INSTALAR O HABBLAUD

Site:
`https://habblaud.com/`

Siga o prompt oficial de instalação mostrado no site.

Depois abra:
`https://habblaud.localhost`

Alternativa:
`http://localhost:4747`

---

# PARTE 3 — CLONAR O ESCRITÓRIO ECOMGLOBAL

```bash
git clone https://github.com/jhuliecommerce-design/ecomglobal-gestao.git
cd ecomglobal-gestao
```

Abrir com:

Claude:
```bash
claude
```

ou Codex:
```bash
codex
```

---

# PARTE 4 — CONECTAR O SCROLLSTASH VIA MCP

MCP:
`https://mcp.scrollstash.com/mcp`

## Claude Code

```bash
claude mcp add --transport http scrollstash https://mcp.scrollstash.com/mcp
```

Depois, no Claude:

```
/mcp
```

Faça login pelo navegador.

Verificar:

```bash
claude mcp list
```

## Codex

```bash
codex mcp add scrollstash --url https://mcp.scrollstash.com/mcp
```

Verificar:

```bash
codex mcp list
```

Concluir o fluxo de autenticação apresentado pelo cliente quando solicitado.

---

# PARTE 5 — CARREGAR O DNA ECOMGLOBAL

Arquivos fundamentais:

- `core/BASE_INSTRUCTIONS.md`
- `core/ROUTER.md`
- `knowledge/dna-ecomglobal/identidade.md`
- `knowledge/dna-ecomglobal/glossario-campanhas.md`
- `agents/REGISTRY.md`
- `agents/gestao/14-auditor-saude-operacao.md`

---

# PARTE 6 — ISAURA

Isaura é a COO do Escritório EcomGlobal e o primeiro contato.

Ela:
- identifica gargalo
- encaminha squad
- usa linguagem da comunidade
- cita estruturas da Jhulie
- aciona o Minerador DTC quando a demanda for pesquisa de mercado/concorrentes

---

# PARTE 7 — SQUADS

## Squad Loja
01–04

## Squad Fornecedores
05–08

## Squad dos Fazedores
09–12

## Squad Processos & Gestão
13–16

## Squad Criativos & DTC
17 Especialista em Advertorial
18 Estrategista DTC
19 Produtor de Vídeo
20 Diretor Criativo
21 Minerador DTC · ScrollStash

---

# PARTE 8 — TESTE DO SCROLLSTASH

Prompt:

"Isaura, quero minerar DTC no nicho de sono e relaxamento nos EUA. Acione o Minerador DTC, encontre marcas relevantes, ângulos, landers e tipos de funil que merecem aprofundamento."

Esperado:
- descoberta de marcas
- análise observacional
- landers
- hooks/ângulos
- funis
- deixar claro que atividade observada não prova ROAS/CPA
- entregar hipóteses para modelagem

---

# PARTE 9 — RESULTADO DA AULA

O aluno termina com:
- Habblaud instalado
- Escritório EcomGlobal aberto
- Git clonado
- Isaura ativa
- squads carregados
- ScrollStash conectado por MCP
- primeira mineração DTC executada
- material enviado para Advertorial/Criativos
