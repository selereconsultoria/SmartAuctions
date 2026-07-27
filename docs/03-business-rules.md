# Smart Auction

# Business Rules

Versão: 1.0

---

# 1. Smart Score

## Objetivo

Classificar automaticamente cada veículo entre 0 e 100 pontos.

Quanto maior a pontuação, maior o potencial da oportunidade.

---

## Faixas

| Score | Classificação |
|-------:|---------------|
| 90 - 100 | Excelente |
| 80 - 89 | Muito Boa |
| 70 - 79 | Boa |
| 60 - 69 | Atenção |
| 0 - 59 | Alto Risco |

---

# 2. Critérios do Smart Score

| Critério | Peso |
|----------|------|
| Diferença para FIPE | 25% |
| Liquidez do modelo | 20% |
| Estado do veículo | 15% |
| Histórico documental | 10% |
| Quilometragem | 10% |
| Ano do veículo | 10% |
| Tipo de leilão | 5% |
| Demanda de mercado | 5% |

Total: 100%

---

# 3. Smart Profit

Objetivo:

Calcular automaticamente o lucro estimado.

Fórmula inicial:

Lucro Estimado =
Preço de Mercado
- Lance
- Comissão
- Taxas
- Frete
- Documentação
- Reparo Estimado

---

# 4. Smart Risk

Classificação:

Baixo

Médio

Alto

Crítico

Fatores analisados:

- Sinistro
- Recuperado de financiamento
- Pequena monta
- Média monta
- Grande monta
- Enchente
- Ausência de documentos
- Chaves
- Funcionando

---

# 5. Smart Advisor

O sistema deverá recomendar uma ação.

Possíveis recomendações:

COMPRAR

ANALISAR

AGUARDAR

DESCARTAR

Cada recomendação deverá apresentar os motivos.

---

# 6. Watchlist

O usuário poderá favoritar veículos.

Sempre que ocorrer:

- alteração de lance
- alteração de status
- novo documento
- aproximação do encerramento

o sistema deverá gerar uma notificação.

---

# 7. Alertas

O usuário poderá criar alertas por:

Marca

Modelo

Ano

Faixa de preço

Estado

Leiloeiro

Score mínimo

Lucro mínimo

---

# 8. Atualização

Os veículos deverão ser sincronizados periodicamente.

Cada atualização deverá registrar:

Data

Hora

Origem

Status

---

# 9. Histórico

Todas as alterações importantes deverão ser armazenadas.

Exemplos:

Mudança de lance

Mudança de status

Mudança de score

Mudança de documentação

Mudança de preço

---

# 10. Auditoria

Toda ação do usuário deverá ser registrada.

Exemplos:

Login

Logout

Favoritou

Removeu favorito

Criou alerta

Alterou cadastro
