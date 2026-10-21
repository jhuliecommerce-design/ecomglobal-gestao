# Skill — analisar_funil_loja

## Objetivo
Diagnosticar **onde a operação perde dinheiro depois do clique** e transformar a queda do funil em uma decisão concreta de página, oferta, carrinho ou checkout.

Esta skill não deve responder apenas "a página está ruim". Ela deve localizar a etapa, levantar hipóteses, dizer **o que conferir primeiro** e qual alteração merece teste.

---

## Funil analisado

TRÁFEGO
→ CLIQUE
→ PÁGINA DE PRODUTO
→ ADD TO CART
→ INITIATE CHECKOUT
→ COMPRA

Quando houver advertorial/quiz:

ANÚNCIO
→ ADVERTORIAL / QUIZ
→ PÁGINA DE PRODUTO
→ ATC
→ IC
→ COMPRA

---

## Entradas mínimas

### Mídia
- Plataforma
- Campanha
- Gasto
- Impressões
- Cliques
- CPC
- CTR quando disponível
- Compras atribuídas
- CPA
- ROAS

### Loja
- Sessões
- Visualizações de página de produto
- AddToCart
- InitiateCheckout
- Compras
- Taxa de conversão
- Ticket médio

### Contexto
- Produto
- Oferta
- Página usada
- Mercado
- Dispositivo dominante
- Frete
- Meios de pagamento
- Mudanças recentes
- Período comparado

---

## Regra principal

**Métrica boa antes de uma etapa + queda forte depois dela = investigar a próxima etapa do funil.**

Não assumir automaticamente que o anúncio é o problema quando o anúncio já está entregando clique qualificado.

---

# ÁRVORE DE DIAGNÓSTICO

## CENÁRIO A — CPC BOM + CTR BOM + POUCO/SEM ATC

### Interpretação
O anúncio consegue gerar interesse e clique, mas a página não transforma interesse em intenção de compra.

### Investigar primeiro
1. A página entrega exatamente o que o anúncio prometeu?
2. O produto/benefício fica claro nos primeiros segundos?
3. A oferta aparece cedo o suficiente?
4. Preço e desconto fazem sentido?
5. Existe demonstração clara do produto?
6. Existe prova suficiente?
7. A página está lenta ou ruim no mobile?
8. Existe informação demais antes da proposta de valor?
9. O cliente entende por que comprar agora?
10. A variante/tamanho/cor está clara?

### Blocos que podem estar faltando na página
- Benefício principal acima da dobra
- Antes/depois legítimo quando aplicável e permitido
- Demonstração de uso
- Benefícios em linguagem simples
- Comparação com alternativa comum
- Provas/reviews reais
- FAQ de objeções
- Garantia/política clara
- Oferta em kits
- Desconto por quantidade
- Frete/prazo visível
- CTA mais claro
- Urgência real
- Explicação do mecanismo
- Conteúdo específico para mobile

### Próxima ação
Priorizar **1–3 hipóteses de maior impacto**, não redesenhar toda a página de uma vez.

---

## CENÁRIO B — ATC BOM + POUCO INITIATE CHECKOUT

### Interpretação
O cliente gostou o suficiente para adicionar ao carrinho, mas encontrou fricção antes de iniciar checkout.

### Investigar
- Carrinho lateral ou página de carrinho quebrada
- Frete aparece tarde ou fica caro
- Taxas inesperadas
- Cupom que gera distração
- Upsell atrapalhando
- Botão de checkout pouco evidente
- Variant selector errado
- Quantidade/preço mudando
- Produto indisponível
- Redirecionamento lento
- Moeda incoerente
- Carrinho mobile ruim

### Testes
- Simplificar carrinho
- Evidenciar botão de checkout
- Mostrar estimativa de frete antes
- Remover distrações
- Corrigir moeda/preço
- Conferir scripts/apps que bloqueiam avanço

---

## CENÁRIO C — INITIATE CHECKOUT BOM + POUCAS COMPRAS

### Interpretação
Existe intenção forte. O gargalo está próximo da transação.

### Investigar primeiro
1. Meios de pagamento disponíveis no país
2. Cartões locais / carteiras
3. Erros de pagamento
4. Checkout recusando endereço
5. Frete final inesperado
6. Prazo de entrega
7. Taxas adicionais
8. Conversão de moeda
9. Confiança no checkout
10. Página/checkout carregando mal
11. Falha técnica no botão/pagamento
12. Compra acontecendo mas tracking não registra

### Diferenciar
**problema real de compra** vs **problema de tracking**.

Conferir:
Shopify / gateway / plataforma de mídia / tracking externo.

---

## CENÁRIO D — MUITOS CLIQUES + CPC BOM + FUNIL TODO FRACO

### Possibilidades
- Criativo gera curiosidade, não intenção
- Promessa e página não combinam
- Público amplo demais
- Oferta pouco competitiva
- Produto não encaixa no mercado
- Tráfego acidental/baixa qualidade

### Ação
Não culpar página automaticamente. Comparar:
- taxa de scroll
- tempo/sessão quando disponível
- ATC
- comportamento por dispositivo
- campanha/público/criativo

---

## CENÁRIO E — ATC E IC BONS + COMPRA CAI DE REPENTE

### Possibilidades prioritárias
- Gateway
- Shopify Payments / provedor
- Frete
- Erro de checkout
- País/moeda
- app/script
- tracking
- estoque/variante

### Ação
Tratar primeiro como **incidente operacional**, não como problema de copy.

---

## CENÁRIO F — CLIQUE PIOROU ANTES DO RESTO DO FUNIL

Quando CPC sobe / taxa de clique cai / entrega deteriora **antes** da página:
- revisar criativo
- hook
- ângulo
- público
- fadiga
- posicionamento
- oferta anunciada

Não fazer CRO de página para corrigir problema que nasceu no anúncio.

---

# ANÁLISE DA PÁGINA DE PRODUTO

A skill deve avaliar a página por blocos.

## 1. Primeira dobra
- Produto identificável?
- Dor/benefício claro?
- Preço visível?
- CTA visível?
- Oferta compreensível?
- Visual transmite confiança?

## 2. Oferta
- Compra única?
- Kit?
- desconto por quantidade?
- assinatura quando aplicável?
- preço âncora?
- economia clara?
- motivo para escolher um pacote?

## 3. Demonstração
- Mostra uso?
- Mostra aplicação?
- Mostra tamanho/escala?
- Mostra transformação de forma legítima?
- Vídeo suficiente?

## 4. Prova
- Reviews reais
- Fotos reais
- UGC real/licenciado
- dados verificáveis
- depoimentos autênticos
- prova compatível com a promessa

## 5. Objeções
A página responde:
- funciona para mim?
- quanto tempo?
- como usar?
- o que vem?
- tamanho?
- material?
- risco?
- devolução?
- prazo?
- garantia?

## 6. Segurança
- contato
- política clara
- checkout reconhecível
- pagamento
- devolução
- identidade da marca
- erros visuais/ortográficos
- coerência de moeda

## 7. Mobile
Sempre analisar separadamente:
- velocidade
- tamanho dos botões
- sticky ATC
- imagens
- texto
- popups
- seletor de variantes
- carrinho

---

# PRIORIZAÇÃO DE TESTE

Classificar cada hipótese:

**IMPACTO ALTO / ESFORÇO BAIXO**
→ testar primeiro

**IMPACTO ALTO / ESFORÇO ALTO**
→ planejar

**IMPACTO BAIXO**
→ não priorizar enquanto houver gargalo maior

---

# Saída obrigatória

## 1. ETAPA DO FUNIL COM PROBLEMA
Ex.: Página de Produto → ATC

## 2. EVIDÊNCIA
Ex.: CPC e CTR saudáveis, mas ATC caiu 42% vs histórico.

## 3. HIPÓTESES PRIORIZADAS
1.
2.
3.

## 4. O QUE CONFERIR AGORA
Checklist curto.

## 5. TESTE RECOMENDADO
Uma mudança principal ou pacote coerente.

## 6. RESPONSÁVEL
Loja / CRO / tráfego / pagamentos / fornecedor.

## 7. PRAZO
Quando implementar.

## 8. KPI
Qual número precisa reagir.

## 9. PRÓXIMA DECISÃO
O que fazer se melhorar / se não melhorar.

## Regra final
Nunca concluir "é a página" apenas porque não houve compra. Localizar a queda no funil primeiro.
