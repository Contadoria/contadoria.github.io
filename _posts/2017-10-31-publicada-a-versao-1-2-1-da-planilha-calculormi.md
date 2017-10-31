---
title: Publicada a versão 1.2.1 da planilha CalculoRMI
timestamp: 31/10/2017 17:49:11
categories:
  - atualizações
---

**Correção de bugs**:
+ Criadas, na página `ParametrosRMI` as variáveis `MenorSalarioNoPC`, `NumeroSalariosExcedentes` e `CompetenciaLimiteMenorSalario` para auxiliar na seleção de salários na coluna `SalarioUtilizado`
+ Alterada variável `PCMaximo` para `PCNormal`, para refletir melhor o seu conceito 
+ Alterada a fórmula na coluna `SalarioUtilizado` para assegurar que, na hipótese de o menor salário corresponder aos salários de mais de uma competência, serão excluídos os salários que excederem o `PCConsiderado`