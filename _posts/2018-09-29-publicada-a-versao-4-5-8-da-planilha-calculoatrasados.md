---
title: Publicada a versão 4.5.8 da planilha CalculoAtrasados
timestamp: 29/09/2018 17:05:43
categories:
  - atualizações
---

** Correção de bugs **
+ Inserida condição no intervalo `LimitacaoCalculoAbono` para corrigir o valor quando o último mês das diferenças é igual a dezembro.
+ alterada fórmula do intervalo `Abono` para corrigir o valor quando há `Adicional25` e o último mês das diferenças é proporcional.
+ Criado intervalo `DataInicioIPCAEInformada` e redefinido o intervalo `DataInicioIPCAE` para ajustar corretamente o índice quando `CompetenciaInicial` é posterior à `DataInicioIPCAE`.
