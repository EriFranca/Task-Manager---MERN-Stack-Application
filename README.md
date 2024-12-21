# Task Manager - MERN Stack Application

Uma aplicação web moderna e completa para gerenciamento de tarefas, construída utilizando MongoDB, Express.js, React.js e Node.js (MERN Stack). O projeto demonstra a implementação de uma aplicação full-stack com autenticação, CRUD completo e interface responsiva.

## 📋 Visão Geral

O Task Manager permite que usuários criem, organizem e gerenciem suas tarefas diárias de forma eficiente. A aplicação oferece uma experiência fluida com atualizações em tempo real e uma interface intuitiva.

### Funcionalidades Principais

O Task Manager possui um conjunto robusto de funcionalidades:

- Autenticação completa com JWT (JSON Web Tokens)
- Criação, edição e exclusão de tarefas
- Categorização de tarefas por status e prioridade
- Filtros e busca avançada
- Dashboard com métricas e visualizações
- Sistema de lembretes e notificações
- Interface responsiva e intuitiva

## 🛠️ Stack Tecnológica

### Backend
- **MongoDB**: Banco de dados NoSQL para armazenamento flexível de dados
- **Express.js**: Framework web rápido e minimalista para Node.js
- **Node.js**: Ambiente de execução JavaScript do lado do servidor
- **Mongoose**: ODM (Object Data Modeling) para MongoDB e Node.js

### Frontend
- **React.js**: Biblioteca JavaScript para construção de interfaces
- **Redux Toolkit**: Gerenciamento de estado da aplicação
- **React Router**: Navegação e roteamento
- **Material-UI**: Framework de componentes React para design responsivo

### Ferramentas de Desenvolvimento
- **TypeScript**: Adiciona tipagem estática ao JavaScript
- **ESLint**: Ferramenta de linting para identificar problemas no código
- **Prettier**: Formatador de código
- **Jest**: Framework de testes
- **Docker**: Containerização da aplicação

## 🚀 Instalação e Configuração

### Pré-requisitos
- Node.js (versão 14 ou superior)
- MongoDB (local ou Atlas)
- npm ou yarn

### Passos para Instalação

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/task-manager-mern.git
cd task-manager-mern
```

2. Instale as dependências do backend:
```bash
cd backend
npm install
```

3. Instale as dependências do frontend:
```bash
cd ../frontend
npm install
```

4. Configure as variáveis de ambiente:

Backend (.env):
```env
MONGODB_URI=sua_uri_mongodb
JWT_SECRET=seu_jwt_secret
PORT=5000
NODE_ENV=development
```

Frontend (.env):
```env
REACT_APP_API_URL=http://localhost:5000/api
REACT_APP_ENV=development
```

5. Inicie a aplicação:

Em um terminal (backend):
```bash
cd backend
npm run dev
```

Em outro terminal (frontend):
```bash
cd frontend
npm start
```

## 📁 Estrutura do Projeto

```
task-manager/
├── backend/
│   ├── src/
│   │   ├── controllers/    # Controladores da aplicação
│   │   ├── models/         # Modelos do Mongoose
│   │   ├── routes/         # Rotas da API
│   │   ├── middleware/     # Middlewares personalizados
│   │   └── config/         # Configurações
│   ├── tests/              # Testes do backend
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── components/     # Componentes React
│   │   ├── pages/         # Páginas da aplicação
│   │   ├── redux/         # Configuração do Redux
│   │   ├── services/      # Serviços e APIs
│   │   └── utils/         # Utilitários
│   ├── tests/             # Testes do frontend
│   └── package.json
│
└── docker-compose.yml
```

## 🧪 Testes

O projeto inclui testes unitários e de integração:

Backend:
```bash
cd backend
npm run test        # Executa todos os testes
npm run test:watch  # Modo watch
npm run test:coverage # Relatório de cobertura
```

Frontend:
```bash
cd frontend
npm run test
npm run test:coverage
```

## 📊 API Endpoints

A API REST segue as melhores práticas RESTful:

### Autenticação
- `POST /api/auth/register`: Registro de usuário
- `POST /api/auth/login`: Login de usuário
- `GET /api/auth/me`: Obtém dados do usuário atual

### Tarefas
- `GET /api/tasks`: Lista todas as tarefas
- `POST /api/tasks`: Cria nova tarefa
- `GET /api/tasks/:id`: Obtém uma tarefa específica
- `PUT /api/tasks/:id`: Atualiza uma tarefa
- `DELETE /api/tasks/:id`: Remove uma tarefa

## 🔒 Segurança

Implementamos várias medidas de segurança:

- Autenticação JWT
- Sanitização de dados
- Rate limiting
- Validação de entrada
- Proteção contra ataques comuns (XSS, CSRF)

## 🚀 Deploy

### Usando Docker

1. Construa as imagens:
```bash
docker-compose build
```

2. Inicie os containers:
```bash
docker-compose up -d
```

### Deploy Manual

Documentação detalhada para deploy em diferentes plataformas:
- Heroku
- DigitalOcean
- AWS
- Vercel (frontend)

## 📈 Monitoramento

A aplicação inclui monitoramento através de:
- Morgan para logging de requisições
- Winston para logging personalizado
- Sentry para rastreamento de erros

## 🤝 Contribuição

1. Faça um fork do projeto
2. Crie sua branch de feature (`git checkout -b feature/NovaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/NovaFeature`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT - veja o arquivo [LICENSE.md](LICENSE.md) para detalhes.

## 👥 Autores

- Eri França - ecfs1988@hotmail.com

## 📞 Suporte

Para suporte, envie um email para exemplo@email.com ou abra uma issue no GitHub.

## 🙏 Agradecimentos

- MongoDB por prover hosting gratuito
- Comunidade MERN Stack
- Todos os contribuidores
