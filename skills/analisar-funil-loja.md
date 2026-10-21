# Skill — analisar_funil_loja

## Objetivo
Diagnosticar em qual etapa do funil da loja a conversão está se perdendo.

## Entrada
Sessões, PDP views, ATC, IC, compras, taxa por etapa, período e mudanças recentes.

## Processo
1. Calcular taxas entre etapas.
2. Comparar com histórico da própria loja.
3. Identificar maior queda relativa.
4. Separar hipótese de confirmação.
5. Relacionar etapa com possíveis causas.

## Heurísticas
- Sessão alta + PDP/ATC fraco → oferta/produto/página
- ATC bom + IC fraco → carrinho/frete/fricção
- IC bom + compra fraca → checkout/preço/pagamento/confiança

## Saída
Etapa crítica, evidência, 3 hipóteses priorizadas, ação, responsável, KPI.
