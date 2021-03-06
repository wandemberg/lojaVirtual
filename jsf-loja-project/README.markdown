JSF Loja Project
=========================

Projeto simples de uma aplicação de Loja Virtual com `JSF 1.2`, `Spring 3.x` e `Hibernate 3.5.x` com o objetivo de explanar as principais features de cada tecnologia e como integra-las de maneira produtiva em um projeto real. O projeto é construído durante os cursos e treinamentos de **JSF 1.2, Spring e Hibernate** ministrados pela [TriadWorks](http://www.triadworks.com.br).

Caso tenha interesse ou alguma dúvida nos nossos cursos e treinamentos, por favor, [deixe-nos saber](http://www.triadworks.com.br/contatos.html).

Configurando o projeto e banco de dados.
----------------------------------------

Por padrão o projeto está configurado para o banco de dados `PostgreSQL`, mas já que se trata de uma aplicação com `Hibernate`, você pode simplesmente configura-lo para trabalhar com qualquer outro banco.

Os passos básicos são:

1. Importe o projeto no [Eclipse Java EE IDE for Web Developers (Galileo)](http://www.eclipse.org/downloads/) ou superior; 
2. Adicione o JDBC Driver no diretório `/WebContent/WEB-INF/lib` caso não pretenda utilizar o `PostgreSQL`;
3. Configure as informações do banco no arquivo `src/jdbc.properties`;
4. Crie o banco de dados `loja` e `loja_test` com a ferramenta de sua preferência (como o `PGAdmin`, no caso do `PostgreSQL`);
5. Faça o deploy no `Apache Tomcat 6.x` e inicie o servidor;
6. Insria um novo usuário no banco (tabela `USUARIO`) para que seja possível logar na aplicação;
7. Acesse a aplicação através da url [http://localhost:8080/loja](http://localhost:8080/loja) ;
8. Faça o login com o usuário criado;

Gerando .war da aplicação
------------------------
1. Para gerar o `.war` da aplicação basta executar o ant script (`build.xml`) no Eclipse ou na linha de comando:

		$ ant

2. Após ter executado o ant script o `.war` será gerado em `/target/war/snapshot/loja.war`;

