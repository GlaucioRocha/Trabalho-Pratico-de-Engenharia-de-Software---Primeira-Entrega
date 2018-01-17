# Trabalho-Pratico-de-Engenharia-de-Software---Primeira-Entrega

# LocaFácil: Análise de Requisitos

## 1. Introdução

Objetivando automizar o sistema de locação de filmes desenvolvemos este software que busca abranger todos os aspectos que envolvem a locação,  



Tem se tornado cada vez maior a busca por alimentação saudável. Alimentos com baixo teor calórico, sem glúten ou sem lactose. Pensando nesse público, e na tentativa de influenciar cada vez mais pessoas a se alimentarem de forma saudável, está loja se destina a fornecem diversas iguarias que se adequam à vida saudável.

Dentre nossos produtos, encontram-se óleos de coco, óleos de abacate, barras de cereal ou de frutas, doces sem lactoses e temperos sem adição desal ou produtos inorgânicos. Além disso, nosso site contará com dicas de como incluir alimentos saudáveis à rotina diária, e quais os benefícios que estes alimentos trazem para anossa saúde. Como substituir alimentos gordurosos e calóricos por alimentos mais saudáveis e muitas outras dicas.

##2. Descrição do Problema

O ambiente comercial atual requer formas práticas, funcionais e confiáves quando se trata de entregar um produto ou serviço idependente do ramo em que o mesmo é utilizado. 

Nossa proposta está em trazer um produto que visa considerar todos os aspectos importantes de mercado e entregar um produto coeso e integro para o gerenciamento comercial de locação de filmes, automatizando processos e entregando um sistema ideal para a sua locadora.



Nos dias de hoje cada vez mais pessoas procuram uma alimentação mais saudável, mas nem sempre sabem onde encontrar produtos do tipo
Visando isso, esse site busca facilitar a oferta de produtos e dicas de alimentação saudável, independentemente do lugar que o cliente se encontra.

## 3. Objetivo

Levar a sua empresa o gerenciamento de aluguel de filmes que irá suprir todas as necessidades, permitindo cadastros de Clientes, Catálogo de Filmes, Tela de Login, registros de empréstimo e devolução. 







Fornecer aos clientes de forma prática e no conforto de suas casas, produtos orgânicos e saudáveis. Produtos livres de glúten, lactose, componentes inorgânicos e demasiada quantidade de sódio. Além disso, buscaremos fornecer dicas de como se alimentar de forma saudável, como incluir tais alimentos na rotina alimentar, e como substituir alimentos gordurosos e calóricos por alimentos saudáveis. 

Nosso foco é atender ao público que deseja manter uma dieta alimentar saudável. E incentivar a transformação dos hábitos alimentares de cada vez mais pessoas. Nosso site conta também com uma aba de dicas de alimentação saudável.

## 4. Escopo da Aplicação
Sistema que permite o gerenciamento da locação de filmes.

O escopo do projeto é um site para que a Digital Nutri possa vender seus produtos e interagir com seus clientes.
## 5. Descrição do Produto
Objetivando o acesso de forma simplificada e intuitiva foi criado um site utilizando PHP, interligado ao banco de dados

Para produzir um produto que seja de fácil acesso a todos, escolhemos a criação de um site.
Para tal, pretendemos utilizar o Laravel 5, famoso framework PHP de código aberto,  por permitir um melhor controle de banco de dados e uma sintaxe mais limpa, facilitando manutenção do código.


## 6. Casos de Uso
Interações dos usuários com o sistema.
### 6.1 Caso de Uso I – Cadastrar Cliente
  - **Nível:** Administrador ou Cliente
  - **Atores primários:** Administrador e Cliente, 
  - **Interessados:**
    - **Administrador:** Efetuação de cadastro a fim de acessar o sistema.
    - **Cliente:** Efetuação de cadastro a fim de acessar o sistema.
  - **Pré-condições:** Acesso à Internet.
  - **Garantias de sucesso:** Clientes devidamente adicionado ao banco de dados. 
  - **Cenário de sucesso principal:**
	1. Cliente acessa a página web;
	2. Cliente seleciona o link Cadastrar;
	3. Cliente preenche devidamente os campos do formulário de cadastro;
	4. Cliente confirma o cadastro;
	5. Sistema confirma que o cadastro foi efetuado com sucesso.
  - **Extensões:** 
    - Passos 3 a 5: Campos preenchidos erroneamente
        - Processo de cadastro é interrompido
        - Usuário recebe feedback relativos ao problema

### 6.2 Caso de Uso II – Cadastrar Produto
 - **Nível:** Administrador
 - **Atores primários:** Administrador
 - **Interessados:** 
	- **Administrador:** Efetuação de cadastro a fim de adicionar produtos ao banco de dados.
 - **Pré-condições:** Acesso à Internet.
 - **Garantia de sucesso:** Produtos devidamente adicionados ao banco de dados. 
 - **Cenário de sucesso principal:**
	 1. Administrador acessa a página web;
	 2. Administrador seleciona o link Cadastrar Produtos ;
	 3. Administrador preenche devidamente os campos do formulário de cadastro;
	 4. Administrador confirma o cadastro;
	 5. Sistema confirma que o cadastro foi efetuado com sucesso.
 - **Extensões:** 
    - Passos 3 a 5: Campos preenchidos erroneamente
	     - Processo de cadastro é interrompio
	     - Administrador  recebe feedback relativos ao problema.

### 6.3 Caso de Uso III – Editar Cliente
 - **Nível:** Administrador ou Cliente
 - **Atores primários:** Cliente
 - **Interessados:** 
  - **Cliente:** Realizar alterações em campos editáveis após cadastro.
 - **Pré-condições:** Acesso à Internet. Usuário autenticado.
 - **Garantias de sucesso:**
    - Campo devidamente alterado no banco de dados. 
    - Atualização do valor do campo exibido no sistema.
 - **Cenário de sucesso principal:**
      1. Cliente acessa a página web;
      2. Cliente seleciona o link Fazer Login;
      3. Cliente realiza o processo de autenticação;
      4. Cliente acessa seu Perfil;
      5. Cliente seleciona modifica o campo desejado;
      6. Cliente confirma a edição;
      7. Perfil do cliente é atualizado.
  - **Extensões:** 
    - Passo 3: Usuário ou senha inválidos:
        - Processo de login é interrompido;
        - Erro é notificado ao usuário;
        - Dados são solicitados novamente;
    - Passos 5 a 6: Campos preenchidos erroneamente:
        - Processo de edição é interrompido.
        - Usuário recebe feedback relativos ao problema.

### 6.4 Caso de Uso IV – Editar Produto
 - **Nível:** Administrador
 - **Atores primários:** Administrador
 - **Interessados:** 
    - **Administrador:** Realizar alterações em campos editáveis após cadastro.
 - **Pré-condições:** Acesso à Internet. Usuário autenticado.
 - **Garantia de sucesso:** 
    - Campo devidamente alterado no banco de dados. 
    - Atualização do valor do campo exibido no sistema.
 - **Cenário de sucesso principal:**
    1. Administrador acessa a página web;
    2. Administrador seleciona o link Fazer Login;
    3. Administrador realiza o processo de autenticação;
    4. Administrador acessa seu link de Produto;
    5. Administrador seleciona link editar produto;
    6. Administrador seleciona e modifica o campo desejado;
    7. Administrador confirma a edição;
    8. Produto é atualizado.
 - **Extensões:**
    - Passo 3: Usuário ou senha inválidos:
        - Processo de login é interrompido;
        - Erro é notificado ao usuário;
        - Dados são solicitados novamente,
    - Passos 5 a 6: Campos preenchidos erroneamente:
        - Processo de edição é interrompido;
        - Usuário recebe feedback relativos ao problema.

### 6.5 Caso de Uso V – Remover Usuário
 - **Nível:** Administrador
 - **Atores primários:** Administrador
 - **Interessados:** 
    - **Administrador:** Realizar remoção de um usuário cadastrado.
 - **Pré-condições:** 
    - Acesso à Internet. 
    - Privilégio de Administrador.
 - **Garantias de sucesso:** 
    - Usuário devidamente removido do banco de dados. 
    - Confirmação exibida.
 - **Cenário de sucesso principal:**
    1. Administrador acessa a página web;
    2. Administrador realiza o processo de autenticação;
    3. Administrador pesquisa usuário à ser removido;
    4. Administrador aperta o botão remover;
    5. Administrador confirma que ele realmente deseja remover o usuário;
    6. Usuário é removido do banco de dados;
    7. Mensagem de confirmação de remoção é exibida.
 - **Extensões:** 
    - Passo 2: Usuário ou senha inválidos:
        - Processo de login é interrompido;
        - Erro é notificado ao usuário;
        - Dados são solicitados novamente.

### 6.6 Caso de Uso VI – Logar
  - **Nível:** Administrador ou Cliente
  - **Atores primários:** Administrador, Cliente
  - **Interessados:** 
    - **Administrador:** Efetuação de autenticação a fim de acessar o sistema.
    - **Cliente:** Efetuação de autenticação a fim de acessar o sistema.
  - **Pré-condições:** 
    - Acesso à Internet. 
    - Usuário previamente cadastrado.
  - **Garantia de sucesso:** Redirecionamento para página inicial do usuário.
  - **Cenário de sucesso principal:**
      1. Cliente acessa a página web;
      2. Cliente seleciona o link Logar ;
      3. Cliente informa campos usuário e senha;
      4. Cliente pressiona botão Logar ;
      5. Cliente redirecionado para sua página inicial;
  - **Extensões:** 
    - Passos 3 a 4: 
        - Usuário ou senha inválidos:
        - Processo de login é interrompido;
        - Erro é notificado ao usuário;
        - Dados são solicitados novamente.

### 6.7 Caso de Uso VII – Comprar produto
 - **Nível:** Cliente
 - **Atores primários:** Cliente
 - **Interessados:** Cliente: Comprar um produto em oferta.
 - **Pré-condições:** 
    - Acesso à Internet. 
    - Usuário autenticado.
 - **Garantias de sucesso:** O produto é selecionado e ao final do processo é retirado do banco de dados.
 - **Cenário de sucesso principal:**
    1. Cliente realiza processo de login no sistema;
    2. Cliente seleciona o link do produto(os) desejado(os);
    3. Cliente preenche os dados para finalização da compra;
    4. A compra é finalizada e o produto é retirado do banco de dados.
 - **Extensões:** 
    - Passo 1: Usuário ou senha inválidos:
        - Processo de login é interrompido;
        - Erro é notificado ao usuário;
        - Dados são solicitados novamente.
    - Passo 3: 
        - Campos preenchidos erroneamente;
        - Processo de criação é interrompido;
        - Administrador recebe feedback relativos ao problema.

### 6.8 Caso de Uso VIII – Tabela de todos os tipo de produtos existentes
  - **Nível:** Administrador ou Clientes
  - **Atores primários:** Administrador, Clientes
  - **Interessados:**
    - **Administrador:** Visualizar todas as opções de produtos oferecidos para venda.
    - **Cliente:** Visualizar todas as opções de produtos oferecidos para venda.
  - **Pré-condições:** 
    - Acesso à Internet. 
    - Administrador ou Clientes autenticados.
  - **Garantias de sucesso:** 
    - Nova aba é aberta e uma tabela é exibida. 
    - Em seguida, o usuário pode visualizar os produtos e fazer a compra dos mesmos se desejado.
  - **Cenário de sucesso principal:**
    1. Usuário acessa a página web;
    2. Usuário realiza processo autenticação;
    3. Usuário seleciona o link Produtos;
    4. A tabela de produtos é exibida com opções de botões para compra;
    5. Usuário escolhe os produtos e a quantidade desejada.
    6. Se selecionado algum produto para compra, nova aba é aberta para o processo de Compra de Produto.
  - **Extensões:**
    - Passo 1: Usuário ou senha inválidos:
        - Processo de autenticação é interrompido;
        - Erro é notificado ao usuário;
        - Dados são solicitados novamente.
    - Passo 5: Quantidade de produtos desejados é maior que a quantidade disponível no banco de dados:
        - Notificação do problema é exibido.
        - Alerta informando a quantidade disponível em estoque.
        - Retorna a aba de produtos.

### Caso de Uso IX – Aba de Dicas
  - **Nível:** Administrador ou Clientes
  - **Atores primários:** Administrador, Clientes
  - **Interessados:** 
    - **Administrador:** Visualizar todas as opções de produtos oferecidos para venda.
    - **Cliente:** Visualizar dicas de como se alimentar de forma saudável. Como substituir alimentos gordurosos ou calóricos por alimentos mais saudáveis. Quais os benefícios que cada um desses alimentos pode trazer. e muitas outras dicas
  - **Cenário de sucesso principal:**
    1. Usuário acessa a página web;
    2. Usuário seleciona o link Dicas;
    3. A lista de dicas é exibida com opções de botões para compra.

## 7 Classes
Nesta seção são apresentadas as classes que integram a aplicação, bem como um
diagrama para cada e um diagrama de classes onde mostra as relações entre elas.

### 7.1 Usuário
  Classe genérica para compartilhar atributos em comum entre as subclasses Administrador e Cliente.
  - **Administrador:** Usuário capaz de inserir, remover e atualizar Cliente e Produtos, bem
  como adicionar, editar e remover todas as categorias do sistema. Tem todos os privilégios do sistema.
  - **Cliente:** Usuário capaz fazer cadastro, visualizar produtos e fazer compra dos mesmos.

### 7.4  Compras
  A classe Compras é responsável por agrupar diferentes produtos e suas devidas características, como por exemplo o preço.
  - **Cadastrar Produtos:** A classe Cadastrar Produtos é responsável por adicionar produtos ao banco de dados, sendo o único que pode atualizar é o administrador.
  - **Cadastrar Cliente:** A classe Cadastrar Clientes é responsável por adicionar clientes ao banco de dados, sendo acessado por todos os níveis.

### 7.5 Dicas 
  A classe Dicas fornece dicas de como se alimentar de forma saudável, como incluir tais alimentos na rotina alimentar, e como substituir alimentos gordurosos e calóricos por alimentos saudáveis, sendo acessada por todos os níveis.

## 8 Banco de Dados

### 8.1 Diagrama de classes 
  ![Diagrama de Classes](Diagramas/Diagrama1.png)
### 8.2 Diagrama Entidade Relacionamento
  ![Diagrama Entidade Relacionamento](Diagramas/Diagrama2.png)

## 9 Protótipos
Foram criados protótipos das principais partes do site: área de contato, login, dicas e home page. Essas duas últimas são praticamente idênticas, já que a ideia de visualização do catálogo ou de posts sobre dicas de saúde é praticamente mesma.

Abaixo seguem os links para cada página, todos os protótipos  e seus códigos podem ser acessados [aqui](Prototipos).

  - [Login](Prototipos/Login.html)
  - [Contato](Prototipos/contato.html)
  - [Dicas](Prototipos/Dicas.html)
  - [Home Page](Prototipos/index.html)

## 10 Cronograma
O cronograma abaixo mostra o planejamento do projeto entre os meses de Junho e Julho.

|           | Documentação | Pesquisa | Implementação | Testes |
|:---------:|:------------:|:--------:|:-------------:|:------:|
|  *Semana 1* |       X      |     X    |       X       |    X   |
|  *Semana 2* |       X      |     X    |               |        |
|  *Semana 3* |       X      |     X    |               |        |
|  *Semana 4* |       X      |     X    |       X       |        |
|  *Semana 5* |       X      |     X    |       X       |    X   |
|  *Semana 6* |       X      |     X    |       X       |        |
|  *Semana 7* |       X      |     X    |       X       |        |
|  *Semana 8* |       X      |     X    |       X       |        |
|  *Semana 9* |       X      |     X    |       X       |    X   |
| *Semana 10* |       X      |     X    |       X       |    X   |

## 11 Referências
  - [Shop Homepage Template](http://startbootstrap.com/template-overviews/shop-homepage/)
  - [Loja Digital Nutri](https://www.facebook.com/Loja-Digital-Nutri-892444520871747)
  - [Dia Diagram Editor](http://dia-installer.de/)
  - [Ponto Natural Shop](http://pontonaturalshop.com.br)
  - [Laravel Framework](https://laravel.com/)







