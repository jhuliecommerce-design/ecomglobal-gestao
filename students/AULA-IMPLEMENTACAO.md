# Aula — Implementando o Escritório EcomGlobal

Objetivo da aula:
fazer o mentorado sair da aula com o **Escritório EcomGlobal funcionando**, a Isaura como porta de entrada e os squads carregados com a base da mentoria.

## Parte 1 — Preparação
O aluno precisa ter:
- computador
- conta GitHub
- acesso à plataforma de agentes usada na aula
- link deste repositório

## Parte 2 — Baixar/instalar a plataforma
**IMPORTANTE:** o passo a passo exato da plataforma deve ser preenchido a partir da documentação oficial e da versão mostrada na aula.

Não inventar nomes de botões ou menus.

### Checklist do tutorial
1. abrir o link oficial
2. baixar a versão correta
3. instalar
4. fazer login
5. criar o workspace/escritório
6. nomear: **EcomGlobal**
7. importar/conectar este Git
8. carregar instruções-base
9. criar/importar Isaura
10. criar/importar os demais squads
11. testar roteamento

## Parte 3 — Repositório
Repositório:
`jhuliecommerce-design/ecomglobal-gestao`

Arquivos essenciais:
- core/BASE_INSTRUCTIONS.md
- core/ROUTER.md
- knowledge/dna-ecomglobal/
- agents/REGISTRY.md
- agents/gestao/14-auditor-saude-operacao.md

## Parte 4 — Configuração da Isaura
Isaura recebe:
1. BASE_INSTRUCTIONS
2. identidade EcomGlobal
3. glossário de campanhas
4. Router
5. sua própria instrução de COO

## Parte 5 — Teste de funcionamento

### Teste 1
"Isaura, meu CPC está bom e estou tendo clique, mas quase ninguém adiciona ao carrinho. O que você analisaria?"

Esperado:
- não sugerir subir budget
- localizar gargalo PDP→ATC
- acionar Squad Loja
- apontar Fator A

### Teste 2
"Isaura, tenho uma CBO validada e quero lateralizar sem mexer na base."

Esperado:
- usar linguagem da comunidade
- consultar estruturas EcomGlobal
- citar campanha interna se critérios estiverem registrados

### Teste 3
"Minha PMax tem ROAS alto, mas não gasta todo o orçamento."

Esperado:
- não recomendar simplesmente aumentar budget
- diagnosticar lance/volume
- considerar lateralização

## Parte 6 — Regra para alunos
Os agentes não substituem dados.
Quanto melhor o dado enviado, melhor a decisão.

Sempre enviar:
- período
- estrutura
- orçamento
- gasto
- métricas
- mudança recente
- objetivo
