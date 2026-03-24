## 🚗 API de Carros em PHP (PDO)

## API simples desenvolvida em PHP puro utilizando PDO, com foco em praticar operações básicas de back-end e consumo de API REST.

## 📌 Tecnologias utilizadas
PHP
PDO (PHP Data Objects)
MySQL
Thunder Client (testes de requisições)

## ⚙️ Funcionalidades
✅ Criar carros (POST)
📄 Listar carros (GET)
✏️ Atualizar carros (PUT / PATCH)
❌ Deletar carros (DELETE)

## 🗄️ Configuração do Banco de Dados
1. Criar o banco
CREATE DATABASE consumo_api;

2. Criar a tabela
CREATE TABLE carros (
    id INT AUTO_INCREMENT PRIMARY KEY,
    tipo VARCHAR(100),
    categoria VARCHAR(100),
    modelo VARCHAR(100),
    ano DATE,
    valor DECIMAL(10,2)
);

## 🚀 Configuração do Projeto
1. Clone o repositório
git clone <url-do-repositorio>

2. Acesse a pasta
cd nome-do-projeto

3. Configure o arquivo .env
DB_HOST=localhost
DB_NAME=consumo_api
DB_USER=root
DB_PASS=sua_senha

## ▶️ Rodando o projeto
Inicie o servidor local com:
php -S localhost:8000

## 🔗 Endpoints da API
Para alterar as funcionalidades, mude apenas o método, os endpoints continuam os mesmos

Métodos   Descrição:
GET    =  Lista todos os carros 
POST   =  Cria um novo carro
PUT    =  Atualiza um carro
DELETE =  Remove um carro

## 🧪 Testes
A API foi testada utilizando o Thunder Client no VS Code, mas pode ser utilizada com:
Postman
Insomnia
cURL

## ⚠️ Observações
Projeto desenvolvido para fins de estudo
Não possui autenticação
Não possui validações robustas
Não segue ainda um padrão arquitetural (ex: MVC completo)

## 🎯 Objetivo
Este projeto foi desenvolvido para praticar:

Criação de APIs REST com PHP puro
Manipulação de banco de dados com PDO
Estruturação de rotas
Testes de requisições HTTP

## 📈 Possíveis melhorias

Implementar validações de dados
Adicionar autenticação (JWT, Session, etc.)
Separar em arquitetura MVC
Criar versionamento de API (/v1/)
Implementar tratamento de erros padronizado
Usar migrations ao invés de SQL manual
