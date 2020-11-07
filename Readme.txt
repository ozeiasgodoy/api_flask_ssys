Criar usuario:
curl -H "Content-Type: application/json" localhost:8000/signup

Response

{
	"username": "username",
	"password": "password"
}

Gerar Token: 

curl -H "Content-Type: application/json" localhost:8000/auth
Json
{
	"username": "username",
	"password": "password"
}

Response

{
  "access_token": "token_gerado"
}

Utilizando o token:

Adicionar ao Header da requisição
Authorization: jwt token_gerado