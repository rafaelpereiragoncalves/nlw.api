# 📍 Nearby API

> **API do App Nearby** desenvolvida durante a **NLW Pocket Mobile** da [Rocketseat](https://www.rocketseat.com.br) 🚀

## 📖 Sobre o Projeto

Esta API foi criada como parte do evento **Next Level Week (NLW) Pocket Mobile**, uma semana intensiva de aprendizado promovida pela Rocketseat. O projeto consiste em uma API REST para o aplicativo **Nearby**, que permite aos usuários encontrar estabelecimentos próximos e resgatar cupons de desconto.

## 🛠️ Tecnologias Utilizadas

- **Node.js** - Ambiente de execução JavaScript
- **TypeScript** - Superset tipado do JavaScript
- **Express** - Framework web para Node.js
- **Prisma ORM** - Object-Relational Mapping para banco de dados
- **SQLite** - Banco de dados leve e eficiente
- **Zod** - Validação de esquemas TypeScript

## 🎯 Funcionalidades

- ✅ **Gerenciamento de Categorias** - CRUD de categorias de estabelecimentos
- ✅ **Gerenciamento de Estabelecimentos** - Listagem e busca de mercados/estabelecimentos
- ✅ **Sistema de Cupons** - Criação e resgate de cupons de desconto
- ✅ **Validação de Dados** - Validação robusta com Zod
- ✅ **Tratamento de Erros** - Middleware personalizado para handling de erros

## 🚀 Como Executar

### Pré-requisitos
- Node.js instalado
- npm ou yarn

### Instalação

1. **Clone o repositório**
   ```bash
   git clone [url-do-repositorio]
   cd nlw.api
   ```

2. **Instale as dependências**
   ```bash
   npm install
   ```

3. **Configure o banco de dados**
   ```bash
   npx prisma migrate dev
   ```

4. **Execute o seed do banco**
   ```bash
   npm run seed
   ```

5. **Inicie o servidor**
   ```bash
   npm start
   ```

O servidor estará rodando em `http://localhost:3333`

## 📁 Estrutura do Projeto

```
src/
├── controllers/     # Controladores das rotas
│   ├── categories-controller.ts
│   ├── coupons-controller.ts
│   └── markets-controller.ts
├── routes/          # Definição das rotas
│   ├── categories-route.ts
│   ├── coupons-route.ts
│   ├── markets-route.ts
│   └── index.ts
├── database/        # Configuração do banco
│   └── prisma.ts
├── middlewares/     # Middlewares customizados
│   └── error-handling.ts
├── utils/           # Utilitários
│   └── AppError.ts
└── server.ts        # Arquivo principal
```

## 🔗 Endpoints da API

### Categorias
- `GET /categories` - Lista todas as categorias

### Estabelecimentos
- `GET /markets` - Lista estabelecimentos próximos
- `GET /markets/:id` - Detalhes de um estabelecimento

### Cupons
- `GET /markets/:id/coupons` - Lista cupons de um estabelecimento
- `PATCH /coupons/:id` - Resgata um cupom

## 👨‍💻 Desenvolvido por

Este projeto foi desenvolvido seguindo as aulas da **Rocketseat** durante a **NLW Pocket Mobile**.

### Instrutor
- **Rodrigo Gonçalves** ([@orodrigogo](https://github.com/orodrigogo))

---

## 🚀 Sobre a Rocketseat

A [Rocketseat](https://www.rocketseat.com.br) é uma plataforma de educação em tecnologia que tem como missão levar você até os seus objetivos de forma acelerada. Especializada em Node.js, ReactJS, React Native e outras tecnologias modernas.

### 📚 Next Level Week (NLW)

O NLW é um evento online e gratuito da Rocketseat que acontece várias vezes ao ano, onde em uma semana você desenvolve uma aplicação completa, do backend ao mobile, utilizando tecnologias modernas e as melhores práticas do mercado.

---

💜 **Feito com muito aprendizado durante a NLW da Rocketseat**
