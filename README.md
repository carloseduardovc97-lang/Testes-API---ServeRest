Automacao de testes API - ServeRest

Automacao de testes API. Baseado em uma aplicacao que gerencia informacoes de usuários (Criacao, ataulizacao, exclusao e leitura de usuários). Aplicacao é baseada em uma API RESTfull para as seguintes operacoes:

- GET/users: Retorna lista de todos os usuarios;
- POST/users: Cria um novo usuário;
- GET/users/{id}: Retorna detalhes do usuário especifico;
- PUT/users/{id}: Atualiza informacoes do usuário;
- DELETE/users/{id}: Exclui usuário.

API utilizada: https://serverest.dev/#/


📋 Pré-requisitos - O que é preciso?

Ferramente de testes de API - Postman
Acesso ao GitHub

 Pré-requisitos - Como instalar?

Postman
- Acesse https://www.postman.com/downloads;
- Clique em "download" (de acordo com sistema operacional da sua máquina);
- Abra o arquivo .exe baixado;
- Execute o arquivo .exe de acordo com a orientacao do instalador;
- Abra o Postman;
- Crie uma conta;
- Pronto, diposnivel para navegar na ferramenta.

GitHub

- Acesse https://git-scm.com/download/win;
- Baixe o arquivo .exe
- Execute o arquivo .exe de acordo com a orientacao do instalador;
- Abra o GitHub;
- Crie uma conta;
- Pronto, também disponivel para navegar na ferramenta


 Pré-requisitos - Criar cenários e scripts de testes no Postman

- Escrever os cenários e os scripts de testes utilizando a ferramenta do Postman.
- A esquerda da tela é possivel criar collections e adicionar as request a elas, separando por pasta, conforme ache mais organizado.
- Ao adicionar uma request, é possivel configura-la de  acordo com o contrato que baseará os testes
- Na aba "scripts", voce consegue escrever todos os cenários de testes que serão validados
- Após finalizar a request de acordo com o contrato e com os scripts prontos 
- Valide os cenários e scripts de testes pelo proprio Postman, clicando em cima da collectins, habilitará as algumas opcoes, dentre elas, a "Run"
- Pronto, terá os seus cenários e scripts validados, com os status de 'passed' ou 'failed'.

 Pré-requisitos - Criar repositorio e integrar a pipeline, gerando relatórios dos testes

- Já no ambiente GitHub, clique em criar repositório
- Voce definira o nome, perfil privado ou publico do seu repositorio
- Depois clicara em 'criar', pronto repositório criado.
- Após isso, você criar um workflow, ambiente que rodará seus teste de forma automatizada
- Clicara em áctions"
  
  
⚙️ Executando os testes

- Escrever os cenários e os scripts de testes utilizando a ferramenta do Postman.
- Valide os cenários e scripts de testes pelo proprio Postman pra ter um visao dos status final dos testes, passed ou failed.
- Apos isso, exporte as collections utilizadas nos testes, incluindo a collection de ambiente, a qual ficam guardadas todas as variaveis utilizadas.
- 


🔩 Analise os testes de ponta a ponta

Explique que eles verificam esses testes e porquê.

Dar exemplos
⌨️ E testes de estilo de codificação

Explique que eles verificam esses testes e porquê.





*Autor* 

Teste automatizado integrado a pipeline - Carlos Castro
Documentacao - Carlos Castro




Um desenvolvedor - Trabalho Inicial - umdesenvolvedor
Fulano De Tal - Documentação - fulanodetal
Você também pode ver a lista de todos os colaboradores que participaram deste projeto.

