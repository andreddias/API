# Utilizando Json e testes de API
## Testes de API

Segue um passo a passo de como realizar um teste de API, nesse exemplo foi utilizado o Postman, mas pode ser feito no Soapui ou em outras ferramentas.
O site utilizado para testes foi o dados abertos também disponibiliza a cotação de outras moedas no [link](https://olinda.bcb.gov.br/olinda/servico/PTAX/versao/v1/swagger-ui3#/) você pode escolher a moeda, cotação do dia ou período por exemplo. Após selecionar os dados é gerada uma url como mostro na imagem abaixo:
![example](https://github.com/andreddias/API/blob/master/dados.png)

Clicar em Copiar a Url
Abrir o Postman
Copiar a URL no espaço em destaque na cor vermelha e clicar em Send
Será retornado o resultado, como mostro na imagem abaixo:

![example](https://github.com/andreddias/API/blob/master/postman.png)

## Json - Cotação Dólar

O site do governo brasileiro disponibiliza a cotação do Dólar comercial de compra e venda no formato Json. Foi utilizado html e JavaScript

Fonte site [Dados abertos](http://dados.gov.br/dataset/dolar-americano-usd-todos-os-boletins-diarios) 
## Taxas de câmbio por período, desde 1899

Link Dólar compra: http://dados.gov.br/dataset/10813-taxa-de-cambio-livre-dolar-americano-compra
Link Dólar venda: http://dados.gov.br/dataset/1-taxa-de-cambio-livre-dolar-americano-venda-diario
Exemplo disponível no site: http://andreddias.wixsite.com/home/cambio
