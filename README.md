<h1 align="center">
    Desafio Conceitos do Node.js
</h1>

## :rocket: Tecnologias

-  [JavaScript](https://www.w3schools.com/js/)
-  [Node.js](https://nodejs.org/en/)

## :boom: Como Executar

- ### **Pré-requisitos**

  - É **necessário** possuir o **[Node.js](https://nodejs.org/en/)** instalado.
  - É **necessário** possuir o **[Git](https://git-scm.com/)** instalado e configurado.
  - É **necessário** ter um gerenciador de pacotes seja o **[NPM](https://www.npmjs.com/)** ou **[Yarn](https://yarnpkg.com/)**.
  - É **necessário** ter um client de requisições REST como o **[Insomnia](https://insomnia.rest/)** ou **[Postman](https://www.postman.com/)**.

1. Faça um clone do repositório:

```sh
  $ git clone https://github.com/ianbmesquita/desafio-conceitos-nodejs.git
```

2. Executando a Aplicação:

```sh
  # Acessando o diretório da API.
  $ cd desafio-conceitos-nodejs

  # Instalando as dependências do projeto.
  $ yarn # ou npm install

  # Inicializando o servidor node.
  $ yarn dev	
```

3. Com um client de requisições REST como o Insomnia ou o Postman, acessar as rotas disponibilizadas na API.

 - Cadastrar um novo repositório.
   **POST** http://localhost:3333/repositories

Request Body (Exemplo):
```
   {
	"title": "Repositório",
	"url": "https://www.desafio.com",
	"techs": [
		"NodeJs",
		"ReactJs",
		"TypeScript"
	]
   }
```

 - Listar todos os repositórios.
   **GET** http://localhost:3333/repositories

 - Alterar os atributos de um repositório específico.
   **PUT** http://localhost:3333/repositories/:id

Request Body (Exemplo):
```
   {
	"title": "Repositório alterado",
	"url": "https://www.desafio.com",
	"techs": [
		"NodeJs",
		"JavaScript"
	]
   }
```

 - Excluir um repositório específico.
   **DELETE** http://localhost:3333/repositories/:id

 - Atribuir likes para um repositório específico.
   **POST** http://localhost:3333/repositories/:id/like


## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.

---
<sup>Projeto desenvolvido com a tutoria de [Diego Fernandes](https://github.com/diego3g), da [Rocketseat](rocketseat.com.br).</sup>
