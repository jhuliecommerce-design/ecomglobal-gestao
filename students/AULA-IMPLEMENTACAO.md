# Aula — Implementando o Escritório EcomGlobal no Habblaud

Objetivo da aula:
fazer o mentorado sair da aula com o **Escritório EcomGlobal funcionando no Habblaud**, com a **Isaura** como porta de entrada e os squads conectados à base da Mentoria EcomGlobal.

---

# PARTE 1 — O QUE O ALUNO PRECISA

- computador
- Git instalado
- conta GitHub
- Claude Code, Codex ou os dois
- Docker
- link deste repositório:
  `https://github.com/jhuliecommerce-design/ecomglobal-gestao`

O Habblaud é 100% local e organiza sessões de Claude Code e Codex em um escritório visual. Cada projeto vira uma sala e cada sessão aparece como um agente/personagem.

---

# PARTE 2 — INSTALAR O HABBLAUD

## Caminho mais rápido

### 1. Abrir o terminal

Mac:
`⌘ + Espaço → Terminal`

Linux:
`Ctrl + Alt + T`

Windows:
abrir PowerShell. O Habblaud roda via WSL2 no Windows.

### 2. Entrar no agente que o aluno já usa

Claude Code:
```
claude
```

ou Codex:
```
codex
```

### 3. Colar o prompt oficial de instalação

Use o prompt oficial do Habblaud disponível em:
`https://habblaud.com/`

O prompt instala e configura automaticamente:
- Docker quando necessário
- repositório do Habblaud
- dependências
- integração com Claude Code
- integração com Codex
- inicialização automática
- acesso local ao escritório

Repositório oficial do Habblaud:
`https://github.com/marmottajr/habblaud`

### 4. Aprovar permissões solicitadas

O agente pode pedir autorização para:
- Docker
- instalação de pacotes
- `sudo`
- pastas fora do projeto
- hooks
- WSL no Windows

Aprovar somente os passos que aparecem durante a instalação guiada.

### 5. Abrir o escritório

Endereço principal:
`https://habblaud.localhost`

Alternativa:
`http://localhost:4747`

O health check do Habblaud usa:
`http://localhost:4747/api/health`

---

# PARTE 3 — CHECAR SE O HABBLAUD ESTÁ CONECTADO

## Claude Code

Dentro da pasta do Habblaud:

```
cd ~/habblaud
npm run mod:status
```

Deve mostrar o mod e os plugins do Habblaud instalados e ativos.

## Codex

```
cd ~/habblaud
npm run codex:status
```

Se houver hooks novos/alterados, o aluno fecha o Codex, abre novamente, roda:

```
/hooks
```

e aprova os hooks do Habblaud.

---

# PARTE 4 — CRIAR O ESCRITÓRIO ECOMGLOBAL

A proposta da aula é usar o repositório da comunidade como o projeto do escritório.

## 1. Clonar o Git da aula

```
git clone https://github.com/jhuliecommerce-design/ecomglobal-gestao.git
cd ecomglobal-gestao
```

## 2. Abrir o projeto com Claude Code ou Codex

Claude:
```
claude
```

Codex:
```
codex
```

A partir daí, a sessão desse projeto deve aparecer no Habblaud como uma sala.

---

# PARTE 5 — CARREGAR O DNA ECOMGLOBAL

Arquivos fundamentais:

- `core/BASE_INSTRUCTIONS.md`
- `core/ROUTER.md`
- `knowledge/dna-ecomglobal/identidade.md`
- `knowledge/dna-ecomglobal/glossario-campanhas.md`
- `agents/REGISTRY.md`
- `agents/gestao/14-auditor-saude-operacao.md`

A ordem de prioridade é:

1. DNA EcomGlobal
2. estruturas e regras da mentoria
3. dados atuais da operação
4. skills
5. conhecimento geral

---

# PARTE 6 — ISAURA

A Isaura é a **COO do Escritório EcomGlobal**.

Ela é o primeiro contato do mentorado.

## Ela precisa saber

- identificar gargalo
- encaminhar para o squad certo
- usar linguagem da comunidade
- citar estruturas da Jhulie
- nunca trocar o método da mentoria por recomendação genérica

## Arquivos da Isaura

- `agents/gestao/14-auditor-saude-operacao.md`
- `core/BASE_INSTRUCTIONS.md`
- `core/ROUTER.md`
- `knowledge/dna-ecomglobal/`
- `knowledge/performance/arvore-decisao-funil.md`

---

# PARTE 7 — SQUADS

## Squad Loja
01 Gestor de Loja
02 Produto, SEO & Precificação
03 Tema & CRO
04 Compliance & Políticas

## Squad Fornecedores
05 Gestor de Fornecedores
06 Gestor de Cotações
07 Devoluções & Problemas
08 Logística & Redundância

## Squad dos Fazedores
09 Gestor Meta Ads
10 Gestor Google Ads
11 Analista Multicanal
12 Gestor de Escala & Capital

## Squad Processos & Gestão
13 Gestor de Processos
14 Isaura
15 Gestor de Equipe
16 Gestor de Expansão

## Squad Criativos & DTC
17 Especialista em Advertorial
18 Estrategista de Criativos DTC
19 Produtor de Vídeo
20 Diretor Criativo de Performance

---

# PARTE 8 — PRIMEIROS TESTES AO VIVO

## TESTE 01 — FUNIL

Prompt:

"Isaura, meu CPC está bom e os criativos estão trazendo clique, mas quase ninguém adiciona ao carrinho. Faz a leitura da operação."

Esperado:
- não recomendar subir orçamento
- localizar queda PDP → ATC
- acionar Squad Loja
- apontar Fator A
- sugerir KPI para validar a alteração

---

## TESTE 02 — META ADS

Prompt:

"Isaura, tenho uma CBO validada e quero lateralizar sem mexer na base."

Esperado:
- preservar campanha base
- consultar estruturas da comunidade
- falar em CBO da Jhulie / Dopamina quando critérios estiverem registrados
- explicar por que a nova estrutura faz sentido

---

## TESTE 03 — GOOGLE

Prompt:

"Minha PMax tem ROAS alto, mas não está consumindo o orçamento."

Esperado:
- não mandar simplesmente aumentar budget
- investigar meta de ROAS / restrição / volume
- considerar lateralização
- preservar a campanha base

---

## TESTE 04 — GESTÃO

Prompt:

"Isaura, minha equipe está me chamando o dia inteiro para decidir tudo. Quero organizar isso."

Esperado:
- identificar falta de autonomia/processo
- acionar Gestor de Equipe + Gestor de Processos
- montar responsáveis, KPIs, níveis de autonomia e escalonamento

---

# PARTE 9 — REGRA PARA USAR OS AGENTES

Quanto melhor o dado enviado, melhor a decisão.

Sempre que possível informar:

- período
- estrutura
- orçamento
- gasto
- métricas
- mudança recente
- objetivo
- mercado
- página
- margem
- contexto operacional

---

# PARTE 10 — RESULTADO DA AULA

O aluno termina com:

- Habblaud instalado
- escritório local funcionando
- Git EcomGlobal clonado
- Isaura ativa
- squads disponíveis
- DNA EcomGlobal carregado
- primeiros testes concluídos

A aula deve terminar com o aluno usando o escritório em uma operação real.
