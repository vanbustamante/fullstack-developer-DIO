# Desafio DIO - Requisitando Dados da API CoinMarketCap

Este projeto é parte de um desafio de código proposto pela Digital Innovation One (DIO). O objetivo é consumir a API do CoinMarketCap para listar as 10 principais criptomoedas.

## 📖 Descrição

A aplicação consiste em uma página HTML simples que utiliza JavaScript para fazer uma requisição GET à API do CoinMarketCap. A resposta da API é processada para exibir o nome e o símbolo das 10 primeiras criptomoedas retornadas, utilizando o Bootstrap para uma estilização básica.

## ✨ Funcionalidades

- Requisição à API CoinMarketCap.
- Exibição dinâmica das 10 principais criptomoedas (nome e símbolo).
- Tratamento básico de erros na requisição.

## 💻 Tecnologias Utilizadas

- **HTML5:** Estrutura da página.
- **CSS3 / Bootstrap 5:** Estilização e layout responsivo.
- **JavaScript (Fetch API):** Para realizar a requisição assíncrona à API.
- **API CoinMarketCap:** Fonte dos dados das criptomoedas.

## 🚀 Como Executar o Projeto

Para executar este projeto, você precisará de uma chave de API válida do CoinMarketCap.

### Pré-requisitos

1. Navegador web moderno.
2. Uma chave da API do [CoinMarketCap Developer](https://coinmarketcap.com/api/).

### Passos

1. **Clone ou baixe o código:**
   Salve o código HTML fornecido em um arquivo chamado `index.html`.

2. **Imagem Placeholder:**
   O código utiliza uma imagem placeholder chamada `coin.jpeg`. Certifique-se de ter um arquivo de imagem com esse nome no mesmo diretório do `index.html`, ou altere o caminho da imagem no código:
   ```html
   <img src="coin.jpeg" class="align-self-center mr-3" alt="coin" width="100" height="60">

3. **Configure sua API Key:**
    No bloco <script>, substitua o valor da chave existente pela sua chave de API pessoal do CoinMarketCap:

    ```bash
    var apikey = {
        key: 'SUA_API_KEY_AQUI' // Substitua 'SUA_API_KEY_AQUI' pela sua chave
    }

4. **Execute:**
    Abra o arquivo index.html em seu navegador. A página fará a requisição e exibirá a lista das criptomoedas.


## 🏗️ Estrutura do Código
O código está estruturado da seguinte forma:

- HTML: Define a estrutura básica com um breadcrumb e um contêiner (id='coins') onde os dados serão inseridos. O Bootstrap é importado via CDN.

- JavaScript:

    - Armazena a chave da API.

    - Usa fetch() para solicitar dados do endpoint /v1/cryptocurrency/map.

    - Itera sobre os primeiros 10 itens (api.data) retornados.

    - Constrói dinamicamente o HTML usando template literals para exibir os dados no div#coins.

    - Inclui um bloco .catch() para logar erros no console, caso a requisição falhe.

### ⚠️ Importante
Para que este projeto funcione, você deve inserir sua própria chave da API do CoinMarketCap no local indicado no arquivo index.html.

É importante notar que a abordagem de colocar a chave diretamente no código do lado do cliente (front-end) foi usada aqui para simplificar este desafio de estudo. Em um projeto real (de produção), as chaves de API devem ser mantidas em segredo e gerenciadas em um servidor back-end para evitar que sejam expostas publicamente.

## 👨‍💻 Autora:

Desenvolvido por Vanessa Osório Bustamante.

<a href="https://www.linkedin.com/in/vanessaosoriobustamante/" target="_blank">

<img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">

</a>