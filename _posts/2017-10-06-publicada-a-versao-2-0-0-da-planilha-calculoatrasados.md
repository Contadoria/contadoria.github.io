---
title: Publicada a versão 2.0.0 da planilha CalculoAtrasados
timestamp: 06/10/2017 01:44:10
categories:
  - atualizações
---

**Alterações estruturais**
+ reformulação de toda a sistemática de cômputo de benefícios recebidos, com a eliminação da página `BeneficioPago` e criação da página `BeneficiosPagos`.
  Agora é possível evoluir o valor de um benefício revisto e de até cinco outros benefícios pagos pelo INSS seguindo os mesmos critérios utilizados administrativamente pela autarquia.
  O cálculo dos benefícios pagos é agora feito por meio de uma fórmula customizada, em Javascript, o que melhora o desempenho da planilha.
  A nova estrutura torna também possível fazer a evolução de benefícios a partir da inserção de dados do CONBAS, por meio da ferramenta de preenchimento automático do complemento **Cálculos Previdenciários**.

**Aprimoramentos**
+ em razão da recente decisão do STF quanto à correção dos débitos judiciais, foram incluídos o IPCA e o IPCAE na página `IndicesConsolidados`, o que permitirá a utilização imediata desses índices para cálculo de atrasados.
  Por ora, diante da incerteza quanto ao índice a ser adotado e os critérios de aplicação, os valores deverão ser inseridos por meio dos modificadores, o que pode ser feito de modo automático pelo uso de fórmulas.

**Correção de bugs**
+ nenhum desta vez