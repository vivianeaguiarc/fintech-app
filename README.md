# 💼 SaaS Multitenancy Financeiro

> Estudo de caso prático: sistema financeiro multiempresa com autenticação centralizada e arquitetura de microsserviços.

## 🚀 Visão Geral

Este projeto simula um SaaS multitenancy de controle financeiro, aplicando tecnologias usadas em grandes corporações para autenticação, mensageria e observabilidade.

Cada cliente possui um subdomínio exclusivo e pode gerenciar suas finanças, emitir relatórios e acompanhar métricas em um dashboard interativo.

## 🧩 Arquitetura

- **Backend:** NestJS + PostgreSQL
- **Frontend:** Next.js + TypeScript
- **Autenticação:** Keycloak
- **Mensageria:** Apache Kafka + Kafka Connect
- **Observabilidade:** Elasticsearch + Kibana
- **Infraestrutura:** Docker e Docker Compose

## 🔐 Autenticação

- Centralizada via Keycloak
- Validação de tokens JWT por chave pública
- Associação entre usuários e empresas (tenants)

## 📊 Relatórios Assíncronos

- Solicitação via API → Kafka
- Processamento assíncrono via microsserviço
- Sincronização via Kafka Connect
- Armazenamento no Elasticsearch
- Download via Cloud Storage

## 📁 Estrutura de Branches

| Branch | Função |
|--------|--------|
| main | versão estável |
| develop | integração principal |
| feat/* | novas features |
| fix/* | correções |
| chore/* | manutenção |
| docs/* | documentação |


## 👩‍💻 Autora

**Viviane Aguiar**  
Desenvolvedora Fullstack & Entusiasta de Arquiteturas Escaláveis  
📍 Juiz de Fora – MG  
📧 vivianeaguiarc@outlook.com  
[LinkedIn](https://www.linkedin.com/in/vivianeaguiar)
