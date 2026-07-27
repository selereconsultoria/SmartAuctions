# Smart Auction

# Database Model

Versão: 1.0

---

# Entidades Principais

## Company

Representa uma empresa cliente.

Campos:

- id
- nome
- cnpj
- plano
- status
- created_at
- updated_at

---

## User

Representa um usuário da plataforma.

Campos:

- id
- company_id
- nome
- email
- senha_hash
- perfil
- status
- ultimo_login
- created_at
- updated_at

---

## AuctionHouse

Representa um leiloeiro.

Campos:

- id
- nome
- site
- tipo_integracao
- status

---

## Auction

Representa um leilão.

Campos:

- id
- auction_house_id
- titulo
- data_inicio
- data_fim
- status

---

## Vehicle

Representa um veículo.

Campos:

- id
- auction_id
- lote
- placa
- chassi
- marca
- modelo
- versao
- ano_fabricacao
- ano_modelo
- combustivel
- cambio
- cor
- km
- cidade
- estado
- fipe
- lance_atual
- valor_minimo
- status

---

## VehiclePhoto

Campos:

- id
- vehicle_id
- url
- ordem

---

## VehicleDocument

Campos:

- id
- vehicle_id
- tipo
- url

---

## SmartAnalysis

Resultado dos algoritmos.

Campos:

- id
- vehicle_id
- smart_score
- smart_profit
- smart_risk
- advisor
- updated_at

---

## Favorite

Campos:

- id
- user_id
- vehicle_id
- created_at

---

## Alert

Campos:

- id
- user_id
- tipo
- parametros
- ativo

---

## Notification

Campos:

- id
- user_id
- titulo
- mensagem
- tipo
- lida
- created_at

---

## VehicleHistory

Histórico do veículo.

Campos:

- id
- vehicle_id
- evento
- valor_anterior
- valor_novo
- created_at

---

## AuditLog

Registro das ações do sistema.

Campos:

- id
- user_id
- acao
- ip
- created_at
