# EcomGlobal Gestão — Escritório de IA

Repositório entregue aos alunos da Mentoria EcomGlobal para montar um escritório operacional com **21 agentes de IA**, divididos em squads e apoiados por skills, MCPs e base de conhecimento própria.

## O que existe aqui

### Squad 01 — Loja
1. Gestor de Loja
2. Produto, SEO & Precificação
3. Tema & CRO
4. Compliance & Políticas

### Squad 02 — Fornecedores
5. Gestor de Fornecedores
6. Gestor de Cotações
7. Devoluções & Problemas
8. Logística & Redundância

### Squad 03 — Fazedores
9. Gestor Meta Ads
10. Gestor Google Ads
11. Analista Multicanal
12. Gestor de Escala & Capital

### Squad 04 — Processos & Gestão
13. Gestor de Processos
14. Isaura — COO EcomGlobal
15. Gestor de Equipe
16. Gestor de Expansão

### Squad 05 — Criativos & DTC
17. Especialista em Advertorial
18. Estrategista de Criativos DTC
19. Produtor de Vídeo
20. Diretor Criativo de Performance
21. Minerador DTC · ScrollStash

## Estrutura

```
agents/       → os 21 agentes
skills/       → funções reutilizáveis
knowledge/    → método EcomGlobal
schemas/      → estrutura de dados
core/         → instruções compartilhadas e roteamento
students/     → guias de implementação
```

## MCPs usados na aula

### ScrollStash
`https://mcp.scrollstash.com/mcp`

Usado para mineração DTC, marcas, anúncios, criativos, landers e funis observados.

## Como um agente deve funcionar

Cada agente possui:
- missão
- entradas
- processo
- regras de decisão
- skills
- limites
- formato de saída

### Saída operacional padrão
1. Situação
2. Diagnóstico
3. Prioridade
4. Ação
5. Responsável
6. Prazo
7. KPI de validação
8. Próxima decisão

## Regra central

Os agentes devem usar primeiro a base em `knowledge/`. Estruturas da Mentoria EcomGlobal têm prioridade sobre recomendações genéricas.

## Primeiros arquivos para ler

- `students/QUICKSTART.md`
- `students/AULA-IMPLEMENTACAO.md`
- `students/SCROLLSTASH-MCP.md`
- `core/BASE_INSTRUCTIONS.md`
- `core/ROUTER.md`
- `agents/REGISTRY.md`

## Objetivo

Transformar gestão de e-commerce em sistema: **responsável + resultado + KPI + prazo + próxima decisão**.
