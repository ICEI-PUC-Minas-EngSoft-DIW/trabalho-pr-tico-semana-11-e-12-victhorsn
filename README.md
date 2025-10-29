# Trabalho Prático 06 - Semanas 11 e 12

Nessa etapa, você irá evoluir o projeto anterior e montando um ambiente de desenvolvimento mais completo, típico de projetos profissionais. Nesse processo, vamos utilizar um **servidor backend simulado** com o JSON Server que fornece uma APIs RESTful a partir de um arquivo JSON.

Para esse projeto, além de mudarmos o JSON para o JSON Server, vamos permitir o cadastro e alteração de dados da entidade principal (CRUD).

## Informações do trabalho

- Nome: Victhor Guilherme Santos Loiola
- Matricula: 903255
- Proposta de projeto escolhida: CRUD com JSON Server (Filmes)
- Breve descrição sobre seu projeto: O projeto tem como objetivo desenvolver uma aplicação web que realiza o gerenciamento de filmes, permitindo o cadastro, listagem, edição e exclusão de informações utilizando o JSON Server como backend simulado.
A interface foi construída com HTML, CSS e JavaScript, aplicando o conceito de consumo dinâmico de dados via fetch(), simulando o funcionamento de um sistema real com API REST.
Além disso, o projeto apresenta uma interface moderna e intuitiva, permitindo visualizar as capas dos filmes, seus títulos, descrições e demais detalhes de forma prática e interativa.

**Print dos testes da API com Postman ou similar**

![GET](https://github.com/user-attachments/assets/728dabe3-6527-4d3a-a29a-f42cdd01b600)

![POST](https://github.com/user-attachments/assets/38aa1e99-9c09-42bf-939c-6c23daeb5083)

![PUT](https://github.com/user-attachments/assets/3482d8f3-988a-4cd0-984a-02a8b18de304)

![DELETE](https://github.com/user-attachments/assets/dbdfa267-879f-4bb1-a04b-5f4b0df4dedb)

**Print da aba NETWORK com requisições Fetch/XHR POST e GET**

![Print NETWORK GET](https://github.com/user-attachments/assets/e8e6fa6d-4eb3-4c09-87b6-e18504c81cdb)

![1](https://github.com/user-attachments/assets/8a47aa2d-2488-48ff-ab76-23683b0bc3d3)

![MÉTODO POST](https://github.com/user-attachments/assets/f31bf5a3-b42b-4bd8-b4dd-9b7fa89a4323)

## **Orientações Gerais**

Nesse projeto você vai encontrar a seguinte estrutura base:

* **Pasta db**
  Essa pasta contem um único arquivo: `db.json`. Esse arquivo serve de banco de dados simulado e nele você deve colocar as estruturas de dados que o seu projeto manipula.
  * **OBS**: Já incluímos a estrutura de usuários como exemplo e para que você possa utlizar no seu projeto. Se precisar, faça os ajustes necessários para seu projeto.
* **Pasta public**
  Nesta pasta você deve colocar todos os arquivos do seu site (front end). Aqui vão os arquivos HTML, CSS, JavaScript, imagens, vídeos e tudo o mais que precisar para a interface do usuário.
* **Arquivo README.md**
  Este arquivo em que são colocadas as informações de quem está desenvolvendo esse projeto e os registros solicitados no enunciado da tarefa.
* **Arquivo .gitignore**
  Configuração do que deve ser ignorado pelo git evitando que seja enviado para o servidor no GitHub.
* **Arquivo package.json**
  Considerado o manifesto do projeto ou arquivo de configuração. Nesle são incluídas as informações básicas sobre o projeto (descrição, versão, palavras-chave, licença, copyright), a lista de pacotes dos quais o projeto depende tanto para desenvolvimento quanto execução, uma lista de  do projeto, scripts entre outras opções.
  * **OBS**: Esse arquivo é criado assim que o projeto é iniciado por meio do comando `npm init`.
  * **OBS2**: Esse arquivo já traz a informação de necessidade do JSONServer.
* **Pasta node_modules**
  Local onde ficam os pacotes dos quais o projeto depende. Evite enviar essa pasta para o repositório remoto. Essa pasta é reconstruída toda vez que se executa o comando `npm install`.

**Ambiente de Desenvolvimento (IMPORTANTE)**

> A partir de agora, **NÃO utilizamos mais o LiveServer/FiveServer** durante o processo de desenvolvimento. O próprio JSONServer faz o papel de servidor.

Para iniciar o JSONServer e acessar os arquivos do seu site, siga os seguintes passos:

1. Abra a pasta do projeto dentro da sua IDE (por exemplo, Visual Studio Code)
2. Abra uma janela de teminal e certifique-se que a pasta do terminal é a pasta do projeto
3. Execute o comando `npm install`
   Isso vai reconstruir a pasta node_modules e instalar todos os pacotes necessários para o nosso ambiente de desenvolvimento (Ex: JSONServer).
4. Execute o comando `npm start`
   Isso vai executar o JSONServer e permitir que você consiga acessar o seu site no navegador.
5. Para testar o projeto:
   1. **Site Front End**: abra um navegador e acesse o seu site pela seguinte URL: 
      [http://localhost:3000]()
   2. **Site Back End**: abra o navegador e acesse as informações da estrutura de usuários por meio da API REST do JSONServer a partir da seguinte URL: 
      [http://localhost:3000/usuarios](http://localhost:3000/usuarios)

Ao criar suas estruturas de dados no arquivo db.json, você poderá obter estes dados através do endereço: http://localhost:3000/SUA_ESTRUTURA, tal qual como foi feito com a estrutura de usuários. **IMPORTANTE**: Ao editar o arquivo db.json, é necessário parar e reiniciar o JSONServer.

**IMPORTANTE:** Assim como informado anteriormente, capriche na etapa pois você vai precisar dessa parte para as próximas semanas. 

**IMPORTANTE:** Você deve trabalhar:

* na pasta **`public`,** para os arquivos de front end, mantendo os arquivos **`index.html`**, **`detalhes.html`**, **`styles.css`** e **`app.js`** com estes nomes, e
* na pasta **`db`**, com o arquivo `db.json`.

Deixe todos os demais arquivos e pastas desse repositório inalterados. **PRESTE MUITA ATENÇÃO NISSO.**
