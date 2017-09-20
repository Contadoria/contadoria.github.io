---
timestamp: "03/11/2016"
title: Realizada a primeira reunião do projeto
categories:
  - histórico
---

A primeira reunião do projeto, realizada no dia 03/11/2016, no Juizado Especial Federal de São Paulo, teve como assunto principal a definição do sistema que seria utilizado para desenvolvimento: *Excel* ou *Google Sheets*.

Foram avaliados os seguintes pontos:

a. viabilidade de implementação das funcionalidades que desejamos;
a. facilidade de controle de versões e distribuição;
a. facilidade de colaboração;
a. a ferramenta deve ser gratuita.

Em relação ao *Google Sheets* foram identificados os seguintes pontos positivos e negativos:

a) **pontos positivos**:

* gratuidade, com 15Gb de armazenamento no *Google Drive*;
* armazenamento em nuvem, facilitando a distribuição e a colaboração;
* desnecessidade de instalação;
* controle de versões automático, possibilidade de integração com o Github;
* facilidade de importação de dados da web;
* funcionamento no Browser, sem necessidade de alteração das regras de TI existentes;
* integração com outros serviços do Google;
* possibilidade de criar webservices e sites gratuitos;
* possibilidade de rodar código no servidor e no cliente;
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
* no Office Online, possibilidade de criar livremente em Javascript (possibilidade de utilização de qualquer IDE;
* quaisquer bibliotecas, frameworks etc.;
* meios robustos para criação e depuração de fórmulas complexas;
* já utilizado pelas contadorias;
* tabelas - criação de referências estruturadas e alteração de fórmulas em bloco;
* intervalos nomeados dinâmicas.

b) **pontos negativos**:

* o Office 2010, que é a versão licenciada pela Justiça Federal, só roda VBA;
* necessidade de rodar o Office Online (mais simples) para acessar suplementos criados em Javascript;
* necessidade de obter hospedagem para os suplementos;
* várias APIs ainda incompletas (Microsoft Graph em estágio de desenvolvimento);
* aparentemente, não serve HTML, nem permite conversão de arquivos no servidor;
* os sites do *Sharepoint* são pagos;
* não há meio de criar web services (só se pode utilizar o serviço REST para acesso a planilhas).

Em seguida, os dois sistemas foram comparados entre si:

**Vantagens do Google Sheets sobre o Excel**:

* maior facilidade de colaboração, controle de versões, distribuição, manutenção (desde que tomadas medidas de segurança e implementada a possibilidade de operação em conjunto com o Github);
* maior clareza na criação de fórmulas de matriz;
* maior facilidade de criação, manutenção e distribuição de scripts;
* possibilidade de rodar códigos no servidor e criar web services. 

**Vantagens do Excel sobre Google Sheets**:

* maior familiaridade dos contadores;
* possibilidade de criar referências estruturadas e dinâmicas (definição de intervalos nomeados com fórmulas);
* recursos mais robustos para efetuar cálculos em lote;
* ferramentas de depuração para fórmulas complexas.

Ao final, chegou-se à conclusão de que o *Google Sheets* era o único sistema que atenderia a todas as nossas necessidades do projeto, porque facilitaria a distribuição e daria acesso a ferramentas mais modernas de desenvolvimento e ao controle de versões.

As deficiências em relação ao *Excel*, especialmente no que tange à falta de referências estruturadas, poderiam ser supridas pela modularização das planilhas. Além disso, no futuro seria provavelmente mais fácil integrar o *Excel* ao *Google Sheets* do que o inverso, já que ambos os sistemas haviam optado por adotar as tecnologias da Web e o *Google Sheets* já estav avançado nesse caminho.