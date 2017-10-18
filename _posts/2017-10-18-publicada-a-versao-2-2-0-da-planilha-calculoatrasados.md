---
title: Publicada a versão 2.2.0 da planilha CalculoAtrasados
timestamp: 18/10/2017 00:05:42
categories:
  - atualizações
---

**Correção de bugs**
+ alterado intervalo `EquivalenciaArt58` na página `BeneficioDevido` para assegurar que a precisão fique idêntica à da fórmula customizada de cálculo de benefícios pagos, isto é, duas casas decimais, com arredondamento para baixo
+ alterada fórmula da coluna `FatorReajuste` na página `Evolucao` para que converter "zeros" em "uns", pois de outro modo os benefícios sujeitos ao art. 58 do ADCT ficavam sempre com renda zero, elevada ao mínimo

**Aprimoramentos**
+ introduzido novo aviso e novas regras de formatação condicional na página `BeneficiosPagos` para alertar o usuário sobre a necessidade de fornecer a equivalência salarial em caso de DIB anterior a 06/10/1988  