---
title: Publicada a versão 4.2.1 da planilha CalculoRMI
timestamp: 26/05/2018 19:37:58
categories:
  - atualizações
---

**Correção de bugs**
+ Alterada fórmula do intervalo `BaseIndiceTeto` para observar os valores `MediaComFatorPrevidenciario`e `MediaSemFatorPrevidenciario` em vez do próprio valor do `SalarioBeneficio` (resolve [issue#5](https://github.com/Contadoria/CalculoRMI/issues/5))
+ Corrigida condição de verificação da limitação aos 12 últimos salários de contribuição para auxílio-doença no `DemonstrativoNovo`
