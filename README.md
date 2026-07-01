# Front-end API Licitacao

Este é o front-end do projeto desenvolvido como parte do teste técnico para a Effecti. A aplicação foi construída com **Vue.js 3** e consome dados de uma API construída com **Spring Boot**.

## 🧾 Funcionalidades

- Lista de licitações públicas extraídas do site do ComprasNet.
- Filtros por código UASG e número de pregão.
- Integração com a API `Spring Boot` hospedada localmente.
- Interface simples e responsiva para visualização dos dados.

## 🛠 Tecnologias utilizadas
- Vue.js 3
- Vite
- Axios
- CSS

---

## 🚀 Como rodar o projeto localmente

### Pré-requisitos

- Node.js (versão recomendada: >= 18)
- npm (ou yarn)

### Passo a passo

1. Clone este repositório:

```bash
git clone https://github.com/anecrispim/front-end-teste-effecti.git
cd front-end-teste-effecti
```

2. Instalar dependências
   
```bash
npm install
```

3. Executar a aplicação localmente
   
```bash
npm run dev
```

4. Acessar no navegador

```bash
http://localhost:5173
```

## 🔗 Integração com a API

1. Certifique-se de que o back-end está rodando em:

```bash
http://localhost:8080
```
2. A aplicação Vue consome os dados da seguinte rota da API: GET /licitacoes/listar

## 🛠 Decisões Técnicas
- Vue 3 + Vite: escolhidos pela leveza, rapidez no setup e suporte moderno.
- **Vitest**: escolhido para testes unitários por ser nativamente compatível com Vite, ter inicialização rápida e oferecer uma API similar ao Jest.
- Axios: usado para comunicação com a API por ser leve e fácil de configurar.
- Composição de componentes: abordagem modular, separando a tela de filtros e listagem para manter legibilidade.
- Sem Vuex ou Pinia: a aplicação é simples o suficiente para controlar estado via ref e watch.
- Responsividade: layout flexível com CSS puro visando compatibilidade e simplicidade.

## 🧪 Como executar os testes

1. Talvez precise instalar o pacote
   
```bash
npm install -D vitest @vue/test-utils jsdom
```

2. Comando para executar o teste
   
```bash
npm run test
```
ou
```bash
npm run test:ui
```
