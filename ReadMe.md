# generate-data-faker

`generate-datafaker` é uma biblioteca JavaScript projetada para facilitar a geração de dados fictícios para uso em testes de aplicações web ou APIs. Com uma ampla gama de funções, esta biblioteca pode criar dados realistas como nomes, endereços, números de telefone e muito mais.

## Instalação

Para adicionar `generate-datafaker` ao seu projeto, execute o seguinte comando:

```bash
npm install generate-datafaker
```

## Uso

```js
const faker = require("generate-data-faker");

let neighborhood = faker.generateNeighborhood();
let cep = faker.generateCEP();
let cnpj = faker.generateCNPJ();
```

## Funcionalidades

    O generate-datafaker oferece as seguintes funções:

`generateNeighborhood():` Retorna um bairro fictício aleatório.<br>
`generateCEP():` Gera um CEP fictício válido.<br>
`generateCNPJ():` Gera um CNPJ fictício válido.<br>
`generateCity():` Retorna uma cidade fictícia aleatória.<br>
`generateStreet():` Retorna um nome de rua fictício aleatório.<br>
`generateState():` Retorna um estado fictício aleatório.<br>
`generateCPF():` Gera um CPF fictício válido.<br>
`generateEmail():` Gera um endereço de e-mail fictício aleatório.<br>
`generatePhone():` Gera um número de telefone fictício válido.<br>
`generateRG():` Retorna um número de RG fictício válido<br>
`generateEnterprise():` Retorna dados de uma empresa fictícia<br>
`generateCNH():` Retorna número de CNH válido fictícia <br>
`generateName():` Retorna um nome fictício <br>
`generatePISPASEP():` Retorna um número fictício de PIS/PASEP <br>
`generateCreditCard():` Retorna dados como numero, data, e code de um cartão de crédito <br>
`generateAge():` Retorna um número min 18 max de 60, para alterar basta passar novos numeros<br>
`generateRNE():` Retorna um número de RNE registro de estrangeiros <br>
`generatePlate():` Retorna um objeto com duas placas de veículos incluindo novo modelo<br>
`generateUuidv4():` Retorna uuid v4<br>
`generateLoremIpsum():` Retorna um texto dependendo do tamanho requerido<br>
`generateDate():`Retorna um objeto de datas e vários formatos<br>
`generatePassword():` Retorna um password incluindo letras numeros e caracters<br>

## Modo de uso

```js
const faker = require("generate-data-faker");

let bairro = faker.generateNeighborhood(); // Santo Amaro

let cep = faker.generateCEP(); // 77015570

let cnpj = faker.generateCNPJ(); // 83833453000126

let city = faker.generateCity(); // Curitiba

let street = faker.generateStreet(); // Margem Esquerda do Rio Negro

let state = faker.generateState(); // MG

let cpf = faker.generateCPF(); // 37745776090

let email = faker.generateEmail(); // Ex: joaocarlos@example.com

let phone = faker.generatePhone(); // Ex: (11) 99999-9999
let rg = faker.generateRG(); // Ex: 40.000.000-X
let enterprise = faker.generateEnterprise(); // Ex: Empresa X Ltda
let cnh = faker.generateCNH(); // Ex: 12345678901
let name = faker.generateName(); // Ex: João Carlos
let pispasep = faker.generatePISPASEP(); // Ex: 120.12345.12-3
let creditCard = faker.generateCreditCard(); // Ex: 1234 5678 9123 4567
let age = faker.generateAge(); // Ex: 30
let rne = faker.generateRNE(); // Ex: V123456-7
let plate = faker.generatePlate(); // Ex: ABC-1234
let uuidv4 = faker.generateUuidv4(); // Ex: 123e4567-e89b-12d3-a456-426614174000
let loremIpsum = faker.generateLoremIpsum(); // Ex: Lorem ipsum dolor sit amet...
let date = faker.generateDate(); // Ex: 01/01/2020

let password = faker.generatePassword();
```

### generateDate()

pode ser receber parametros que modificam das datas

- generateDate(1, 2, 1) // um dia a mais, dois meses a mais, um ano a mais da data atual
- generateDate(-1, -2, -4) // menos um dia anterior, menos 2 meses, menos 4 anos

```json
{
  "iso": "2019-09-06T18:10:49.579Z",
  "utc": "Fri, 06 Sep 2019 18:10:49 GMT",
  "stringFormat": "Fri Sep 06 2019 15:10:49 GMT-0300 (Horário Padrão de Brasília)",
  "localDate": "06/09/2019",
  "localTime": "15:10:49",
  "localDateTime": "06/09/2019 15:10:49",
  "timestamp": 1567793449579,
  "customFormat": "2019-09-06 15:10:49",
  "br": {
    "date": "06/09/2019",
    "time": "15:10:49",
    "dateTime": "06/09/2019 15:10:49",
    "timeStamp": 1567793449579,
    "iso": "2019-09-06T18:10:49.579Z",
    "stringFormat": "Fri Sep 06 2019 15:10:49 GMT-0300 (Horário Padrão de Brasília)"
  }
}
```
