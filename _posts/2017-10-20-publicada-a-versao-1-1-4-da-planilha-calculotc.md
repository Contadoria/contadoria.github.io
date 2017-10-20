---
title: Publicada a versão 1.1.4 da planilha CalculoTC
timestamp: 20/10/2017 18:22:18
categories:
  - atualizações
---

**Correção de bugs**
+ inserida na função customizada `jef_ELIMINAR_CONCOMITANCIA`, a hipótese em que, havendo conflito entre dois períodos, (i) o segundo tem peso maior; (ii) as datas iniciais são iguais; e (iii) a data final do primeiro é posterior à do segundo. Sem essa previsão, a função resultava em "loop infinito" quando presente a hipótese em análise, pois a concomitância entre os dois períodos nunca era eliminada.