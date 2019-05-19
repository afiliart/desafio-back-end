# Desafio Back-End

Nos útlimos anos o mercado de cursos online tem crescido exponencialmente nos cenários nacional e internacional. Com grandes players no mercado, como Hotmart, Udemy, Udacity, etc.., sejam eles produtores ou distribuidores de conteúdo, vê-se cada vez mais a necessidade de organizar e categorizar os cursos.

Sendo assim, o desafio consiste na criação de uma API Rest, cujo objetivo é justamente fornecer ao consumidor final uma listagem de cursos disponíveis nas demais plataformas digitais.

## API Rest
Para isso, sua aplicação CRUD deverá apresentar as seguintes funcionalidades conforme os métodos e endpoints indicados.
Observação: Não esqueça de configurar corretamente os `status code` para cada requisição, considerando os diversos cenários possíveis.

#### Cadastrar Curso

**Request - POST : /courses**
```javascript
{
		id: String,
    	name: String,
    	category: String,
    	img: String,
    	link: String,
    	price: Number,
    	description: String
}
```

#### Editar Curso

**Request - PUT : /courses**
```javascript
{
		id: String,
    	name: String,
		*atributo a ser atualizado: valor do atributo*
}
```

#### Deletar Curso

**Request - DELETE : /courses**
```javascript
{
		id: String,
    	name: String
}
```

#### Listar Cursos

**Request - GET : /courses**
A listagem dos cursos deve ser apresentada com paginação de 15 cursos/página.

## Requisitos
Sua API deve ser desenvolvida seguindo os seguintes requisitos:
- Linguagem: `NodeJS`.
- Banco de dados: `MongoDB`.
- Hospedagem: qualquer hospedagem de sua preferência (dica: existem serviços que disponibilizam planos gratuitos).
- A partir do momento que for feito o `FORK` desse repositório, o prazo de entrega do desafio é de 5 dias. O código deverá ser postado em seu GitHub e deverá conter um arquivo `readme.md`  com as especificações do seu projeto.

## Diferenciais
- Interface Web para manipulação dos dados.
- Sistema de autenticação de usuários para criar, editar e deletar cursos.
