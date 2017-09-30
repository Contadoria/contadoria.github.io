---
title: Publicada a versão 1.1.3 da planilha CalculoAtrasados
timestamp: 22/09/2017 00:00:00
categories:
  - atualizações
---

**Correção de bugs**
* Primeiro abono calculado: foi invertida a lógica da ProporcaoAbono:  
  1. Primeiro
    ~~~
    SE(LIN(ProporcaoAbono)=LinhaPrimeiroAbono;ProporcaoPrimeiroAbono;
    ~~~
  1. Depois
    ~~~
    SE(LIN(ProporcaoAbono)=UltimaLinhaAbono;ProporcaoUltimoAbono;
    ~~~