
# Trabalho Pratico de Engenharia de Software / Primeira-Entrega

## <center>Documento de Requisitos</center>


                     






## Locavideo: Análise de Requisitos


	Histórico de Revisões



|       Data       |Versão           |Descrição             |Autor   			                                                         |
|--------------------|-------------------------------|-----------------------------|-----------------------------|
|12/12/2017	     | 1.0           	   |Criação de Documento de Requisitos                    | Equipe
|14/12/2017          | 1.1        |Atualização Requisitos          | Equipe
|15/12/2017 	   |1.2	         	   |Criação do Índice      		 | Gláucio Gonçalves
|03/01/2018          |1.3|Pequenas correções| Lucas Lima
|04/01/2018         | 1.4        |Atualização Requisitos          | Flávio Gonçalves
|05/01/2018 	   |1.5	         	   |Atualização Requisitos   		 | Glaucio Gonçalves
|06/01/2018          |1.6|Pequenas Correções  | Lucas Lima
|07/01/2018          |1.7|Atualização Requisitos  | Lucas Lima
|09/01/2018          |1.8|Atualização Requisitos   | Flávio Gonçalves
|10/01/2018          |1.9|Atualização Requisitos   | Édlon Sá
|13/01/2018          |2.0|Atualização Requisitos Segundo Release  | Édlon Sá
|15/01/2018          |2.1|Pequenos Ajustes | Lucas Lima

**Sumário**
1. [           Introdução](#id1)
2. [Requisitos](#id2)

<div id='id1' />

## 1. Introdução	

#### 1.1 . Objetivos

Este documento visa os clientes e desenvolvedores envolvidos na criação do sistema denominado LocaVídeo. Objetiva demonstrar todos os processos e serviços que o envolvem, incluindo funcionalidades e restrições com o intuito de auxiliar o processo de desenvolvimento do mesmo. O presente documento demonstra todos os requisitos funcionais e não funcionais.

### 1.2. Escopo da Aplicação

Nossa proposta está em trazer um produto que visa considerar todos os aspectos importantes de mercado e entregar coesão e integridade para o gerenciamento comercial de locação de filmes, automatizando processos e entregando um sistema ideal para a locação de filmes de forma simplificada e intuitiva,  foi criado um site utilizando PHP, interligado ao banco de dados.


<div id='id2' />

## 2. Requisitos

	Requisitos Gerais



|       Código       |Nome               |Descrição             |Prioridade        			                                                         |
|--------------------|-------------------------------|-----------------------------|-----------------------------|
|RF-01(1) 	     | Alugar Título           	   | Locação.                    | Essencial
|RF-02(1)          | Pagar Título         |Quitação.          | Essencial
|RF-03(1)  	   |Devolver Título         	   |Devolução.        		 | Essencial
|RF-04(1)          |Cadastro Administrador|Cadastro de Usuário Admistrador do Sistema	| Essencial
|RF-05(1)          |Alterar Administrador|Modificar cadastro do administrador| Essencial
|RF-06(1)          |Alterar Recupera Senha do Administrador|Recupera Senha do Administrador caso ele Perca| Essencial
|RF-07(1)          |Exclui Administrador| Exclui um Administrador do Sistema| Essencial
|RF-08(1)          | Cadastro Usuário |Cadastro de Usuário| Essencial
|RF-09(1)          |Alterar Usuário|Modificar cadastro do administrador| Essencial
|RF-10(1)          |Excluir Usuário|Remover Cadastro do Usuário| Essencial
|RF-11(1)          |Cadastro Título|Cadastro do Título| Essencial
|RF-12(1)          |Alterar Título| Modificar cadastro do Título | Essencial
|RF-13(1)          |Excluir Título | Remover Cadastro do Título  | Essencial
|RF-14(1)          |Lista Cliente| Listar Clientes Cadastrados| Essencial
|RF-15(1)          |Lista Títulos| Lista de Títulos Cadastrados| Essencial
|RF-16(1)          |Lista Administradores| Lista Administradores Cadastrados| Essencial
|RF-17(1)          |Cadastrar Preço do Título|Cadastra um peço para todos os Títulos|Essencial
|RF-18(1)          |Alterar Preço do Título|Altera o preço para todos os Títulos|Essencial
|RF-19(1)          |Total de Títulos Alugados|Mostra o total de Títulos Alugados| Essencial
|RF-20(1)          |Total de Título cadastrados| Mostra o total de Títulos cadastrados|Essencial


	Requisitos Não-funcionais
|       Código       |Nome               |Descrição             |Prioridade        			                                                         |
|--------------------|-------------------------------|-----------------------------|-----------------------------|
|RNF-01(1) 	     |Segurança         	   | Operações só serão realizadas através de Usuários autentificados.                   | Essencial
|RNF-02(1)          | Interface        |Sistema de interface intuitiva.          | Essencial
|RNF-03(1)  	   |Operacional         	   |Sistema deve ser Desenvolvido em PHP.        		 | Essencial
|RF-03(2)          |Operacional|Sistema deve ser compatível com os navegadores existentes.| Essencial

## 3. Detalhamento dos Casos de Uso
Interações dos usuários com o sistema.
#### 3.1 Caso de Uso I – Cadastrar Cliente
  - **Nível:** Administrador ou Usuário
  - **Atores primários:** Administrador e Usuário 
  - **Interessados:** Administrador e Usuário
    - **Administrador:** Efetuação de cadastro do Usuário para ter acesso ao sistema.
    - **Usuário:** Efetuação de cadastro do Usuário para ter acesso ao sistema.
  - **Pré-condições:** ?
  - **Garantias de sucesso:** Usuário e Clientes criados no sistema. 
  - **Cenário de sucesso principal:**
	1. Usuário tem acesso à página de Login;
	2. Usuário acessa a opção de Lista de Clientes;
	3. Usuário pressiona o botão Cadastrar Clientes
	4. Usuário preenche os campos do formulário de cadastro ;
	5. Usuário finaliza o cadastro;
	6. Mensagem do sistema confirmando o cadastro;
  - **Extensões:** 
    - Passos 3 a 5: Campos preenchimento indevido:
        - Processo de cadastro é interrompido;
        - Usuário recebe informações relacionadas ao problema encontrado. 
#### 3.2 Caso de Uso II – Cadastrar Título
 - **Nível:** Administrador e Usuário
 - **Atores primários:** Administrador e Usuário
 - **Interessados:** Administrador e Usuário
	- **Administrador:** Realização de Cadastro corretamente ao banco de dados.
 - **Pré-condições:**
 - **Garantia de sucesso:** Títulos cadastrados corretamente ao banco de dados. 
 - **Cenário de sucesso principal:**
	 1. Usuário tem acesso a página web;
	 2. Usuário acessa a opção Cadastrar Título ; 
	 3. Usuário preenche os campos do formulário de cadastro, seleciona o gênero e seleciona o arquivo de Imagem;
	 4. Usuário envia dados;
	 5. Mensagem confirmando o cadastro.
 - **Extensões:** 
    - Passos 3 a 5: Preenchimento incorreto dos campos
	     - Cadastro é interrompido;
	     - Usuário recebe informação relacionado ao problema encontrado.

#### 3.3 Caso de Uso III – Editar Cliente
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
        - Autentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas;
    - Passos 5 a 6: Preenchidos indevidamente:
        - Alteração interrompida.
        - Usuário recebe informação relacionada ao problema encontrado.

#### 3.4 Caso de Uso IV – Editar Filme
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
        - Autentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas;
    - Passos 5 a 6:  Preenchidos indevidamente:
        - Alteração interrompida;
        - Usuário recebe informação relacionada ao problema encontrado.

#### 3.5 Caso de Uso V – Remoção de Usuário
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
    3. Administrador acessa a opção Lista de Clientes;
    4. Administrador busca usuário à ser removido;
    5. Administrador escolhe a opção remover;
    6. Administrador confirma a remoção do usuário;
    7. Usuário é removido, banco de dados atualizado;
    8. Mensagem confirmando a remoção.
 - **Extensões:** 
    - Passo 2: Usuário ou senha incorretos:
        - Autentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas.
    - Passo 4:  Usuário inexistente;
	    - Mensagem informando que usuário não existe.
	    - 
#### 3.6 Caso de Uso VI – Cadastrar Gênero
 - **Nível:** Administrador ou Usuário
 - **Atores primários:** Administrador ou Usuário
 - **Interessados:** 
    - **Administrador:**  Cadastro do Gênero do Título
    - **Usuário:** Cadastro do Gênero do Título
 - **Pré-condições:** 
    - Usuário tem acesso a página de Login;
    - Usuário com Login autorizado.
 - **Garantias de sucesso:** 
    - Remoção do Gênero do banco de dados. 
    - Mensagem de confirmando do cadastro;
 - **Cenário de sucesso principal:**
    1. Usuário tem acesso a página de Login;
    2. Usuário tem Login autenticado;
    3. Usuário acessa a opção Controle Gênero;
    4. Usuário escolhe cadastrar Gênero na caixa de Seleção ;
    5. Usuário preenche o formulário;
    6. Usuário pressiona botão Cadastrar Gênero
    7. Gênero é incluído, banco de dados atualizado;
    8. Mensagem confirmando a inclusão.
 - **Extensões:** 
    - Passo 2: Usuário ou senha incorretos:
        - Autentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas.
        - 
#### 3.7 Caso de Uso VII – Remover Gênero
 - **Nível:** Administrador ou Usuário
 - **Atores primários:** Administrador ou Usuário
 - **Interessados:** 
    - **Administrador:**  Remover Gênero do Título
    - **Usuário:** Remover Gênero do Título
 - **Pré-condições:** 
    - Usuário tem acesso a página de Login;
    - Usuário com Login autorizado.
 - **Garantias de sucesso:** 
    - Remoção do Gênero do Título do banco de dados. 
    - Mensagem de confirmando a exclusão;
 - **Cenário de sucesso principal:**
    1. Usuário tem acesso a página de Login;
    2. Usuário tem Login autenticado;
    3. Usuário acessa a opção Controle Gênero;
    4. Usuário escolhe Deletar Gênero na caixa de Seleção ;
    5. Usuário pressiona botão de confirmação;
    6. Mensagem confirmando a inclusão;
 - **Extensões:** 
    - Passo 2: Usuário ou senha incorretos:
        - Autentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas.
        - 
#### 3.8 Caso de Uso VIII – Logar
 - **Nível:** Administrador ou Usuário
 - **Atores primários:** Administrador, Usuário
 - **Interessados:** 
    - **Administrador:** Autentificação no sistema.
    - **Usuário:** Autentificação no sistema.
 - **Pré-condições:** 
    - Usuário tem acesso a página de Login;
    - Usuário existente.
 - **Garantias de sucesso:** 
    - Login na página de acesso ao sistema.
 - **Cenário de sucesso principal:**
      1. Usuário tem acesso a página de Login;
      2. Usuário informa Login e senha;
      3. Usuário pressiona o botão Entrar;
      4. Usuário redirecionado para a página principal do sistema.
 - **Extensões:** 
    - Passo 2: Usuário ou senha incorretos:
        - Autentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas.     
      
  #### 3.9 Caso de Uso I – Lista Cliente
  - **Nível:** Administrador ou Usuário
  - **Atores primários:** Administrador e Usuário 
  - **Interessados:** Administrador e Usuário
    - **Administrador:** Listar Clientes cadastrados no sistema.
    - **Usuário:** Listar Clientes cadastrados no sistema.
  - **Pré-condições:** ?
  - **Garantias de sucesso:** Listar Clientes cadastrados no sistema.
  - **Cenário de sucesso principal:**
	1. Usuário tem acesso à página de Login;
	2. Usuário informa Login e senha;
	3. Usuário acessa a opção de Lista de Clientes;
	4. Usuário tem acesso a lista de Clientes.
  - **Extensões:** 
     - Passo 2: Usuário ou senha incorretos:
        - Autentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas.  
   

  #### 3.1 Caso de Uso I – Lista Títulos
  - **Nível:** Administrador ou Usuário
  - **Atores primários:** Administrador e Usuário 
  - **Interessados:** Administrador e Usuário
    - **Administrador:** Listar Títulos cadastrados no sistema.
    - **Usuário:** Listar Títulos cadastrados no sistema.
  - **Pré-condições:** ?
  - **Garantias de sucesso:** Listar Títulos cadastrados no sistema.
  - **Cenário de sucesso principal:**
	1. Usuário tem acesso à página de Login;
	2. Usuário informa Login e senha;
	3. Usuário acessa a opção de Lista de Filmes;
	4. Usuário tem acesso a lista de Filmes.
  - **Extensões:** 
     - Passo 2: Usuário ou senha incorretos:
        - Autentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas.  
        
#### 3.1 Caso de Uso I – Lançar Preço
  - **Nível:** Administrador ou Usuário
  - **Atores primários:** Administrador e Usuário 
  - **Interessados:** Administrador e Usuário
    - **Administrador:** Lançar valor locação de Título.
    - **Usuário:** Lançar valor locação de Título.
  - **Pré-condições:** ?
  - **Garantias de sucesso:** Registrar valor locação de Título no sistema.
  - **Cenário de sucesso principal:**
	1. Usuário tem acesso à página de Login;
	2. Usuário informa Login e senha;
	3. Usuário acessa a opção Preço e Desconto;
	4. Usuário escolhe a opção Incluir Preço na caixa de seleção;
	5. Usuário preenche os campos do formulário.
	6. Usuário confirma lançamento.
  - **Extensões:** 
     - Passo 2: Usuário ou senha incorretos:
        - Autentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas.  
        - 
#### 3.1 Caso de Uso I – Alterar Preço
  - **Nível:** Administrador ou Usuário
  - **Atores primários:** Administrador e Usuário 
  - **Interessados:** Administrador e Usuário
    - **Administrador:** Alterar valor locação de Título.
    - **Usuário:** Alterar valor locação de Título.
  - **Pré-condições:** ?
  - **Garantias de sucesso:** Registrar alteração valor locação de Título no sistema.
  - **Cenário de sucesso principal:**
	1. Usuário tem acesso à página de Login;
	2. Usuário informa Login e senha;
	3. Usuário acessa a opção Preço e Desconto;
	4. Usuário escolhe a opção Alterar Preço na caixa de seleção;
	5. Usuário altera os campos do formulário;
	6. Usuário confirma alteração.
  - **Extensões:** 
     - Passo 2: Usuário ou senha incorretos:
        - Autentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas.  
        
#### 3.1 Caso de Uso I – Alterar Desconto
  - **Nível:** Administrador ou Usuário
  - **Atores primários:** Administrador e Usuário 
  - **Interessados:** Administrador e Usuário
    - **Administrador:** Alterar valor desconto de Título.
    - **Usuário:** Alterar valor desconto de Título.
  - **Pré-condições:** ?
  - **Garantias de sucesso:** Registrar alteração valor locação de Título no sistema.
  - **Cenário de sucesso principal:**
	1. Usuário tem acesso à página de Login;
	2. Usuário informa Login e senha;
	3. Usuário acessa a opção Preço e Desconto;
	4. Usuário escolhe a opção Alterar Preço na caixa de seleção;
	5. Usuário altera os campos do formulário;
	6. Usuário confirma alteração.
  - **Extensões:** 
     - Passo 2: Usuário ou senha incorretos:
        - Autentificação não é realizada;
        - Notificação de erro ao Usuário;
        - Informações novamente solicitadas.  
#### 3.10 Caso de Uso VII – Locação do Título
 - **Nível:** 
 - **Atores primários:** 
 - **Interessados:** 
 - **Pré-condições:** 
 - **Garantias de sucesso:** 
 - **Cenário de sucesso principal:**
    
 - **Extensões:** 
<div id='id3' />

### 11 Referências

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTc3NzQyMjE1NF19
-->
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTg5MjY5NjUxMF19
-->