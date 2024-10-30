# O que são APIs? 

Uma interface de programação de aplicações (API) é um conjunto de ferramentas, definições e protocolos para criar e integrar softwares de aplicações. Com ela, sua solução ou serviço pode se comunicar com outras soluções e serviços sem precisar saber como eles foram implementados. As APIs simplificam o desenvolvimento de aplicações, gerando economia de tempo e dinheiro para as empresas. Ao projetar novas ferramentas e soluções (ou gerenciar as atuais), as APIs oferecem a flexibilidade necessária, simplifica o design, a administração e o uso, além de fornecer oportunidades de inovação.
Fonte: redhat.com

## Testando uma API

Segue um passo a passo de como realizar testes de API, nesse exemplo foram utilizadas duas ferramentas: Postman e SoapUI. O site utilizado para testes foi o [dados abertos](http://dados.gov.br/dataset), site do governo brasileiro que disponibiliza entre outras coisas a cotação de moedas, sendo assim um bom site para praticar. Você pode escolher a moeda, cotação do dia ou período por exemplo, após selecionar os dados é gerada a url como mostro na imagem abaixo:  

![example](https://github.com/andreddias/API/blob/master/dados.png) 

Passo a passo de como utilizar:  
1 - Clicar em Copiar URL;  
2 - Abrir o Postman;  
3 - Copiar a URL no espaço em destaque na cor vermelha e clicar em Send (imagem 2);  
4 - Será retornado o resultado, como mostro na imagem 2:  

![example](https://github.com/andreddias/API/blob/master/postman.png) 

Você pode realizar os testes da API verificando os dados manualmentem ou automatizar fazendo com que a própria ferramenta verifique se o valor apresentado é o valor esperado, isso é muito bom para realizar um teste de regressão. Na imagem 2 foi utilizado o SoapUI para conferir os dados automaticamente, vou explicar nesse passo a passo.  
1 - Foi passado um determinado CEP como exemplo;  
2 - Foram criados cinco asserts testando o valor recebido em cada variável;  
3 - Mostrando o valor esperado para o campo bairro;  
4 - Ao clicar no Play retornou o resultado;  
5 - Em verde temos a comprovação que esse caso de teste passou. Quando informamos o CEP 24130223, o resultado esperado no passo 2 para o campo bairro "Fonseca" foi o valor retornado no passo 4. 

Neste exemplo mostramos cada campo, mas você pode realizar a regressão de todos os casos de testes de uma única vez sem precisar verificar o resultado, porque com os asserts você está garantido que o valor recebido é igual ao resultado esperado, garantindo assim que o teste de regressão passou.
![example](https://github.com/andreddias/API/blob/master/soapUI.png)

## Criando uma aplicação front-end

No meu [site pessoal](http://andreddias.wixsite.com/home/cambio) demonstro como utilizar os dados recebidos na API, utilizei como exemplo a cotação do Dólar comercial de compra e venda no formato Json, no site foi utilizado html e JavaScript para receber os dados. Você pode ver o código fonte [aqui](cotacoes.html)

Em um outro exemplo foi criado o site [saudelisboa](http://saudelisboa.wixsite.com/meusite) que retorna os dados abertos de Lisboa referente a saúde, [aqui](http://lisboaaberta.cm-lisboa.pt/index.php/pt/) 

## Centros de Saúde 

Encontre o centro de saúde desejado, após selecionar a morada são exibidos os centros de saúde do sítio desejado em uma tabela. Veja o [código](https://github.com/andreddias/API/blob/master/centrosaude.html).

## Farmácias

Encontre a farmácia desejada. Após selecionar a farmácia são exibidos os dados de contato. Veja o [código](https://github.com/andreddias/API/blob/master/farmacia.html).

## Weather

Previsão do tempo. É necessário criar uma chave de API, você pode ler a referência e o help [aqui](https://openweathermap.org/appid). Veja o [código](https://github.com/andreddias/API/blob/master/climatempoHoje.html)

## Fontes:  
#### Urls utilizadas do site Dados abertos do governo brasileiro:  
[Cotação de qualquer moeda](https://olinda.bcb.gov.br/olinda/servico/PTAX/versao/v1/swagger-ui3#/) utilizado em "Como testar a API"  
[Cotação dólar](http://dados.gov.br/dataset/dolar-americano-usd-todos-os-boletins-diarios) utilizado em "Como utilizar esses dados coletados da API?"  
Exemplo disponível no meu [site pessoal](http://andreddias.wixsite.com/home/cambio ) 

#### Urls utilizadas no site Lisboa aberta do governo português:
Site [saudelisboa](http://saudelisboa.wixsite.com/meusite)
Fonte dos dados do site saúde [Lisboaaberta](http://lisboaaberta.cm-lisboa.pt/index.php/pt/saude)

O que é uma API? [link1](https://vertigo.com.br/o-que-e-api-entenda-de-uma-maneira-simples/), [link2](https://blog.caelum.com.br/rest-principios-e-boas-praticas/), [link3](https://becode.com.br/o-que-e-api-rest-e-restful/), [link4](https://canaltech.com.br/software/o-que-e-api/) e por último a definição utilizada no início pela [Redhat](https://www.redhat.com/pt-br/topics/api/what-are-application-programming-interfaces)
