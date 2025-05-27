# 🪙 Budget Roots – Overview

[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](./LICENSE)


Welcome to the **Budget Roots** project – an open, modular system to help individuals and households manage their
finances transparently and collaboratively.

This repository acts as the **overview and documentation hub** for the entire Budget Roots ecosystem, maintained under
the [Budget Roots GitHub Organization](https://github.com/budget-roots).

---

## 🔍 What Is Budget Roots?

**Budget Roots** is a Kotlin-based microservice system for:

- 💶 Managing personal and shared income/expenses
- 🧑‍🤝‍🧑 Supporting households with multiple members
- ⚖️ Fairly splitting costs based on individual net income
- 💡 Providing budget recommendations per person and household
- 🧾 Keeping personal and shared finances strictly separated

---

## 🧱 Architecture Overview

Budget Roots is built using a clean microservice architecture. Each core domain is modeled as a separate, independently
deployable service.

| Microservice                                                                                             | Description                                          |
|----------------------------------------------------------------------------------------------------------|------------------------------------------------------|
| [`budget-roots-household-service`](https://github.com/budget-roots/budget-roots-household-service)       | Manages households, members, and roles               |
| [`budget-roots-personal-transaction`](https://github.com/budget-roots/budget-roots-personal-transaction) | Tracks personal income and private expenses          |
| [`budget-roots-shared-transaction`](https://github.com/budget-roots/budget-roots-shared-transaction)     | Handles shared household costs and fair distribution |
| [`budget-roots-budget-service`](https://github.com/budget-roots/budget-roots-budget-service)             | Suggests savings, allocations & spending strategies  |
| [`budget-roots-reporting-service`](https://github.com/budget-roots/budget-roots-reporting-service)       | Aggregates data and provides analytics               |
| [`budget-roots-gateway`](https://github.com/budget-roots/budget-roots-gateway)                           | Central API gateway with routing and auth            |

---

## ⚙️ Tech Stack

- 🧑 Kotlin + Spring Boot
- 🛠️ Gradle
- 🐳 Docker
- 📡 Prometheus + Grafana
- 📬 Kafka
- 🧪 Testcontainers
- 🗂️ OpenAPI / Swagger

---

## 🚧 Getting Started

Each microservice has its own repo, README, and Dockerfile. For local development:

---

## 📜 License

BudgetRoots is Open Source software released under
the [Apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0.html).
