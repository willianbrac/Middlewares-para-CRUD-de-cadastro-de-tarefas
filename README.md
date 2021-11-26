## Nesta API foram desenvolvidos Middlewares para um CRUD de Users

## Tecnologias envolvidas:
  Javascript, Jest, NodeJS, Banco de dados em Memória
  
## O que fazem as funções middlewares criadas?

### function checksExistsUserAccount(request, response, next)

- Verifica se existe um usuário com o username passado no headers da request
- Caso não exista a API retornará um status 404 e a mensagem "User not found"

### function checksCreateTodosUserAvailability(request, response, next) 

- Verifica se o usuário passado no request tem mais de 10 todos cadastrados e se ele é um usuário pro
- Caso não passe será retornado um status 403 e a mensagem "upgrade to pro!"

### function checksTodoExists(request, response, next)
- Verifica o id e o username passado no header da request existe
- Se existir e guarda o user e seus todos cadastrados em memória para poderem ser utilizados posteriormente
- Caso o usuário não seja encontrado será retornado um status 404 e a mensagem "User not found!"
- Caso o id não seja válido será retornado um status 400 e a mensagem "The provided id is not a uuid!"  
- Caso o todo não exista será retornado um status 404 e a mensagem "User's todo not found!"  


### Baixe o projeto
<div>
  <p>Faça o comando 'yarn' para instalar todas as dependências</p>
  <p>Faça o comando 'yarn test' para realizar os testes com jest</p>
</div>




