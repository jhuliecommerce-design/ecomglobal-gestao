# Compatibilidade — Claude Code + Codex

## Objetivo

Todos os agentes do Escritório EcomGlobal devem funcionar tanto no **Claude Code** quanto no **Codex** sem manter dois cérebros diferentes.

## Arquitetura correta

### Fonte única de verdade

A lógica central fica em:

- `core/`
- `agents/`
- `skills/`
- `knowledge/`
- `schemas/`

Esses arquivos são neutros em relação ao provider.

## O que NÃO deve acontecer

Não criar:

- uma versão de Isaura para Claude
- outra Isaura diferente para Codex
- regras de campanha diferentes por provider
- skills duplicadas

Isso gera divergência operacional.

## O que pode variar

Somente a camada de integração:

- arquivo de instrução inicial
- hook
- comando de startup
- forma de carregar contexto
- configuração de ferramenta

## Regra

**Provider muda. DNA não muda.**

Claude e Codex devem responder com a mesma lógica EcomGlobal quando recebem os mesmos dados.

## Teste de paridade

Rodar a mesma pergunta nos dois:

"Tenho CPC bom, clique bom, ATC ruim. O que você faria?"

Ambos devem:
1. localizar o gargalo pós-clique
2. priorizar PDP/oferta
3. não recomendar aumentar orçamento
4. sugerir Fator A
5. terminar com ação + KPI + próxima decisão

## Quando houver diferença entre providers

Ajustar o adaptador, não a base EcomGlobal.

## Recomendação

Sempre que um novo agente ou skill for criado:
1. adicionar na base compartilhada
2. atualizar registry/router se necessário
3. testar no Claude
4. testar no Codex
5. validar paridade
