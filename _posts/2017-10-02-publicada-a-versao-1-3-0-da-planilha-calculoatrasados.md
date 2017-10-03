---
title: Publicada a versão 1.3.0 da planilha CalculoAtrasados
timestamp: 02/10/2017 21:02:14
categories:
  - atualizações
---

**Correção de bugs**

+ Corrigido bug na coluna `Reajustar` da página `Evolucao`. Não se sabe por que motivo, a fórmula continha a expressão `<>DataBase`. Ou seja, a impressão é que ela inverteria os valores de `VERDADEIRO` e `FALSO` no lugar de simplesmente transpo-los.
  Agora está assim:
  ~~~
  =ARRAYFORMULA(SE(LIN(Reajustar)=1;"Reajustar";SE(LIN(Reajustar)<=TotalCompetencias+1;SE(LIN(Reajustar)=LinhaPrimeiraCompetencia;FALSO();SE(LIN(Reajustar)=LinhaReajusteLei8870;VERDADEIRO();{"";DESLOC(DataBase;LinhaInicialTabelaIndices-1;0;TotalCompetencias)}));"")))
  ~~~
  Ou seja:
  1) nunca aplica o reajuste na primeira competência;
  2) sempre aplica o reajuste na competência da Lei 8.870;
  3) no mais, aplica o reajuste seguindo as datas-base.
  Note-se, ainda, que a técnica de transposição da coluna `DataBase` foi alterada.
  No lugar de:
  ~~~
  DESLOC(DataBase;LinhaInicialTabelaIndices-2;0;TotalCompetencias)
  ~~~
  Agora tem-se:
  ~~~
  {"";DESLOC(DataBase;LinhaInicialTabelaIndices-1;0;TotalCompetencias)}
  ~~~
  Essa técnica é similar a que foi utilizada nos demonstrativos, só que agora para inclusão de uma linha "cega" no lugar em que fica o título, para possibilitar o deslocamento da área de dados para o "corpo" da página.

**Aprimoramentos**

+ A mesma técnica de inclusão da linha de título na matriz para deslocamento da área de dados foi também aplicada nas colunas dos modificadores e em `Piso`, `Teto`, `IndicesReajuste`, `IndiceMensalAtualizacao`, `IndiceMensalAtualizacaoAjustado` e `JurosTaxaMensal`.
Não foi possível implementar essa técnica em `DescontoRenda` nem em `DescontoAbono` porque a análise da fórmula resultava em erro. 