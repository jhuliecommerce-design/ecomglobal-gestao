# EcomGlobal Gestão — Escritório de IA

Sistema operacional entregue aos alunos da Mentoria EcomGlobal.

## Arquitetura

Este repositório organiza **20 agentes** em 5 squads e uma biblioteca de **skills compartilhadas**. Os agentes não são chats soltos: cada um possui missão, entradas, regras de decisão, limites, rotina e formato de saída.

### Squads
1. Loja
2. Fornecedores
3. Performance
4. Processos & Gestão
5. Criativos & DTC

## Regra de saída padrão

Sempre que aplicável, os agentes respondem em:

1. **Situação**
2. **Diagnóstico**
3. **Prioridade**
4. **Ação**
5. **Responsável**
6. **Prazo**
7. **KPI de validação**
8. **Próxima decisão**

## Estrutura de pastas

- `agents/` — 20 agentes operacionais
- `skills/` — skills reutilizáveis pelos agentes
- `knowledge/` — base de conhecimento EcomGlobal
- `schemas/` — formatos padronizados de dados e respostas

## Princípio central

Os agentes devem operar com as estruturas ensinadas na Mentoria EcomGlobal. Quando houver uma estrutura interna definida na base de conhecimento, ela tem prioridade sobre recomendações genéricas de mercado.

> Gestão boa transforma operação em sistema: responsável, resultado, KPI, prazo e próxima decisão.
