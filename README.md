# NLW Agents

Este projeto foi desenvolvido durante o evento NLW da Rocketseat.

## Descrição
Backend simples para gerenciamento de "rooms" (salas), utilizando Fastify, Drizzle ORM e PostgreSQL com suporte ao pgvector.

## Tecnologias e Bibliotecas
- **Node.js** + **TypeScript**
- **Fastify**: Framework web para Node.js
- **@fastify/cors**: Middleware CORS
- **Zod**: Validação de esquemas
- **fastify-type-provider-zod**: Integração Zod + Fastify
- **Drizzle ORM**: ORM para TypeScript
- **drizzle-kit**: Ferramentas para migração e seed
- **PostgreSQL**: Banco de dados relacional (com extensão pgvector)
- **docker-compose**: Para subir o banco localmente

## Padrões de Projeto
- **Modularização por responsabilidade** (rotas, banco, schema)
- **Validação de dados com Zod**
- **Environment variables** para configuração

## Setup e Configuração
1. **Clone o repositório**
2. **Instale as dependências**:
   ```bash
   npm install
   ```
3. **Configure o banco de dados** com Docker:
   ```bash
   docker-compose up -d
   ```
4. **Copie o arquivo de exemplo de variáveis de ambiente**:
   ```bash
   cp .env.example .env
   ```
   Edite `.env` conforme necessário.
5. **Rode as migrações e seeds** (se aplicável):
   ```bash
   npm run db:seed
   ```
6. **Inicie o servidor**:
   ```bash
   npm run dev
   ```

O backend estará disponível em `http://localhost:3333` (ajuste a porta no `.env` se necessário).
