Automacao de testes API - ServeRest

Automacao de testes API. Baseado em uma aplicacao que gerencia informacoes de usuários (Criacao, ataulizacao, exclusao e leitura de usuários). Aplicacao é baseada em uma API RESTfull para as seguintes operacoes:

- GET/users: Retorna lista de todos os usuarios;
- POST/users: Cria um novo usuário;
- GET/users/{id}: Retorna detalhes do usuário especifico;
- PUT/users/{id}: Atualiza informacoes do usuário;
- DELETE/users/{id}: Exclui usuário.

API utilizada: https://serverest.dev/#/

*Pré-requisitos - O que é preciso?*

Ferramente de testes de API - Postman
Acesso ao GitHub

*Pré-requisitos: Como instalar*

Postman
1.	Acesse https://www.postman.com/downloads.
2.	Clique em "Download" de acordo com o sistema operacional da sua máquina.
3.	Abra o arquivo .exe baixado e siga as instruções do instalador.
4.	Abra o Postman e crie uma conta.
5.	Pronto! O Postman estará disponível e pronto para uso.

GitHub
1.	Acesse https://git-scm.com/download/win.
2.	Baixe o arquivo .exe.
3.	Execute o arquivo e siga as instruções do instalador.
4.	Abra o GitHub e crie uma conta.
5.	Pronto! O GitHub estará disponível e pronto para uso.

*Pré-requisitos: Criar cenários e scripts de testes no Postman*

1 - Escrever cenários e scripts de teste
       - Utilize o Postman para criar os cenários e escrever os scripts de teste.
2 - Organizar requests em collections
       - Na lateral esquerda da tela, é possível criar collections e adicionar requests a elas, organizando em pastas conforme preferir.
3 - Configurar requests de acordo com o contrato
       - Ao adicionar uma request, configure-a conforme o contrato que servirá de base para os testes.
4 - Escrever scripts de validação
       - Na aba "Scripts", escreva todos os cenários de teste que devem ser validados para aquela request.
5 - Validar cenários e scripts
       - Após finalizar a configuração da request e os scripts, valide os testes pelo próprio Postman.
       - Clique sobre a collection e utilize a opção "Run" para executar os testes.
6 - Verificar resultados
       - Ao rodar os testes, você terá os cenários e scripts validados, com o status 'passed' ou 'failed'.

*Pré-requisitos: Criar repositório e integrar a pipeline para geração de relatórios de testes*

1 - Criar o repositório no GitHub
       - Acesse o GitHub e clique em "Criar repositório".
       - Defina o nome do repositório e escolha se será público ou privado.
       - Clique em "Criar" e o repositório estará pronto.
2 - Configurar o workflow para execução automatizada dos testes
       - No repositório, clique em "Actions" e depois em "New workflow".
       - Configure o workflow conforme desejado (o GitHub oferece opções de configuração simples ou padrão).
3 - Configurar arquivo YAML para relatórios
       - Ajuste o arquivo .yaml de acordo com a ferramenta de relatório escolhida (por exemplo, Newman + Allure Report).
4 - Executar a automação
       - Com o workflow configurado e o YAML pronto, o ambiente do GitHub estará preparado para rodar a automação e gerar os relatórios automaticamente.

*Executando a automação*

1.	Upload dos arquivos do Postman
	      - Com o ambiente configurado, faça o upload dos arquivos .json gerados pelo Postman.
	      - Verifique se os nomes dos arquivos correspondem aos nomes definidos no arquivo .yaml do workflow.
2.	Executar o workflow
       - Clique em "Actions" no repositório do GitHub.
       - Selecione o workflow previamente criado.
       - 	Clique em "Run workflow" para iniciar a automação.
3.	Aguardar execução e conferir relatório
       - Aguarde a automação ser executada.
       - Ao final, será gerado um relatório com os resultados dos testes, mostrando os status passed ou failed.

*Analise os testes*

Esta automação cobre 56 cenários de teste da API ServeRest, validando tanto os cenários esperados conforme o contrato, schema, quanto aos cenários negativos, garantindo que a API se comporte corretamente em situações inesperadas. Os testes fazem uso de variáveis de ambiente, o que permite executá-los sem necessidade de alterar informações nos requests, mesmo com múltiplos cenários distintos. Além disso, realizam validações completas dos responses, assegurando que os retornos da API estejam corretos, com os campos preenchidos e os status codes alinhados ao contrato. A automação inclui também três cenários que apresentam status failed, evidenciando divergências entre o schema definido no contrato e o retorno real da aplicação.


*Autor*
- Teste automatizado integrado à pipeline: Carlos Castro
- Documentação: Carlos Castro





Um desenvolvedor - Trabalho Inicial - umdesenvolvedor
Fulano De Tal - Documentação - fulanodetal
Você também pode ver a lista de todos os colaboradores que participaram deste projeto.

