# Trabalho-Pratico-de-Engenharia-de-Software---Primeira-Entrega

# LocaVdeo: Análise de Requisitos

## 1. Introdução	

## 1.1 . Objetivos

Este documento visa os clientes e desenvolvedores envolvidos na criação do sistema denominado LocaVídeo. Objetiva demonstrar todos os processos e serviços que o envolvem, incluindo funcionalidades e restrições com o intuito de auxiliar o processo de desenvolvimento do mesmo. O presente documento demonstra todos os requisitos funcionais e não funcionais.

~~Objetivando automatizar o sistema de locação de filmes desenvolvemos o software LocaVídeo que busca abranger todos os aspectos que envolvem o empréstimo de filmes. Possibilitando o gerenciamento de aluguel de filmes que irá suprir as necessidades, permitindo cadastros de Clientes, Catálogo de Filmes, Tela de Login, registros de empréstimo e devolução.~~ 

## 1.2. Escopo da Aplicação

Nossa proposta está em trazer um produto que visa considerar todos os aspectos importantes de mercado e entregar coesão e integridade para o gerenciamento comercial de locação de filmes, automatizando processos e entregando um sistema ideal para a locação de filmes de forma simplificada e intuitiva,  foi criado um site utilizando PHP, interligado ao banco de dados que será empregado para utilização dos usuários. 

~~O ambiente comercial atual requer formas práticas, funcionais e confiáves quando se trata de entregar um produto ou serviço idependente do ramo em que o mesmo é utilizado.~~ 
## 2. Requisitos

	Requisitos Gerais


|       Código       |Nome               |Descrição             |Prioridade        			                                                         |
|------------------|-------------------------------|-----------------------------|-----------------------------|
| RF-01(1) | Alugar Título           | Locação.            | Essencial
|RF-02(1)         | Alugar e Pagar Título            |Locação e quitação.            | Essencial
|RF-03(1)          |Reservar Título|Agendar locação.  | Essencial
|RF-04(1)   |Devolver Título         |Devolução.        | Essencial
|RF-05(1)           |Devolver Título Com Atraso.         |Devolução com Atraso.	| Essencial
|RF-06(1)           | Não Devolver|Título não é devolvido.| Essencial
|RF-07(1)            |Título Inexistente|Título não existente no acervo.	| Essencial
|RF-08(1)           |Cadastro Administrador|Cadastro de Usuário Admistrador do Sistema	| Essencial
|RF-09(1)         |Alterar Administrador|Modificar cadatro do admi	nistrador| Essencial
|RF-10(1)        | Cadastro Usuário |Cadastro de Usuário| Essencial
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|




## 3. Detalhamento dos Casos de Uso
Interações dos usuários com o sistema.
### 3.1 Caso de Uso I – Cadastrar Cliente
  - **Nível:** Administrador ou Usuário
  - **Atores primários:** Administrador e Usuário 
  - **Interessados:** Administrador e Usuário
    - **Administrador:** Efetuação de cadastro do Usuário para ter acesso ao sistema.
    - **Usuário:** Efetuação de cadastro do Usuário para ter acesso ao sistema.
  - **Pré-condições:** ?
  - **Garantias de sucesso:** Usuário e Clientes criados no sistema. 
  - **Cenário de sucesso principal:**
	1. Usuário tem acesso á página de Login;
	2. Usuário acessa a opção de Cadastro de Cliente;
	3. Usuário preenche os campos do formulário de cadastro ;
	4. Usuário finaliza o cadastro;
	5. Mensagem do sistema confirmando o cadastro;
  - **Extensões:** 
    - Passos 3 a 5: Campos preenchimento indevido:
        - Processo de cadastro é interrompido;
        - Usuário recebe informações relacionadas ao problema encontrado. 
### 3.2 Caso de Uso II – Cadastrar Filme
 - **Nível:** Administrador e Usuário
 - **Atores primários:** Administrador e Usuário
 - **Interessados:** Administrador e Usuário
	- **Administrador:** Realização de Cadastro corretamente ao banco de dados.
 - **Pré-condições:**
 - **Garantia de sucesso:** Filmes cadastrados corretamente ao banco de dados. 
 - **Cenário de sucesso principal:**
	 1. Usuário tem acesso a página web;
	 2. Usuário acessa a opção Cadastrar Filme ; 
	 3. Usuário preenche os campos do formulário de cadastro;
	 4. Usuário Finaliza o cadastro;
	 5. Mensagem confirmando o cadastro.
 - **Extensões:** 
    - Passos 3 a 5: Preenchimento incorreto dos campos
	     - Cadastro é interrompido;
	     - Usuário recebe informação relacionado ao problema encontrado.

### 3.3 Caso de Uso III – Editar Cliente
 - **Nível:** Administrador ou Usuário
 - **Atores primários:** Administrador ou Usuário
 - **Interessados:** 
  - **Usuário:** Alterações de campos editáveis.
 - **Pré-condições:** Usuários com Login autorizado.
 - **Garantias de sucesso:**
    - Alteração realizada, banco de dados atualizado. 
    - Alteração realizada podendo ser visualizada no sistema.
 - **Cenário de sucesso principal:**
      1. Usuário tem acesso a página de Login;
      2. Usuário tem Login autenticado;
      3. Usuário acessa a opção Lista de Clientes;
      4. Usuário  acessa o cadastro de Cliente desejado;
      5. Usuário  modifica o campo desejado;
      6. Usuário  finaliza a alteração;
      7. Mensagem confirmando a alteração;
      8. Cadastro do Cliente é atualizado.
  - **Extensões:** 
    - Passo 3: Usuário ou senha incorretos:
        - Atentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas;
    - Passos 5 a 6: Preenchidos indevidamente:
        - Alteração interrompida.
        - Usuário recebe informação relacionada ao problema encontrado.

### 3.4 Caso de Uso IV – Editar Filme
 - **Nível:** Administrador ou Usuário
 - **Atores primários:** Administrador ou Usuário
 - **Interessados:** 
    - **Administrador:** Alterações de campos editáveis.
 - **Pré-condições:** Usuários com Login autorizado.
 - **Garantia de sucesso:** 
    - Alteração realizada, banco de dados atualizado.
    - Atualização do valor do campo exibido no sistema.
 - **Cenário de sucesso principal:**
    1. Usuário tem acesso a página de Login;
    2. Usuário acessa a opção Lista de Filmes;
    3. Usuário acessa o cadastro do Filme desejado;
    4. Usuário  modifica o campo desejado;
    5. Usuário  finaliza a alteração;
    6. Mensagem de confirmando a alteração;
    7. Usuário confirma a edição;
    8. Cadastro do Filme é atualizado.
 - **Extensões:**
    - Passo 3: Usuário ou senha incorretos:
        - Atentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas;
    - Passos 5 a 6:  Preenchidos indevidamente:
        - Alteração interrompida;
        - Usuário recebe informação relacionada ao problema encontrado.

### 3.5 Caso de Uso V – Remoção de Usuário
 - **Nível:** Administrador
 - **Atores primários:** Administrador
 - **Interessados:** 
    - **Administrador:** Remover um usuário cadastrado.
 - **Pré-condições:** 
    - Usuário tem acesso a página de Login;
    - Usuário tem acesso de Administrador.
 - **Garantias de sucesso:** 
    - Remoção do Usuário do banco de dados. 
    - Mensagem de confirmando a exclusão;
 - **Cenário de sucesso principal:**
    1. Administrador tem acesso a página de Login;
    2. Administrador tem Login autenticado;
    3. Adminstrador acessa a opção Lista de Clientes;
    4. Administrador busca usuário à ser removido;
    5. Administrador escolhe a opção remover;
    6. Administrador confirma a remoção do usuário;
    7. Usuário é removido, banco de dados atualizado;
    8. Mensagem confirmando a remoção.
 - **Extensões:** 
    - Passo 2: Usuário ou senha incorretos:
        - Atentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas.
    - Passo 4:  Usuário enexistente;
	    - Mensagem informando que usuário não existe.

### 3.6 Caso de Uso VI – Logar
  - **Nível:** Administrador ou Usuário
  - **Atores primários:** Administrador, Usuário
  - **Interessados:** 
    - **Administrador:** Autentificação no sistema.
    - **Cliente:** Autentificação no sistema.
  - **Pré-condições:** 
    - Acesso à página de Login. 
    - Usuário existente .
  - **Garantia de sucesso:** Login na página de acesso ao sistema.
  - **Cenário de sucesso principal:**
      1. Usuário tem acesso a página de Login;
      2. Usuário informa Login e senha;
      3. Usuário pressiona o botão Entrar;
      4. Usuário redirecionado para a página principal do sistema.
      
  - **Extensões:** 
    - Passos 2 e 3: 
        - Autentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas.
### 3.7 Caso de Uso VII – Aluguel de Filme
 - **Nível:** 
 - **Atores primários:** 
 - **Interessados:** 
 - **Pré-condições:** 
 - **Garantias de sucesso:** 
 - **Cenário de sucesso principal:**
    
 - **Extensões:** 
  
### 3.8 Caso de Uso VIII – Tabela de Filmes
  - **Nível:** 
  - **Atores primários:** 
  - **Interessados:**
    - **Administrador:**
    - **Cliente:** 
  - **Pré-condições:** 
   - **Garantias de sucesso:** 
      - **Cenário de sucesso principal:**
 
  - **Extensões:**

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







<!--stackedit_data:
eyJoaXN0b3J5IjpbMjA3NzY4MTE3MF19
-->