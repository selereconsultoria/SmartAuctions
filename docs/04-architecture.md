# Smart Auction

# Software Architecture

Versão: 1.0

---

# Objetivo

Definir a arquitetura técnica da plataforma Smart Auction.

---

# Arquitetura Geral

Frontend

↓

Backend (API)

↓

Banco de Dados

↓

Workers

↓

Integrações com Leiloeiros

---

# Stack Tecnológica

## Frontend

- Next.js
- React
- TypeScript
- Tailwind CSS

---

## Backend

- NestJS
- TypeScript
- Prisma ORM

---

## Banco

- PostgreSQL

---

## Cache

- Redis

---

## Filas

- BullMQ

---

## Storage

- Amazon S3 ou Cloudflare R2

---

## Containers

- Docker
- Docker Compose

---

# Módulos

## Auth

Responsável por:

- Login
- Cadastro
- Recuperação de senha
- Permissões

---

## Companies

Responsável por:

- Empresas
- Planos
- Usuários

---

## Auction Collector

Responsável por:

- Integrações
- Importação
- Sincronização

---

## Vehicles

Responsável por:

- Cadastro
- Fotos
- Documentos
- Histórico

---

## Smart Engine

Responsável por:

- Smart Score
- Smart Profit
- Smart Risk
- Smart Advisor

---

## Alerts

Responsável por:

- Watchlist
- Alertas
- Notificações

---

## Analytics

Responsável por:

- Dashboard
- Indicadores
- Relatórios

---

## Admin

Responsável por:

- Administração
- Auditoria
- Configurações

---

# Comunicação

Frontend

↓

REST API

↓

Backend

↓

PostgreSQL

---

# Integrações

Cada leiloeiro deverá possuir um conector próprio.

Os conectores deverão converter os dados recebidos para o modelo padrão da Smart Auction.

Nenhum módulo interno deverá depender do formato original do leiloeiro.

---

# Segurança

- JWT
- Senhas criptografadas
- HTTPS
- Controle de acesso por perfil
- Auditoria de ações

---

# Logs

Registrar:

- Erros
- Integrações
- Login
- Atualizações
- Execução dos Workers

---

# Escalabilidade

A arquitetura deverá permitir:

- Inclusão de novos leiloeiros sem alterar o núcleo do sistema.
- Escalabilidade horizontal dos Workers.
- Separação futura entre API e Smart Engine.

---

# Versionamento

Git Flow

Branches:

- main
- develop
- feature/*
- hotfix/*
