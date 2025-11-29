# 🏦 Enterprise Ledger Microservice

A dedicated microservice for handling **Double-Entry Accounting** and **Transaction Reconciliations**. Designed to handle 500+ TPS (Transactions Per Second) with idempotency keys to prevent duplicate charges.

## 🔐 Architecture (NDA Redacted)
- **Language:** TypeScript / Node.js
- **Database:** PostgreSQL (Partitioned Tables)
- **Queuing:** Redis + BullMQ for asynchronous transaction processing.
- **Precision:** Uses `decimal.js` to avoid floating-point math errors in financial calculations.

## 🛠️ Key Features
- **Idempotency:** Ensures API requests are processed exactly once.
- **Audit Trails:** Immutable logs for all credit/debit operations.
- **Event Sourcing:** Publishes balance updates to Kafka/RabbitMQ.

---
*Status: Production (Private Client)*
