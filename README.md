# Testes de API

## Como testar a API

Segue um passo a passo de como realizar um teste de API, nesse exemplo foi utilizada a ferramenta Postman, mas existem outras ferramentas como o Soapui. O site utilizado para testes foi o dados abertos, site do governo brasileiro, que disponibiliza entre outras coisas a cotação de moedas. Você pode escolher a moeda, cotação do dia ou período por exemplo, após selecionar os dados é gerada a url como mostro na imagem abaixo:  

![example](https://github.com/andreddias/API/blob/master/dados.png)

Passo a passo de como utilizar:  
1 - Clicar em Copiar a Url;  
2 - Abrir o Postman;  
3 - Copiar a URL no espaço em destaque na cor vermelha e clicar em Send;  
4 - Será retornado o resultado, como mostro na imagem abaixo:  

![example](https://github.com/andreddias/API/blob/master/postman.png)

Você pode realizar os testes da API verificando os dados manualmentem ou automatizar fazendo com que a própria ferramenta verifique se o valor apresentado é o valor esperado. Na imagem abaixo foi utilizado o SoapUI para conferir os dados automaticamente, foram passados os resultados esperados ao informar um determinado CEP

![example](https://github.com/andreddias/API/blob/master/soapUI.png)

## Como utilizar esses dados coletados da API?

No meu [site pessoal](http://andreddias.wixsite.com/home/cambio) demonstro como utilizar os dados recebidos na API, utilizei como exemplo a cotação do Dólar comercial de compra e venda no formato Json, no site foi utilizado html e JavaScript. 

## Fonte  
Site do governo: [Dados abertos](http://dados.gov.br/dataset/dolar-americano-usd-todos-os-boletins-diarios)  
Link Dólar compra: http://dados.gov.br/dataset/10813-taxa-de-cambio-livre-dolar-americano-compra  
Link Dólar venda: http://dados.gov.br/dataset/1-taxa-de-cambio-livre-dolar-americano-venda-diario  
Link de outras moedas: https://olinda.bcb.gov.br/olinda/servico/PTAX/versao/v1/swagger-ui3#/  
Exemplo disponível no site: http://andreddias.wixsite.com/home/cambio
