# Smart Auction

# API Specification

Versão: 1.0

---

# Base URL

/api/v1

---

# Authentication

POST /auth/login

POST /auth/register

POST /auth/forgot-password

POST /auth/reset-password

GET /auth/me

POST /auth/logout

---

# Users

GET /users

GET /users/{id}

POST /users

PUT /users/{id}

DELETE /users/{id}

---

# Companies

GET /companies

GET /companies/{id}

POST /companies

PUT /companies/{id}

---

# Auction Houses

GET /auction-houses

GET /auction-houses/{id}

POST /auction-houses

PUT /auction-houses/{id}

---

# Auctions

GET /auctions

GET /auctions/{id}

POST /auctions

PUT /auctions/{id}

---

# Vehicles

GET /vehicles

GET /vehicles/{id}

POST /vehicles

PUT /vehicles/{id}

DELETE /vehicles/{id}

---

# Vehicle Search

GET /vehicles/search

Filtros disponíveis:

- Marca
- Modelo
- Ano
- Leiloeiro
- Estado
- Cidade
- Score
- Lucro
- Risco
- Faixa de preço

---

# Favorites

GET /favorites

POST /favorites

DELETE /favorites/{id}

---

# Alerts

GET /alerts

POST /alerts

PUT /alerts/{id}

DELETE /alerts/{id}

---

# Dashboard

GET /dashboard

Retorna:

- Total de oportunidades
- Favoritos
- Alertas
- Score médio
- Lucro potencial

---

# Analytics

GET /analytics

GET /analytics/profit

GET /analytics/performance

GET /analytics/history

---

# Smart Engine

GET /analysis/{vehicleId}

Retorna:

- Smart Score
- Smart Profit
- Smart Risk
- Smart Advisor

---

# Notifications

GET /notifications

PUT /notifications/{id}/read

DELETE /notifications/{id}

---

# Admin

GET /admin/logs

GET /admin/jobs

GET /admin/integrations

POST /admin/sync

---

# Response Pattern

Success

{
  "success": true,
  "data": {}
}

Error

{
  "success": false,
  "message": "Descrição do erro."
}
