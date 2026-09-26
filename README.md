# 🚗 Dashboard de Vendas Porsche — Agentes de IA

Dashboard interativo desenvolvido a partir de uma base de vendas de veículos Porsche, utilizando **Inteligência Artificial como apoio à análise de dados, geração de insights e construção das visualizações**.

O projeto teve como objetivo explorar como ferramentas de IA podem ser utilizadas no processo de desenvolvimento de um dashboard, desde a análise inicial da base até a geração e o refinamento da solução final.

---

<p align="center">
  <img src="PorscheAnalytics.gif" alt="Dashboard Porsche Analytics" width="90%">
</p>

---

## 🎯 Objetivo do Projeto

Transformar uma base de vendas de veículos em um dashboard interativo capaz de apresentar indicadores, análises e insights sobre o desempenho comercial.

A análise contempla diferentes dimensões da operação:

* 💰 Desempenho financeiro
* 🚘 Modelos comercializados
* 💳 Formas de pagamento
* 📦 Status das entregas
* 📍 Distribuição geográfica das vendas

---

## 📊 Perguntas de Negócio

As perguntas de negócio foram definidas a partir da **análise exploratória inicial da base de vendas realizada com auxílio de IA**.

As principais perguntas abordadas no dashboard são:

| Pergunta                                                               | Dimensão analisada         |
| ---------------------------------------------------------------------- | -------------------------- |
| 💰 Qual é o volume total de vendas e a receita gerada?                 | Desempenho comercial       |
| 🚘 Quais modelos apresentam maior receita?                             | Produtos                   |
| 📈 Qual é o ticket médio das vendas?                                   | Desempenho financeiro      |
| 💳 Quais formas de pagamento são mais utilizadas?                      | Comportamento de pagamento |
| 📦 Qual é a distribuição dos pedidos por status de entrega?            | Operação logística         |
| 📍 Quais cidades concentram o maior volume de vendas?                  | Distribuição geográfica    |
| 🚘📍 Quais modelos se destacam nas cidades com maior volume de vendas? | Produto × localização      |

Essas perguntas permitem analisar diferentes dimensões da operação comercial e transformar os dados disponíveis em informações para análise.

---

## 🤖 Uso de Inteligência Artificial

A Inteligência Artificial foi utilizada ao longo do desenvolvimento do projeto, desde a análise exploratória inicial até a geração e o refinamento do dashboard.

### 🔎 1. Análise da base

O primeiro prompt utilizado foi:

```text
Quero que se comporte como analista de dados com muitos anos de experiência.
Estou enviando a base de vendas de veículos da Porsche e quero que gere
indicadores, análises e insights a partir dessa base.
Inclua a maior quantidade de insights possíveis.
```

A partir dessa análise inicial foram levantados indicadores, análises e insights que serviram como base para a construção do dashboard.

### 🖥️ 2. Geração do dashboard

Em seguida, foi solicitado:

```text
Quero que crie um dashboard interativo para analisar a base.
Esse dashboard precisa ter todos os indicadores, gráficos e tabelas
que você levantou acima.

Não esqueça de adicionar filtros que vão mudar os valores dos gráficos
e indicadores ao serem alterados.

Crie esse dashboard em HTML/CSS/JS.
```

### 🎨 3. Direcionamento de UI/UX

Para a identidade visual, foi utilizado o seguinte direcionamento:

```text
Sobre o UI/UX, se baseie no site oficial da Porsche Brasil.

Quero um design sofisticado com um toque feminino, pois sou mulher
e quero passar a ideia de que mulheres também gostam de carros de luxo.

Não quero nada infantil.
```

---

## 🔄 Refinamentos realizados

Após a geração inicial, o dashboard passou por uma série de avaliações e ajustes iterativos.

### Primeiros ajustes

* 💰 Padronização dos valores monetários para o formato `1.000,00`;
* 🎨 Inclusão de mais cores nas visualizações;
* 📍 Inclusão de insight sobre os modelos mais vendidos em cada cidade.

### Ajustes nos gráficos

* 🎨 Alteração das cores do gráfico **Status de Entrega**;
* 📊 Inclusão de um gráfico para permitir a comprovação do insight regional;
* 🔍 Revisão do gráfico **Preferência por Região (Top Cidades)**, considerado inicialmente confuso.

### Reformulação do gráfico regional

Após uma nova avaliação, o gráfico foi substituído por:

**Top 5 Cidades por Volume de Vendas**

Características definidas:

* 📊 Barras horizontais;
* 🌹 Uma única cor rose gold;
* ⬇️ Ordenação decrescente;
* 🔢 Número de vendas apresentado no final da barra;
* 🚫 Sem legenda;
* 💬 Tooltip contendo **Cidade, Vendas e Modelo líder**.

### Identidade do dashboard

Após os ajustes dos gráficos, foi incluído um cabeçalho para identificação da empresa.

### 🛠️ Revisão manual do HTML

Na revisão da versão final, foi identificado que o título:

> **Funil Logístico (Status de Entrega)**

não correspondia adequadamente ao tipo de visualização apresentada.

Nesse caso, em vez de solicitar uma nova alteração à IA, o arquivo HTML foi aberto manualmente, o título foi localizado, corrigido e o arquivo foi salvo novamente.

Esse foi um dos momentos em que a revisão humana foi utilizada diretamente no código gerado pela IA.

---

## 🧹 Tratamento da Base

Antes de enviar a base para a IA, foi realizado um tratamento inicial:

* 🧹 Foram mantidas apenas as colunas sanitizadas;
* 🌎 Os títulos das colunas foram traduzidos.

Após esse tratamento, a base foi utilizada como entrada para a análise exploratória e geração do dashboard.

---

## 🧰 Ferramentas Utilizadas

| Ferramenta          | Utilização                                  |
| ------------------- | ------------------------------------------- |
| 🤖 **Gemini Pro**   | Análise da base e geração do dashboard      |
| 🖥️ **Canvas**      | Desenvolvimento do dashboard com IA         |
| 💬 **ChatGPT**      | Desenvolvimento e avaliação do projeto      |
| 🌐 **HTML**         | Estrutura do dashboard                      |
| 🎨 **CSS**          | Estilização e identidade visual             |
| ⚙️ **JavaScript**   | Interatividade e funcionamento dos gráficos |
| 🐙 **GitHub Pages** | Publicação do dashboard                     |

> **Observação:** O ChatGPT foi utilizado durante o desenvolvimento e avaliação do projeto, mas a geração do dashboard foi realizada com o **Gemini Pro com Canvas**. Não foi utilizado um agente com skill para a geração do dashboard.

---

## 🌐 Dashboard Publicado

🔗 **[Acessar o Dashboard Porsche](https://vanmatos.github.io/Dashboard-Porsche-Agentes-IA/)**

---

## 📌 Considerações

Este projeto demonstra uma abordagem de desenvolvimento assistida por Inteligência Artificial, na qual a IA foi utilizada para apoiar a **exploração dos dados, identificação de indicadores, geração de insights e construção do dashboard**, enquanto o resultado foi avaliado e refinado iterativamente.

O projeto também evidencia a importância da **revisão humana da solução gerada**, incluindo a avaliação das visualizações, adequação dos títulos e ajustes manuais no código quando necessário.

---

### 👩‍💻 Projeto desenvolvido por Vanessa Albuquerque

**Dashboard de Vendas Porsche | Agentes de IA | BI & Data Analytics**
