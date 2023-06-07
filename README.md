

**Como Registrar**
**POST** http://localhost:8080/register
{
	"name": "Fernando Piana Pereira",
	"email": "Fernando@gmail.com",
	"password": "Peido"
}

**Exemplo de login:** 
**POST** http://localhost:8080/login
{
	"email": "FernandoPiana@gmail.com",
	"password": "Peidofedorento"
}

**Cadastrando uma receita:**
*O tempo de preparo (preparationTime) em minutos!*

**POST** http://localhost:8080/recipes
{
	"name": "Cheesecake",
	"description": "torta doce de queijo cremoso e calda de frutas vermelhas",
	"preparationTime": 290
}

**Deletando usuário:**
*Ao deletar um usuários, todas as suas receitas publicadas também serão deletadas!*

*id = id do usuário no banco, também é informado ao se registrar*
**DELETE** http://localhost:8080/user/id

**Deletando receita:**
*id = id da receita no banco, também é informado ao publicar uma receita*
**DELETE** http://localhost:8080/recipes/id