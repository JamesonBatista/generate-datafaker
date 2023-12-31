# generate-datafaker

`generate-datafaker` é uma biblioteca JavaScript projetada para facilitar a geração de dados fictícios para uso em testes de aplicações web ou APIs. Com uma ampla gama de funções, esta biblioteca pode criar dados realistas como nomes, endereços, números de telefone e muito mais.

## Instalação

Para adicionar `generate-datafaker` ao seu projeto, execute o seguinte comando:

```bash
npm install generate-datafaker
```

## Uso

```js
const faker = require("generate-datafaker");
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
`generateFakePolicyNumber():` Retorna um número ficticio de apolice de seguros <br>
`generateCompleteCar():` Retorna dados completo de um carro <br>

## Modo de uso

```js
const faker = require("generate-datafaker");

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
let age = faker.generateAge(18, 70); // Ex: 30   min 18, max 70
let rne = faker.generateRNE(); // Ex: V123456-7
let plate = faker.generatePlate(); // Ex: ABC-1234
let uuidv4 = faker.generateUuidv4(); // Ex: 123e4567-e89b-12d3-a456-426614174000
let loremIpsum = faker.generateLoremIpsum(19); // Ex: Lorem ipsum dolor sit amet... 10 palavras
let date = faker.generateDate(); // Ex: 01/01/2020
let apolice = faker.generateFakePolicyNumber(10); // quantidade de caracters
let password = faker.generatePassword();
let car = generateCompleteCar();
```

### generateDate()

pode ser receber parametros que modificam das datas

- generateDate(1, 2, 1) // um dia a mais, dois meses a mais, um ano a mais da data atual
- generateDate(-1, -2, -4) // menos um dia anterior, menos 2 meses, menos 4 anos

```json
{
  "iso": "2023-11-09T10:22:11.564Z",
  "utc": "Thu, 09 Nov 2023 10:22:11 GMT",
  "stringFormat": "Thu Nov 09 2023 07:22:11 GMT-0300 (Horário Padrão de Brasília)",
  "localDate": "09/11/2023",
  "localTime": "07:22:11",
  "localDateTime": "09/11/2023 07:22:11",
  "timestamp": 1699525331564,
  "customFormat": "2023-11-09 07:22:11",
  "br": {
    "date": "09/11/2023",
    "time": "07:22:11",
    "dateTime": "09/11/2023 07:22:11",
    "timeStamp": 1699525331564,
    "iso": "2023-11-09T10:22:11.564Z",
    "stringFormat": "Thu Nov 09 2023 07:22:11 GMT-0300 (Horário Padrão de Brasília)"
  }
}
```
