# API de Gerenciamento de Eventos Extracurriculares

API RESTful para gerenciar eventos extracurriculares, desenvolvida com AdonisJS 5, TypeScript, Docker e PostgreSQL. A API permite que alunos se inscrevam em atividades, gerenciem suas inscrições e registrem presença.

## Tecnologias Utilizadas

- **AdonisJS 5**
- **TypeScript**
- **Docker**
- **PostgreSQL**

## Requisitos

- **Docker** e **Docker Compose** instalados no sistema.
- **Node.js** (versão 16+) e **npm** instalados, caso queira rodar o projeto sem Docker.

## Configuração

1. **Clone o repositório**:
   ```bash
   https://github.com/NaellyV/event-manager-api.git
   cd event-manager-api
2. **Configure o ambiente**:
   ```bash
   cp .env.example .env
3. **Suba os containers com Docker**:
   ```bash
    docker-compose up -d
4. **Execute as migrations para criar as tabelas no banco de dados**:
   ```bash
   docker-compose exec app node ace migration:run

   
# Estrutura do Banco de Dados

A API possui as seguintes tabelas principais:

  students: Armazena as informações dos alunos.
  api_tokens: Usada para gerenciar tokens de autenticação.
  activities: Contém os dados das atividades extracurriculares.
  enrollments: Relaciona os alunos com as atividades nas quais estão inscritos.
  presences: Armazena informações sobre a presença dos alunos nas atividades.
  
# Funcionalidades:

  Gerenciamento de Atividades: Listar, criar, atualizar e excluir atividades.
  Gerenciamento de Alunos: Registro e atualização de dados dos alunos.
  Inscrição em Atividades: Inscrever e cancelar a inscrição de alunos em atividades.
  Controle de Presença: Registrar e consultar a presença dos alunos nas atividades.
  
# Como Rodar os Testes: 
  ```bash
    docker-compose exec app npm run test











