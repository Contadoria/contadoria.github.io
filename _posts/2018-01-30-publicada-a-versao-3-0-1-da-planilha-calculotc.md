---
title: Publicada a versão 3.0.1 da planilha CalculoTC
timestamp: 30/01/2018 00:05:57
categories:
  - atualizações
---

**Correção de "fake" bug**:
As funções customizadas que processam o tempo de contribuição sempre executam uma rotina de validação.
Ocorre que essa rotina de validação acaba retornando falsos positivos quando a planilha está vazia e é preenchida pela primeira vez, já que na ausência de dados será disparado o erro "Dado de entrada não é matriz". Nesse caso, o comportamento esperado é silenciar até que o usuário entre com os dados.
Assim, a exemplo do que se fez antes na fórmula que inclui a função `jef_ELIMINAR_CONCOMITANCIA`, alteramos a fórmula no intervalo `DataInicialTCDiscriminadoProcessado` para:
````
={"Data inicial"\"Data final"\"Descrição"\"Natureza"\"Contar Carência"\"Motivos"\"Observações"\"Classificação"\"Fator";SE(CONT.NÚM(M2:U2)>2;
SE(AjustarMarcosTemporais="Sim";jef_ESTABELECER_MARCOS_TEMPORAIS(DESLOC(M2:U2;0;0;CONT.NÚM(M:M));MarcosTemporais);DESLOC(M2:U2;0;0;CONT.NÚM(M:M)));{HOJE()\HOJE()\""\""\""\""\""\""\""\""})}
````
Desse modo, a fórmula customizada somente será acionada quando houver mais de dois números na linha `M2:U`, ou seja, quando o usuário tiver preenchido ao menos a primeira linha dos períodos. Nesse caso, as datas inicial e final formam dois números e o fator o terceiro número.
Nessa mesma linha de raciocínio, a fórmula da célula `M1` foi aprimorada, trocando-se o trecho `CONT.NÚM(A2:J)>0` para `CONT.NÚM(A2:J)>2`. Assim, também a fórmula `jef_ELIMINAR_CONCOMITANCIA` somente será acionada quando os dados iniciais tiverem pelo menos a primeira linha preenchida. 