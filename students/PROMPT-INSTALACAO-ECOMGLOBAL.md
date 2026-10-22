# PROMPT-INSTALACAO-ECOMGLOBAL

Copie e cole este prompt no **Claude Code** ou no **Codex**.

---

Quero que você configure para mim o **Escritório EcomGlobal** usando o Habblaud e este repositório:

`https://github.com/jhuliecommerce-design/ecomglobal-gestao`

## Objetivo final

Quero terminar com:

1. Habblaud instalado e funcionando localmente.
2. Repositório EcomGlobal clonado.
3. Projeto aberto dentro do Habblaud.
4. Isaura configurada como COO e porta de entrada.
5. Todos os squads disponíveis:
   - Squad Loja
   - Squad Fornecedores
   - Squad dos Fazedores
   - Squad Processos & Gestão
   - Squad Criativos & DTC
6. DNA EcomGlobal carregado.
7. Base de conhecimento, skills e agentes acessíveis.
8. Configuração compatível com **Claude Code e Codex**.
9. Testes iniciais executados.

## Regras importantes

- Não altere o conteúdo do método EcomGlobal.
- Não renomeie squads, agentes ou estruturas internas.
- Não substitua as instruções por recomendações genéricas.
- Preserve os arquivos Markdown como fonte principal de instrução.
- Se uma integração específica de Claude ou Codex exigir um adaptador, crie apenas o adaptador necessário, sem duplicar ou alterar a lógica central.
- Toda configuração específica de provider deve ficar separada da base compartilhada.

## Passo 1 — Instalar Habblaud

Use a documentação oficial do Habblaud para instalar e iniciar o ambiente.

Site oficial:
`https://habblaud.com/`

Repositório oficial:
`https://github.com/marmottajr/habblaud`

Confirme que o escritório abre localmente.

## Passo 2 — Clonar o EcomGlobal

Clone:

```bash
git clone https://github.com/jhuliecommerce-design/ecomglobal-gestao.git
cd ecomglobal-gestao
```

## Passo 3 — Carregar a base compartilhada

A base comum a todos os agentes é:

- `core/BASE_INSTRUCTIONS.md`
- `core/ROUTER.md`
- `knowledge/dna-ecomglobal/identidade.md`
- `knowledge/dna-ecomglobal/glossario-campanhas.md`
- `agents/REGISTRY.md`

## Passo 4 — Configurar Isaura

Use:

- `agents/gestao/14-auditor-saude-operacao.md`
- `knowledge/performance/arvore-decisao-funil.md`
- `skills/analisar-funil-loja.md`

A Isaura deve:
- receber o mentorado primeiro
- identificar o gargalo
- chamar o squad correto
- falar com DNA EcomGlobal
- citar estruturas da Jhulie quando registradas
- não inventar parâmetros ausentes

## Passo 5 — Configurar os squads

Cada agente deve combinar:

1. `core/BASE_INSTRUCTIONS.md`
2. arquivo individual em `agents/`
3. skills listadas pelo agente
4. knowledge relevante
5. schemas quando necessário

## Passo 6 — Compatibilidade Claude + Codex

Crie a configuração de forma **provider-agnostic**.

### Base compartilhada
Todo conteúdo de comportamento, método, skill e conhecimento deve continuar em Markdown neste repositório.

### Claude Code
Crie somente os arquivos/adaptadores que o Claude Code precisar para carregar a base.

### Codex
Crie somente os arquivos/adaptadores que o Codex precisar para carregar a mesma base.

### Regra
Claude e Codex devem ler a **mesma fonte de verdade**.

Não mantenha duas versões diferentes do cérebro do agente.

## Passo 7 — Testar

Execute estes testes:

### Teste 1
"Isaura, meu CPC está bom e estou tendo clique, mas quase ninguém adiciona ao carrinho."

Esperado:
- localizar PDP → ATC
- não recomendar aumento de budget
- chamar Squad Loja
- apontar Fator A

### Teste 2
"Tenho uma CBO validada e quero lateralizar sem mexer na base."

Esperado:
- preservar base
- usar linguagem EcomGlobal
- consultar glossário de campanhas

### Teste 3
"Minha PMax tem ROAS alto, mas não gasta todo o orçamento."

Esperado:
- não aumentar budget automaticamente
- diagnosticar restrição
- considerar lateralização

### Teste 4
"Minha equipe me chama para decidir tudo."

Esperado:
- identificar falha de processo/autonomia
- chamar Gestor de Equipe e Gestor de Processos

## Passo 8 — Entrega final

Ao terminar, me mostre:

1. Habblaud funcionando
2. caminho local do projeto
3. Isaura ativa
4. squads configurados
5. quais adaptadores foram criados para Claude
6. quais adaptadores foram criados para Codex
7. resultado dos testes
8. qualquer etapa que ainda exija ação manual

Não finalize enquanto não verificar os itens acima.
