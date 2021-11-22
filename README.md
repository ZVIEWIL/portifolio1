
## LISTA COM O LINK DOS PORTFÓLIOS DOS APIs:
[API 1° SEMESTRE - **DANZO - Mapeador de Criminalidade ao Redor da FATEC**](https://github.com/ZVIEWIL/portifolio1) 

[API 2° SEMESTRE - **GANTT CHART**](https://github.com/ZVIEWIL/portifolio2)

[API 3° SEMESTRE - **CADASTRO POSITIVO**](https://github.com/ZVIEWIL/portifolio3)

# API do 1° SEMESTRE - ***DANZO - Mapeador de Criminalidade ao Redor da FATEC***

### **RESUMO DO PROJETO**

Iniciamos essa caminhada dos APIs com o desafio de criar um WEB BOT que realizaria alguma tarefa definida pelo grupo, ou seja, tema aberto. 
Visando uma contribuição com a comunidade de estudantes da Fatec, resolvemos desenvolver um web bot que disponibiliza os dados em uma página na Internet sobre o índice de violência na região da FATEC e Parque Tecnológico.

Inicialmente, os usuários seriam os alunos da FATEC e a página seria aberta, sem precisar realizar cadastro ou login na página. 
Ao entrar na página, o usuário tem acesso às informações de acordo com as opções de entrada, podendo inicialmente fazer o filtro do período (ex: de junho/2019 a agosto/2019 e o tipo de violência (ex: tentativa de ou, furto/roubo de carro, celulares, pertences pessoais etc.). 
Essas informações são indicadas em um mapa de calor para melhor visualização.

Tela Inicial:
![Screenshot_1](https://user-images.githubusercontent.com/54503903/142784348-aee4f7b9-0949-4a91-a9e6-b8e6ba22415c.png)

Tela com os Filtros:
![Screenshot_2](https://user-images.githubusercontent.com/54503903/142784358-5455857c-d84e-48db-bff0-6ef6ff40029a.png)

Mapa de Calor gerado:
![Screenshot_4](https://user-images.githubusercontent.com/54503903/142784828-959113ea-7464-48f5-bbe3-4c786207929f.png)

Gráfico realizando comparação dos dados:
![Screenshot_5](https://user-images.githubusercontent.com/54503903/142791377-bc73d39c-81c8-42a1-b372-bcbaaaa0a70b.png)

### **TECNOLOGIAS UTILIZADAS**
#### **PYTHON**
Python é uma linguagem de programação de alto nível, desenvolvida por Guido van Rossum em 1991. Os objetivos desta linguagem são desenvolver códigos bom, ágil e objetiva. Além da linguagem de fácil interpretação o Python conta com uma biblioteca que fornece várias coleções de funções.
Para o desenvolvimento do Projeto Integrador (Web Bot), foi escolhida a linguagem Python pelos integrantes do grupo por estarem familiarizados e por recomendação dos professores. Foi utilizada para desenvolver as raspagens do bot, integração com o front end e conexão com o banco de dados.

Bibliotecas utilizadas:

- Flask: É um micro framework que utiliza a linguagem Python para criar aplicativos Web. Escolhemos utiliza-lo por causa de suas principais caracteristicas que são: simplicidade, rapidez no desenvolvimento.

- Selenium: Utilizado para acessar e realizar comandos no site da SSP/SP, de forma que fosse possível baixar o arquivo .CSV utilizado para alimentar o nosso banco de dados.

- SQlite: O SQLite é uma base de dados relacional de código aberto e que dispensa o uso de um servidor na sua atuação. Utilizamos para armazenar os dados extraidos do arquivo .csv obtido no site da SSP/SP.

- Pandas: O pandas é uma ferramenta de manipulação e análise de dados de código aberto rápida, poderosa, flexível e fácil de usar. Foi Utilizado para manipular os dados recebidos, agrupando eles por localização e tratando os dados para apresentação no mapa de calor.

- Folium: Biblioteca do Python utilizada para facilitar a visualização de dados de vetores/geolocalização em mapas. Utilizamos para gerar o Mapa de Calor através dos dados fornecidos pelo Banco de Dados.

- Flask_googlecharts: É utilizado para gerar gráficos. foi utilizado para gerar gráficos para realizarmos comparações mensais sobre o indíce de criminalidade na região.

### **CONTRIBUIÇÕES INDIVIDUAIS**
Com as divisões das tarefas feitas pela equipe, fiquei responsavel por tratar os dados vindos do arquivo .CSV e inseri-lo no BD. Como um colega da equipe acabou desistindo do curso, acabei acumulando a tarefa de realizar a raspagem dos dados no site da SSP/SP. Pra mim foi bastante desafiador realizar as 2 tarefas, pois nunca tive contato algum com desenvolvimento de softwares.
- Desenvolvimento do método que utilizamos para realizar a raspagem de dados no site da SSP/SP com o Selenium;
- Desenvolvimento do método utilizado para criar os diretórios para armazenar o arquivo .csv extraido;
- Desenvolvimento do método que utilizamos para inserir no banco de dados os dados extraidos do arquivo .csv;
- Desenvolvimento do método que utilizamos para gerar o mapa de calor;





Neste semestre, como estréia deste modelo de aprendizado (por projeto), havia ampla liberdade oriunda da amplitude do escopo. Ademais, o processo de criação e aprendizado tem velocidade diferente entre alunos.

Assim, implantamos uma metodologia que denominamos "competing codes". Dois colegas buscavam solução para o mesmo problema, vencendo o código que melhor atendesse as necessidades dos projetos.

Nesse processo, estudamos e aprendemos a respeito de diversas ferramentas e bibliotecas do Python que não foram utilizadas na solução em si (*v.g.* matplotlib).

Ao final, o webbot foi capaz de realizar as seguintes tarefas:

1 - Escolha do usuário na página DANZO;​

2 – Obtenção de dados do sítio Transparência SSP-SP;​

![20211026-205948](https://user-images.githubusercontent.com/61089745/141654319-476e8427-220e-482b-a289-de10f10399b3.png)

![20211026-210008](https://user-images.githubusercontent.com/61089745/141654347-d9c9a67f-6d83-42da-a74d-f9a642c87c6d.png)

![20211026-210019](https://user-images.githubusercontent.com/61089745/141654358-6f0af4f7-3206-4431-bd10-2083ab2060eb.png)

![20211026-210044](https://user-images.githubusercontent.com/61089745/141654366-f3a1d2ad-51ee-4cce-91b1-9d8532462026.png)

![20211026-210057](https://user-images.githubusercontent.com/61089745/141654374-478e1889-1416-4001-aa37-3ba2fe5bb306.png)


3 – Tratamento de arquivo obtido: criação de pasta local, renomeação;​

4 – Tratamento de dados: Leitura do arquivo obtido, coluna por coluna LISTAS, para  inserção em BD;​

![20211026-210117](https://user-images.githubusercontent.com/61089745/141654394-86b1efdc-3213-4dde-99bc-9aed04b2841f.png)

5 – Inserção incremental em BD Sqlite3;​

6 – Leitura do BD Sqlite3;​

7 – Apresentação dos dados: mapa de calor, barras; ​

![20211026-210136](https://user-images.githubusercontent.com/61089745/141654411-19785ac1-3ee0-417b-bef6-5846348bdd2d.png)


### **II - TECNOLOGIAS**

Em fase inicial do aprendizado, a equipe elegeu o Python por ser linguagem de programação de alto nível mais amigável ao programador.

No contexto do Python, contamos com a orientação do Docente e muita pesquisa em fóruns virtuais especializados para implementar blocos de códigos com propósito específico.

As bibliotecas mais importantes foram:

- Selenium: Emulação de ações humanas para acessar o sitio da Secretaria de Segurança Pública do Estado de São Paulo, baixando os dados das métricas de crimes em arquivo em formato .CSV, após escolher município, bairro, tipo de crime e período. Escolhemos os crimes contra o patrimônio (furto ou roubo), de aparelhos celulares, automóveis, casas ou estabelecimentos comerciais.

-  Pandas: Agrupamento de dados por localização, entregando os dados tratados para a apresentação em mapa de calor. Recebemos um curso extracurricular de "Python para Jornalistas", aprendendo as principais funcionalidades para demostrar dados com significância para o usuário final. aqui, nasceu para mim a curiosidade por Ciência de Dados.

-  Folium:  Biblioteca do Python que facilita a visualização dos dados em um mapa interativo, no projeto essa bibilioteca nos auxiliou a manipular os dados no mapa de calor que que mostrava as regiões que com mais índice de criminalidade ao redor da Fatec.

- Flask: É um framework para Python utilizado para desenvolver aplicação web, escolhemos o Flask pois possui uma arquitetura mais simples, possui menos configurações e rapidez no desenvolvimento, com um deadline curto de aprendizado.

- Flask_googlecharts: É uma biblioteca para geração de gráficos, por ser uma das melhores bibiliotecas de gráficos, utilizamos em nosso projeto para gerar os gráficos mensais do índice de criminalidade.

### **III - CONTRIBUIÇÕES INDIVIDUAIS.**

Na definição do MVP (MINIMUM VIABLE PRODUCT) participei ativamente nas decisões de que tipo de criminalidade deveríamos enfatizar, por morar na região da FATEC, pude contribuir em informar os roubos que mais acontecem nessa região. Ficando definido o mapeamento por de roubo de Veículos, furto de veículos e roubo de celular.

![20211026-202145](https://user-images.githubusercontent.com/61089745/141654512-9f4b0c92-4ff9-4652-ba2d-e76891106934.png)


Como eu estava vindo da área administrativa, sem ter contato com a parte de programação, foi desafiador o aprendizado de uma linguagem backend e o contato com o banco de dados. Portanto como alguns integrantes da equipe já estavam mais familiarizados com essas tecnologias eu assumi o front-end do projeto. Ingressei em cursos online para entender como funcionava uma aplicação web e acabei trazendo as tecnologias de HTML, Bootstrap e GoogleChart para o Projeto Web bot Danzo.

O HTML: É uma linguagem de marcação utilizada na construção de páginas na Web com ela eu desenvolvi o esqueleto do projeto usandos as tags:

- html: Iniciei e finalizei o projeto web com essa tag;

- head: Inseri todas as informações básicas da página, como o título, links de elementos externos, etc; 

- title: Informei o título da página; 

- body: Consiste no corpo do nosso documento, onde se concentram todos os elementos que serão renderizados na tela do navegador;

Bootstrap: é um framework web foi utilizado para estilizar o projeto web e tornar responsivo.

GoogleChart: Como o foco era mostrar os índices de criminalidade para oferecer ao usuário uma análise de fácil compreensão, após pesquisas encontrei o GoogleChart para realizar os gráficos mensais dos índices de criminalidade;



### **IV - APRENDIZADOS EFETIVOS.**

Tivemos o primeiro contato com a Metodologia Agil: Scrum é uma metodologia utilizada para gerenciar trabalho em produtos complexos, o Scrum é composto por ciclos de atividades programadas — os sprints —, com planejamento de tarefas e datas de início e de fim determinados, ou seja, é um framework no qual pessoas podem solucionar problemas complexos e soluções adaptativas, enquanto criam de forma produtiva agregando o mais alto valor possível ao produto.
 
Canal de comunicação SLACK: Não tinha conhecimento sobre esse serviço de comunicação e por fim o Slack se tornou uma das principais ferramentas de comunição utilizadas para o desenvolvimento do Projeto Integrador, pois é um meio de comunicação ágil e instantâneo, neste canal era decidido os próximos encontros presenciais, saneamentos de dúvidas das atividades desenvolvidas, etc.
 
Conhecimento no repositório no Gitlab: Não sabia que existia ferramentas para guardar e compartilhar códigos e de formada gratuita, o nosso Master nos apresentou essa tecnologia que utilizamos até hoje. Aprendemos o principais comandos como: 

- Adicionar um diretório em específico: git add meu_diretorio
- Clonar um repositório: git clone
- Adicionar todos os arquivos/diretórios: git add .	
- Enviar arquivos para o repositório: git push
- Atualizar os arquivos da branch atual: git pull

Obtive conhecimento básico para desenvolver uma aplicação Front-end, focando nos seus elementos e estrutura, tais como:

O HTML: é uma linguagem de marcação utilizada na construção de páginas na Web.

- html: Deve iniciar e finalizar o projeto web com essa tag;

- head: inseri todas as informações básicas da página, como o título, links de elementos externos, etc; 

- title: Informa o título da página; 

- body: Consiste no corpo do nosso documento, onde ficam todos os elementos que serão renderizados na tela do navegador;

- Inserir imagens e cores no HTML;

Bootstrap: É um framework web foi utilizado para estilizar a página web.

GoogleChart: Biblioteca para geração de gráficos;

 
Ao final do projeto, percebemos que a utilização da solução poderia ser aproveitada por muitas áreas sociais:

•	Compra/Aluguel de casa;  
•	Abertura de empresas/comércios;  
•	Estudo na região;  
•	Trabalho na região;  
•	Prática esporte na região;  
•	Lazer (evento cultural, maratona geek, ou festa na região);  
•	Morador/Frequentador da região.  

Poteciais clientes pagantes:
-Empresas de segurança: com esses dados poderiam definir uma demanda de vendas/colaboradores por região;  
-Imobiliárias/Construtoras: com esses dados poderiam traçar o perfil de clientes para determinadas regiões;  
-Empreendedores: que teriam acesso a informações sobre o perfil da pessoa que frequenta a região, abrindo um restaurante ou loja que atenda a este público alvo.  

