[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-360/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) 

<sub> 📂 Projeto - Data Science - Sarah F. Rezende

## **Projeto** - **Detecção de Fraudes em Cartões de Crédito** 

[PROJETO (COLAB)](https://github.com/SarahFeanor/Credit_Card_Fraud_Detection_Project/blob/main/Detec%C3%A7%C3%A3o_de_fraude.ipynb)

Bem-vindos(as). Este repositório foi criado com o propósito de estudo. Vale ressaltar que todos os dados são exclusivamente para fins de demonstração, garantindo total privacidade e conformidade ética.

<p align="center">
  <a href="https://github.com/SarahFeanor?tab=repositories">
    <img src="https://cdn.discordapp.com/attachments/1063559719291199599/1202666498032799894/download.webp?ex=65ce4975&is=65bbd475&hm=0cd44d77f21c6b57ac8a03fde9dc344f5887292ad2b6ac6933ae4f59d570f68d&" alt="capa" width="600" height="300">
  </a>
</p> <p align="center"> <sup>Foto de Imagge </sup> </p>

## **Protegendo Transações Financeiras: Detecção de Fraudes em Cartões de Crédito**

O combate às fraudes em cartões de crédito constitui uma das principais preocupações para as instituições financeiras. Essas ocorrências podem acarretar prejuízos consideráveis tanto para os consumidores quanto para as próprias instituições, destacando-se como um desafio contínuo. A complexidade reside no fato de que os fraudadores estão em busca constante de métodos para contornar os sistemas de segurança.

Segundo dados da Serasa Experian, somente no Brasil, aproximadamente 12,1 milhões de pessoas foram alvo de algum tipo de fraude financeira no último ano. Isso resultou em um prejuízo de 1,8 bilhão de reais somente nos últimos 12 meses.

A tarefa de detectar fraudes em transações de cartões de crédito é intrincada. Transações legítimas e fraudulentas podem ser semelhantes, o que complica o processo de diferenciação. Além disso, as fraudes podem ocorrer em diferentes faixas de valores e locais, dificultando a identificação de um padrão. Esse cenário pode levar a erros de detecção, incluindo tanto falsos positivos (blocos preventivos em transações legítimas) quanto falsos negativos (não identificação de transações fraudulentas).

## **Objetivo do Projeto**

O propósito deste projeto é conduzir uma análise exploratória dos dados referentes a transações de cartões de crédito, bem como desenvolver modelos de machine learning que tenham a capacidade de identificar transações fraudulentas com elevada precisão. Para alcançar esse objetivo, serão empregadas técnicas avançadas de análise de dados e machine learning, com a finalidade de identificar padrões e anomalias nos dados. Adicionalmente, serão aplicadas abordagens de balanceamento de dados. Uma parte crucial do processo consistirá em avaliar a eficácia dos modelos construídos, tanto em termos de sua precisão na detecção de fraudes quanto em relação à minimização de falsos positivos.

## 📂 **Dados**

Os dados utilizados neste projeto provêm de diversas empresas de cartões de crédito na Europa. O conjunto de dados abrange transações financeiras que ocorreram durante um intervalo de dois dias, incluindo 492 casos de fraudes em meio a quase 290 mil transações. É importante observar que o conjunto de dados é altamente desbalanceado, com as fraudes representando somente 0,17% do total.

Outro ponto a se destacar é que as características do conjunto de dados são todas numéricas e foram submetidas a um processo de descaracterização para salvaguardar questões de privacidade e segurança. Por consequência, as colunas são denotadas por meio de nomenclaturas como v1, v2, v3, ..., v28.

"https://www.dropbox.com/s/b44o3t3ehmnx2b7/creditcard.csv?dl=1"

## **Conclusão**
Com base nas análises meticulosas realizadas, fica evidente que a seleção criteriosa do modelo de classificação e a escolha sensata da técnica de balanceamento de classes desempenham um papel fundamental no sucesso da detecção de fraudes em transações financeiras. Ao considerar dois tipos de técnicas de balanceamento de classes (under-sampling e over-sampling) em conjunto com dois modelos de classificação (Decision Tree e Logistic Regression), podemos tirar valiosas lições.

A Regressão Logística emergiu como uma opção de destaque para resolver esse desafio, apresentando um desempenho superior em relação à Decision Tree. Especificamente, os modelos baseados em Regressão Logística alcançaram valores de AUC próximos a 0,93, destacando a capacidade de distinguir entre transações legítimas e fraudulentas de maneira eficaz.

As técnicas de balanceamento de classes, especialmente o under-sampling, revelaram-se estratégias eficazes para aprimorar o desempenho dos modelos. Observou-se que o modelo usando under-sampling e Regressão Logística obteve um recall consistente para a classe minoritária (fraudes), tanto nos conjuntos de validação como de treinamento. Isso indica que essa combinação é uma abordagem robusta e eficiente para enfrentar o desafio de detecção de fraudes.

Por outro lado, o modelo Decision Tree não conseguiu alcançar os mesmos níveis de desempenho que os modelos de Regressão Logística em termos de AUC e recall. Esse modelo registrou valores de AUC em torno de 0,76 e 0,85 (para under-sampling e over-sampling, respectivamente) na validação, com recall de apenas 0,71 para a classe minoritária com over-sampling. No entanto, é notável que, nos dados de teste, ambos os modelos alcançaram um desempenho mais sólido, atingindo valores de recall de 0,92 e 0,81 para a classe minoritária.

Em síntese, esta análise detalhada reforça a importância crítica da seleção cuidadosa do modelo de classificação e da técnica de balanceamento de classes no contexto da detecção de fraudes em transações financeiras. A Regressão Logística se destaca como uma escolha promissora, e o emprego adequado de estratégias de balanceamento pode ser decisivo para otimizar o desempenho do modelo na detecção de fraudes, contribuindo para a segurança e integridade das operações financeiras.
