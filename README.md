## LISTA COM O LINK DOS PORTFÓLIOS DOS APIs:
[API 1° SEMESTRE - **DANZO - Mapa de Criminalidade ao Redor da FATEC**](https://github.com/ZVIEWIL/portifolio1) 

[API 2° SEMESTRE - **GANTT CHART**](https://github.com/ZVIEWIL/portifolio2)

[API 3° SEMESTRE - **CADASTRO POSITIVO**](https://github.com/ZVIEWIL/portifolio3)

# API do 1° SEMESTRE - ***DANZO - Mapa de Criminalidade ao Redor da FATEC***

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
Python é uma linguagem de programação de alto nível, interpretada de script, imperativa, orientada a objetos, funcional, de tipagem dinâmica e forte.
Para o desenvolvimento do Projeto Integrador (Web Bot), foi escolhida a linguagem Python pelos integrantes do grupo por estarem familiarizados e por recomendação dos professores. Foi utilizada para desenvolver as raspagens do bot, integração com o front end e conexão com o banco de dados.

Bibliotecas utilizadas:

- Flask: É um micro framework que utiliza a linguagem Python para criar aplicativos Web. Escolhemos utiliza-lo por causa de suas principais características que são: simplicidade, rapidez no desenvolvimento.

- Selenium: Utilizado para acessar e realizar comandos no site da SSP/SP, de forma que fosse possível baixar o arquivo .CSV utilizado para alimentar o nosso banco de dados.

- SQlite: O SQLite é uma base de dados relacional de código aberto e que dispensa o uso de um servidor na sua atuação. Utilizamos para armazenar os dados extraídos do arquivo .csv obtido no site da SSP/SP.

- Pandas: É uma ferramenta de manipulação e análise de dados de código aberto rápida, poderosa, flexível e fácil de usar. Foi Utilizado para manipular os dados recebidos, agrupando-os por localização e tratando os dados para apresentação no mapa de calor.

- Folium: Biblioteca do Python utilizada para facilitar a visualização de dados de vetores/geolocalização em mapas. Utilizamos para gerar o Mapa de Calor através dos dados fornecidos pelo Banco de Dados.

- Flask_googlecharts: É utilizado para gerar gráficos. foi utilizado para gerar gráficos para realizarmos comparações mensais sobre o índice de criminalidade na região.

### **CONTRIBUIÇÕES INDIVIDUAIS**
Com as divisões das tarefas feitas pela equipe, fiquei responsável por tratar os dados vindos do arquivo .CSV e inseri-los no BD. Como um colega da equipe acabou desistindo do curso, acabei acumulando a tarefa de realizar a raspagem dos dados no site da SSP/SP. Pra mim foi bastante desafiador realizar as 2 tarefas, pois nunca havia tido contato algum com desenvolvimento de softwares.

Acabei contribuindo com as seguintes tarefas realizadas:
- Desenvolvimento do método que utilizamos para realizar a raspagem de dados no site da SSP/SP com o Selenium;
![Screenshot_6](https://user-images.githubusercontent.com/54503903/142793872-cd76070f-5cc5-480b-963b-ce8089fd8147.png)

- Desenvolvimento do método utilizado para criar os diretórios para armazenar o arquivo .csv extraído;
![Screenshot_7](https://user-images.githubusercontent.com/54503903/142794097-674f558a-0b78-4859-9dab-460d1243cb01.png)

- Desenvolvimento do método que utilizamos para inserir no banco de dados os dados extraídos do arquivo .csv;
![Screenshot_8](https://user-images.githubusercontent.com/54503903/142794239-c305b532-517a-4480-a3df-fb8fd2fc1bd7.png)

- Desenvolvimento do método que utilizamos para gerar o mapa de calor;
![Screenshot_9](https://user-images.githubusercontent.com/54503903/142794324-56c6067c-17ef-4b1f-bbc9-b69eae8bd256.png)

### **APRENDIZADOS EFETIVOS**
- Metodologia SCRUM: Aprendi como funciona e utilizamos no projeto a metodologia. As entregas foram realizadas por Sprints, realizamos Daily Scrum e Kanban Scrum(To do, Doing e Done) para monitorarmos o andamento do projeto.

- Slack: Conheci o Slack e utilizamos como meio de comunicação. Ferramenta bastante utilizada no nosso meio, foi importante descobri-la, utilizamos para documentar nossas conversas/reuniões sobre o projeto.

- Git: Conhecei o  Git/GitLab, que utilizamos para armazenar os códigos e documentações do projeto. Aprendi a criar repositório local, clonar repositórios remotos, criar branchs locais/remotas, realizar commits e merges.

- Python: Foi o meu primeiro contato com uma linguagem de programação, aprendi a instalar, conceitos básicos, tipos de variáveis, como importar e utilizar bibliotecas.

- IDE's: Aprendi a configurar o ambiente para programar, utilizei o Pycharm como IDE.
