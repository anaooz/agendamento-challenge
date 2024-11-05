## Como criar a pipeline:

1. No seu projeto do Azure DevOps, vá até Pipelines e selecione New Pipeline.
2. Clique em Use the classic editor na parte inferior da tela.
3. Escolha o repositório onde seu código está hospedado e clique em Continue.
4. No campo de templates, selecione Maven.
5. Faça as configurações necessárias para a aplicação (como versão do JDK, sistema opercaional, pasta do .jar etc.)
6. Clique em Save & Queue.
7. Acompanhe o progresso para verificar se a aplicação compila, executa testes e faz deploy corretamente no Azure.

## JSONs:

`GET` /usuario

`POST` /usuario

```js
{
  "nome": "Roger Waters",
  "cpf": {
    "cpf": "23324234126"
    },
  "email": "lanadelrey@email.com",
  "senha": "210685",
  "dataDeNascimento": "1985-06-21",
  "endereco": {
    "cep": 67890453,
    "logradouro": "Rua das Lamentações",
    "numero": 505,
    "bairro": "Hollywood",
    "complemento": "Sem Complemento"
    }
}
```

`PUT` /usuario/{id}

```js
{
  "nome": "Bernie Taupin",
  "cpf": {
    "cpf": "23324234126"
  },
  "email": "bernietaupin@gmail.com",
  "senha": "210685",
  "dataDeNascimento": "1950-05-22",
  "endereco": {
    "cep": 67890453,
    "logradouro": "Rua das Estrelas",
    "numero": 1000,
    "bairro": "Hollywood",
    "complemento": "Sem Complemento"
  }
}
```

`DELETE` /usuario/{id}

---

`GET` /hospital

`POST` /hospital

```js
{
    "nomeFantasia": "Hospital ABC",
    "razaoSocial": "João da Silva",
    "dataDaAbertura": "2023-10-11",
    "endereco": {
        "logradouro": "Rua Hospitalar",
        "numero": 123,
        "bairro": "Bairro Saúde",
        "complemento": "Sem Complemento",
        "cep": 12345678
    },
    "ativo": true,
    "cnpj": {
        "cnpj": "1234567890123"
    }
}

```

`PUT` /hospital/{id}

```js
{
    "nomeFantasia": "Hospital ABC123",
    "razaoSocial": "João da Silva",
    "dataDaAbertura": "2023-10-11",
    "endereco": {
        "logradouro": "Rua Hospitalar",
        "numero": 123,
        "bairro": "Bairro Saúde",
        "complemento": "Perto da Praça",
        "cep": 12345678
    },
    "ativo": true,
    "cnpj": {
        "cnpj": "1234567890123"
    }
}

```

`DELETE` /hospital/{id}

---

`GET` /medico

`POST` /medico

```js
{
    "nome": "Renato Ruiz",
    "especialidade": "Cardiologista",
    "endereco": {
        "logradouro": "Rua Médica",
        "numero": 1245,
        "bairro": "Bairro Saúde",
        "complemento": "Complemento Médico",
        "cep": 87654321
    },
    "ativo": false,
    "hospitais": [],
    "cmr": "cmr123456",
    "cpf": {
        "cpf": "12345678901"
    },
    "agendamento": null,
    "cnpj": {
        "cnpj": "12345678901234"
    }
}
```

`PUT` /medico/{id}

```js
{
    "nome": "Renato Ruiz de Almeida",
    "especialidade": "Cardiologista",
    "endereco": {
        "logradouro": "Rua Médica",
        "numero": 1245,
        "bairro": "Bairro Saúde",
        "complemento": "Complemento Médico",
        "cep": 87654321
    },
    "ativo": true,
    "cmr": "cmr123456",
    "cpf": {
        "cpf": "12345678901"
    },
    "cnpj": {
        "cnpj": "12345678901234"
    }
}
```

`DELETE` /medico/{id}
