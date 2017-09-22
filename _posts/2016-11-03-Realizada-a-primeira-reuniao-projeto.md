---
timestamp: "03/11/2016"
title: Realizada a primeira reunião do projeto
categories:
  - histórico
---

A primeira reunião do projeto, realizada no dia 03/11/2016, no Juizado Especial Federal de São Paulo, teve como assunto principal a definição do sistema que seria utilizado para desenvolvimento: *Excel* ou *Google Sheets*.

Foram avaliados os seguintes pontos:

a) viabilidade de implementação de todas as funcionalidades desejadas;
b) facilidade de controle de versões e distribuição;
c) facilidade de colaboração;
d) gratuidade.

Em relação ao *Google Sheets* foram identificados os seguintes pontos positivos e negativos:

a) **pontos positivos**:

* gratuidade, com 15Gb de armazenamento no *Google Drive*;
* armazenamento em nuvem, facilitando a distribuição e a colaboração;
* desnecessidade de instalação;
* controle de versões automático, possibilidade de integração com o *Github*;
* facilidade de importação de dados da web;
* funcionamento no Browser, sem necessidade de alteração das regras de TI existentes;
* integração com outros serviços do *Google*;
* possibilidade de criar webservices e sites gratuitos;
* possibilidade de rodar código tanto no servidor quanto no cliente;
* maior facilidade de criação de fórmulas de matriz;
* colaboração com comentários e *chat window*.

b) **pontos negativos**:

* quotas e restrições de tempo;
* processamento mais lento dos scripts;
* modelo de objetos muito menor que o do Excel;
* necessidade de reaprendizado;
* IDE mais simples para criação de scripts.

Em relação ao *Excel* foi levantado o seguinte:

a) **pontos positivos**:

* a JF detém licenças do Office 2010;
* o OneDrive dá 5 GB de armazenagem gratuitos;
* sem quotas ou restrições de tempo;
* no Office Online, possibilidade de programar em Javascript, com utilização de qualquer IDE, biblioteca, framework etc.;
* meios mais robustos para criação e depuração de fórmulas complexas;
* sistema já conhecido e utilizado pelas contadorias;
* possibilidade de estruturar os dados em tabelas;
* possibilidade de utilizar intervalos nomeados dinâmicos.

b) **pontos negativos**:

* o Office 2010, que é a versão licenciada pela Justiça Federal, só executa o Visual Basic for Applications (VBA), uma tecnologia antiga que será provalvemente desativada;
* necessidade de rodar o Office Online (mais simples) para acessar suplementos criados em Javascript;
* necessidade de obter hospedagem para os suplementos;
* várias APIs ainda incompletas (*Microsoft Graph* em estágio de desenvolvimento);
* aparentemente, não serve HTML, nem permite conversão de arquivos no servidor;
* os sites do *Sharepoint* são pagos;
* não há meio de criar web services complexos, sendo possível apenas utilizar um serviço REST para acesso a planilhas.

Em seguida, os dois sistemas foram comparados entre si:

**Vantagens do _Google Sheets_ sobre o _Excel_**:

* maior facilidade de colaboração, controle de versões, distribuição, manutenção, desde que tomadas medidas de segurança e implementada a possibilidade de operação em conjunto com o *Github*;
* maior clareza na criação de fórmulas de matriz (*Array Formulas*);
* maior facilidade de criação, manutenção e distribuição de scripts;
* possibilidade de executar códigos tanto no cliente quanto no servidor e criar web services mais complexos. 

**Vantagens do _Excel_ sobre _Google Sheets_**:

* maior familiaridade dos contadores com o sistema;
* possibilidade de criar referências estruturadas e dinâmicas, com definição de intervalos nomeados utilizando fórmulas;
* recursos mais robustos para efetuar cálculos em lote;
* ferramentas de depuração para fórmulas complexas.

Ao final, chegou-se à conclusão de que o *Google Sheets* era o único sistema que tornaria possível implementar todas as funcionalidades desejadas, porque facilitaria a distribuição pela nuvem, daria acesso a ferramentas mais modernas de desenvolvimento e ao controle de versões.

As deficiências em relação ao *Excel*, especialmente no que tange à falta de referências estruturadas, poderiam ser supridas pela modularização das planilhas. 

Além disso, no futuro seria provavelmente mais fácil integrar o *Excel* ao *Google Sheets* do que o inverso, já que ambos os sistemas haviam optado por adotar as tecnologias da Web e o *Google Sheets* já tinha avançado mais nesse caminho.
