# Testes de API  

Vamos pular a etapa do conceito, mas vou deixar algumas fontes sobre o que é uma API no final da página. O foco aqui é o teste utilizando algumas ferramentas específicas e como utilizar os dados que recebeu em uma aplicação web. 

## Como testar a API

Segue um passo a passo de como realizar testes de API, nesse exemplo foram utilizadas duas ferramentas: Postman e SoapUI. O site utilizado para testes foi o dados abertos, site do governo brasileiro que disponibiliza entre outras coisas a cotação de moedas, um bom site para praticar. Você pode escolher a moeda, cotação do dia ou período por exemplo, após selecionar os dados é gerada a url como mostro na imagem abaixo:  

![example](https://github.com/andreddias/API/blob/master/dados.png)

Passo a passo de como utilizar:  
1 - Clicar em Copiar a Url;  
2 - Abrir o Postman;  
3 - Copiar a URL no espaço em destaque na cor vermelha e clicar em Send;  
4 - Será retornado o resultado, como mostro na imagem abaixo:  

![example](https://github.com/andreddias/API/blob/master/postman.png)

Você pode realizar os testes da API verificando os dados manualmentem ou automatizar fazendo com que a própria ferramenta verifique se o valor apresentado é o valor esperado, isso é muito bom para realizar um teste de regressão. Na imagem abaixo foi utilizado o SoapUI para conferir os dados automaticamente, vou explicar cada campo.  
1 - Foi passado um determinado CEP como exemplo.  
2 - Foram criados cinco asserts testando o valor recebido em cada variável.  
3 - Mostrando o valor esperado para o campo bairro.  
4 - Ao clicar no Play retornou o resultado.  
5 - Em verde temos a comprovação que esse caso de teste passou.

Neste exemplo mostramos cada campo, mas você pode realizar a regressão de todos os casos de testes de uma única vez sem precisar verificar o resultado, garantido assim que a regressão está funcionando.
![example](https://github.com/andreddias/API/blob/master/soapUI.png)

## Como utilizar esses dados coletados da API?

No meu [site pessoal](http://andreddias.wixsite.com/home/cambio) demonstro como utilizar os dados recebidos na API, utilizei como exemplo a cotação do Dólar comercial de compra e venda no formato Json, no site foi utilizado html e JavaScript. 

## Fontes:  
Site do governo: [Dados abertos](http://dados.gov.br/dataset/dolar-americano-usd-todos-os-boletins-diarios)  
Link Dólar compra: http://dados.gov.br/dataset/10813-taxa-de-cambio-livre-dolar-americano-compra  
Link Dólar venda: http://dados.gov.br/dataset/1-taxa-de-cambio-livre-dolar-americano-venda-diario  
Link de outras moedas: https://olinda.bcb.gov.br/olinda/servico/PTAX/versao/v1/swagger-ui3#/  
Exemplo disponível no site: http://andreddias.wixsite.com/home/cambio  
O que é uma API? [link1](https://vertigo.com.br/o-que-e-api-entenda-de-uma-maneira-simples/), [link2](https://pt.wikipedia.org/wiki/Interface_de_programa%C3%A7%C3%A3o_de_aplica%C3%A7%C3%B5es) e [link3](https://canaltech.com.br/software/o-que-e-api/)
