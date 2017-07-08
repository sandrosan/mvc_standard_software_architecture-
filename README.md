## mvc_standard_software_architecture

MVC é nada mais que um padrão de arquitetura de software, separando sua aplicação em 3 camadas. A camada de interação do usuário(view), a camada de manipulação dos dados(model) e a camada de controle(controller).

## Model

Sempre que você pensar em manipulação de dados, pense em model. Ele é responsável pela leitura e escrita de dados, e também de suas validações.

## View

Simples: a camada de interação com o usuário. Ela apenas faz a exibição dos dados.

## Controller

O responsável por receber todas as requisições do usuário. Seus métodos chamados actions são responsáveis por uma página, controlando qual model usar e qual view será mostrado ao usuário.

(A imagem abaixo representa o fluxo do MVC em um contexto de Internet, com uma requisição HTTP e resposta em formato HTML ou XML)

<a href="https://pt.stackoverflow.com/questions/55486/o-que-%C3%A9-mvcmodel-view-controller/"><img src="https://i.stack.imgur.com/YfSWp.jpg" width=200></a><br/>

## O diálogo das camadas na Web

**View** - Fala Controller ! O usuário acabou de pedir para acessar o Facebook ! Pega os dados de login dele ai.

**Controller** – Blz. Já te mando a resposta. Ai model, meu parceiro, toma esses dados de login e verifica se ele loga.

**Model** – Os dados são válidos. Mandando a resposta de login.

**Controller** – Blz. View, o usuário informou os dados corretos. Vou mandar pra vc os dados dele e você carrega a página de perfil.

**View** – Vlw. Mostrando ao usuário…

