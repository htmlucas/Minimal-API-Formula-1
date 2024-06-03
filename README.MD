# Minimal API Formula 1

### Descrição
Um app curto utilizando **[FastiFy](https://www.npmjs.com/package/fastify)**

### Features
- Listar os equipes participantes. (exemplo: Ferrari, entre outros...)
- Listar os motoristas participantes. (exemplo: Max Verpstappen, entre outros...)
- Filtrar motorista por id.

### Listar as equipes

- **Endpoint:** `GET /teams`
- **Descrição:** Retorna uma lista de equipes.
- **Exemplo de resposta:**

```json
    {
    "teams": [
      {
        "id": 1,
        "name": "Ferrari",
        "base": "Maranello,Emillia-Romagna, Italy"
      },
      {
        "id": 2,
        "name": "McLaren",
        "base": "Woking, United Kingdom"
      },
      {
        "id": 3,
        "name": "Mercedes",
        "base": "Brackley, United Kingdom"
      },
      {
        "id": 4,
        "name": "Red Bull Racing",
        "base": "Milton Keynes, United Kingdom"
      }
    ]
  }
```

### Listar os motoristas

- **Endpoint:** `GET /drivers`
- **Descrição:** Retorna uma lista de motoristas.
- **Exemplo de resposta:**

```json
    {
    "drivers": [
      {
        "id": 1,
        "name": "Max Verpstappen",
        "team": "Red Bull Racing"
      },
      {
        "id": 2,
        "name": "Lewis Hamilton",
        "team": "Ferrari"
      },
      {
        "id": 3,
        "name": "Leandro Norris",
        "team": "Mc Laren"
      }
    ]
  }
```

### Filtrar motorista por id

- **Endpoint:** `GET /drivers/{id}`
- **Descrição:** Retorna um motorista especificado pelo id.
- **Exemplo de resposta:**

```json
    {
    "id": 1,
    "name": "Max Verpstappen",
    "team": "Red Bull Racing"
    }
```


### Tecnologias Utilizadas

- **[Node.js](https://nodejs.org/):** Plataforma de desenvolvimento para construir a API.
- **[TypeScript](https://www.typescriptlang.org/):** Linguagem de programação que adiciona tipagem estática ao JavaScript, aumentando a segurança e a qualidade do código.
- **[Tsup](https://github.com/egoist/tsup):** Ferramenta para construir pacotes TypeScript, usada para criar a versão de distribuição do projeto.
- **[Tsx](https://www.npmjs.com/package/tsx):** Ferramenta de execução de TypeScript, utilizada para iniciar o servidor em modo de desenvolvimento e em modo de observação (watch mode).
- **[@types/node](https://www.npmjs.com/package/@types/node):** Tipagens para Node.js, proporcionando suporte ao desenvolvimento em TypeScript com autocompletar e verificação de tipos para APIs Node.js.

### Como Rodar o Projeto
1. Clone o repositório
2. Instale as dependências com `npm install`
3. Execute o servidor em modo de desenvolvimento com `npm run start:dev`
4. Execute o servidor em modo de observação com `npm run start:watch`
5. Crie a versão de distribuição com `npm run dist`
6. Execute a versão de distribuição com `npm run start:dist`

### Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

### Licença
Este projeto está licenciado sob a ISC License.