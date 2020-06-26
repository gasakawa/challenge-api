## Desafio

> ##### <u>Utilize este repositório como template, para "clonar" o mesmo na sua conta de github.</u>



Foi requisitado criar uma API capaz de definir os aprovados no INTENSIVAO 2019. Assim, foi aberto o processo de desenvolvimento, em que as atividades da sprint foram definidas:

#### Cadastrar candidatos

Na rota `/candidatos`  adicione o candidato na lista de candidatos. O objeto enviado deve ter o formato abaixo:

```json
{
	'nome': 'Gabriel Asakawa',
	'cidade': 'São Paulo'
}
```

**PS.** Utilize `uuid` como identificador do candidato.



#### Cadastrar as notas dos candidatos

Na rota `/candidatos/notas` registre as notas do candidato. O objeto enviado de ter o formato abaixo: 

```json
{
	'nome': 'Gabriel Asakawa',
	'cidade': 'São Paulo',
	'notas': [10, 8, 9]
}
```



#### Inserir número de vagas

Na rota `/vagas` registre a quantidade de vagas para cada disciplina.



#### Exibir candidatos aprovados

Na rota `/candidatos/aprovados` retorne todos os candidatos aprovados. O retorno deve ter o formato abaixo:

```json
[
    {
        'nome': 'Gabriel Asakawa',
        'cidade': 'São Paulo',
        'aprovado': true
    },
    {
        'nome': 'Batman',
        'cidade': 'Guarulhos',
        'aprovado': true
    }
]
```



#### Exibir porcentagem de aprovados por cidade

Na rota `/aprovados/cidade` retorne a porcentagem dos candidatos que foram aprovados por cidade. O retorno deve ter o formato abaixo:

```json
[
	{
		'cidade': 'São Paulo',
		'porcentagem': 0.80
	},
	{
		'cidade': 'Guarulhos',
		'porcentagem': 0.78
	}
]
```



### Ferramentas / Tecnologias

Para este exercicio, recomendo utilizar as seguintes ferramentas ou tecnologias

1. [Node.js](https://nodejs.org/en/) 
2. [Express](https://expressjs.com/pt-br/)
3. [Yarn](https://yarnpkg.com/)
4. [Insomnia](https://insomnia.rest/download/core/?&ref=https%3A%2F%2Fwww.google.com%2F) (para testar a API)
5. [Devdocs](https://devdocs.io/) (documentação de quase todas as ferramentas / tecnologias)