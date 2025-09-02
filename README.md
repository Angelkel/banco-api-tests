# banco-api-tests

Automacao de testes para a API REST do projeto [`banco-api`](https://github.com/juliodelimas/banco-api), utilizando ferramentas modernas de testes em JavaScript.

## 🧪 Objetivo

Este projeto tem como objetivo validar o comportamento da API REST do projeto `banco-api`, realizando testes automatizados de integração para garantir a confiabilidade das funcionalidades expostas por meio de endpoints HTTP.

---

## ⚙️ Stack Utilizada

* **Linguagem**: JavaScript (Node.js)
* **Framework de Testes**: [Mocha](https://mochajs.org/)
* **Biblioteca de Asserções**: [Chai](https://www.chaijs.com/)
* **Cliente HTTP para Testes**: [Supertest](https://github.com/ladjs/supertest)
* **Relatórios de Teste**: [Mochawesome](https://github.com/adamgruber/mochawesome)
* **Carregamento de Variáveis de Ambiente**: [dotenv](https://github.com/motdotla/dotenv)

---

## 📁 Estrutura de Diretórios

```
banco-api-tests/
├── test/
│   ├── login.test.js          # Testes relacionados ao Login
│   ├── transacoes.test.js     # Testes relacionados às transações
├── mochawesome-report/        # Relatórios HTML gerados automaticamente (após execução dos testes)
├── .env                       # Arquivo de variáveis de ambiente (não versionado)
├── .gitignore
├── package.json
└── README.md
```

---

## 📄 Formato do Arquivo `.env`

Crie um arquivo `.env` na raiz do projeto com o seguinte conteúdo:

```
BASE_URL=http://localhost:3000
```

> Altere a URL conforme o endereço em que a API `banco-api` estiver rodando localmente ou remotamente.

---

## ▶️ Como Executar os Testes

### 1. Clonar o Repositório

```bash
git clone https://github.com/Angelkel/banco-api-tests.git
cd banco-api-tests
```

### 2. Instalar Dependências

```bash
npm install
```

### 3. Configurar Variáveis de Ambiente

Crie o arquivo `.env` conforme descrito acima.

### 4. Executar os Testes

```bash
npm test
```

> Os testes serão executados usando Mocha, e um relatório HTML será gerado automaticamente pelo Mochawesome.

---

## 📊 Relatório de Testes

Após a execução, um relatório completo será gerado no diretório `mochawesome-report/`. Para visualizar:

1. Navegue até a pasta `mochawesome-report/`
2. Abra o arquivo `mochawesome.html` no navegador

---

## 📚 Documentações das Dependências

* [Mocha](https://mochajs.org/)
* [Chai](https://www.chaijs.com/)
* [Supertest](https://github.com/ladjs/supertest)
* [Mochawesome](https://github.com/adamgruber/mochawesome)
* [dotenv](https://github.com/motdotla/dotenv)

---

## 📌 Observações

* Certifique-se de que a API [`banco-api`](https://github.com/juliodelimas/banco-api) esteja rodando antes de iniciar os test
