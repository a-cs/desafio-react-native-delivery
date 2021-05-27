![Gostask](https://camo.githubusercontent.com/d25397e9df01fe7882dcc1cbc96bdf052ffd7d0c/68747470733a2f2f73746f726167652e676f6f676c65617069732e636f6d2f676f6c64656e2d77696e642f626f6f7463616d702d676f737461636b2f6865616465722d6465736166696f732e706e67)
Desafio react-native-delivery do Bootcamp [GoStack da Rocketseat](https://rocketseat.com.br/gostack)

# Sobre o desafio

O objetivo do desafio é desenvolver mais uma aplicação, a GoRestaurant, só que dessa vez a versão mobile para o cliente. Praticando o que foi aprendido até agora no React Native junto com TypeScript.

Essa será uma aplicação que irá se conectar a uma Fake API, e exibir e filtrar os pratos de comida da API e permitir a criação de novos pedidos.

# Instalando as dependências
Para instalar as dependências, execute o seguinte comando:

  `yarn`

# Utilizando uma fake API

Para que você tenha os dados para exibir em tela, execute o seguinte comando:

  `yarn json-server server.json -p 3333`

com isso você terá acesso as seguintes rotas.
Rota `/foods`: Retorna todas as comidas cadastradas na API

Rota `/foods/:id`: Retorna um prato de comida cadastradas na API baseado no id

Rota `/categories`: Retorna todas as categorias cadastradas na API

Rota `/orders`: Retorna todas os pedidos que foram cadastrados na API

Rota `/favorites`: Retorna todas as comidas favoritas que foram cadastrados na API


# Funcionalidades da aplicação

- [x] **`Listar os pratos de comida da sua API`**: A página `Dashboard` é capaz de exibir uma listagem, com o campo `name`, `value` e `description` de todos os pratos de comida que estão cadastrados na API.
- [x] **`Listar as categorias da sua API`**:  A página `Dashboard` deve ser capaz de exibir uma listagem, com o campo `title` e `image_url` de todas as categorias que estão cadastrados na API.
- [x] **`Filtrar pratos de comida por busca ou por categorias`**: A página `Dashboard` permite que o input de pesquisa e os botões de categoria façam uma busca na API de acordo com o que estiver selecionado ou escrito no input.
- [x] **`Listar os pedidos da sua API`**: A página `Orders` é capaz de exibir uma listagem, com o campo as informações do produto pedido, com `name` e `description` de todos os pedidos que estão cadastrados na API.
- [x] **`Listar os pratos favoritos da sua API`**: A página `Favorites` deve ser capaz de exibir uma listagem, com o campo as informações do produto favorito, com `name` e `description` de todos os pedidos que estão cadastrados na API.
- [x] **`Realizar um pedido`**: Na página `Dashboard`, ao clicar em um item, você deve redirecionar o usuário para a página `FoodDetails`, onde será possível realizar um novo pedido, podendo controlar a quantidade desse item pedido, ou adicionar ingredientes extras. Todo o valor é  calculado de acordo com a quantidade pedida.

# Específicação dos testes

- [x] **`should be able to list the food plates`**: Para que esse teste passe, sua aplicação deve permitir que sejam listados na sua `Dashboard`, todos os pratos de comidas que são retornados da sua fake API.
- [x] **`should be able to list the food plates filtered by category`**: Para que esse teste passe, sua aplicação deve permitir que sejam listados na sua `Dashboard`, os pratos de comidas filtrados por categoria da sua fake API.
- [x] **`should be able to list the food plates filtered by name search`**: Para que esse teste passe, sua aplicação deve permitir que sejam listados na sua `Dashboard`, os pratos de comidas filtrados por nome da sua fake API.
- [x] **`should be able to navigate to the food details page`**: Para que esse teste passe, em sua `Dashboard`, você deve permitir que ao clicar em um item, seja navegado para a página `FoodDetails` passando por parâmetro da navegação o id do item clicado.
- [x] **`should be able to list the favorite food plates`**: Para que esse teste passe, sua aplicação deve permitir que sejam listados na sua página `Favorites`, todos os pratos de comidas que estão salvos na rota `favorites`.
- [x] **`should be able to list the orders`**: Para que esse teste passe, sua aplicação deve permitir que sejam listados na sua página `Orders`, todos os pratos de comidas que estão salvos na rota `orders`.
- [x] **`should be able to list the food`**: Para que esse teste passe, sua aplicação deve permitir que seja listado todos os dados de uma comída específica na página `FoodDetails`, baseado no id recuperado pelos parametros da rota.
- [x] **`should be able to increment food quantity`**: Para que esse teste passe, você deve permitir que seja incrementada em 1 a quantidade do item na página `FoodDetails`.
- [x] **`should be able to decrement food quantity`**: Para que esse teste passe, você deve permitir que seja decrementada em 1 a quantidade do item na página `FoodDetails`.
- [x] **`should not be able to decrement food quantity below than 1`**: Para que esse teste passe, você deve impedir que seja decrementado a quantidade de itens até um número menor que 1, assim o número mínimo de itens no pedido é 1.
- [x] **`should be able to increment an extra item quantity`**: Para que esse teste passe, você deve permitir que seja incrementada em 1 a quantidade de um ingrediente extra na página `FoodDetails` baseado no seu id.
- [x] **`should be able to decrement an extra item quantity`**: Para que esse teste passe, você deve permitir que seja decrementado em 1 a quantidade de um ingrediente extra na página `FoodDetails` baseado no seu id.
