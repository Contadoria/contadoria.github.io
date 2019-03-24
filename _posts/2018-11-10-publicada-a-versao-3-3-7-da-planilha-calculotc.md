---
title: Publicada a versão 3.3.7 da planilha CalculoTC
timestamp: 10/11/2018 11:02:30
categories:
  - atualizações
---

** Correção de bugs **
+ Quando `AjustarMarcosTemporais`= "Não", os cálculos são realizados com base em todos os registros lançados nas abas `TCDiscriminado` e `TCAdicionado`. Coeficiente de cálculo da aposentadoria por tempo de contribuição deixa de ser calculado, tendo em vista que não é possível verificar o tempo até a Emenda Constitucional nº 20/98 e consequentemente o pedágio necessário. Idade e pontos também deixam de ser calculados por eventuais divergências entre a `DER` informada e a data final do último período lançado (resolve [issue#16]( https://github.com/Contadoria/CalculoTC/issues/16))