# 💸 Fin-Tech Multitenancy – Sistema de Controle Financeiro SaaS  

> 🚀 Projeto acadêmico e experimental desenvolvido por **Viviane Aguiar**  
> com o objetivo de aplicar práticas reais de **engenharia de software**,  
> **arquitetura distribuída** e **microsserviços** em um contexto corporativo simulado.

---

## 🧭 Visão Geral  

O **Fin-Tech Multitenancy** é um sistema **SaaS (Software as a Service)** de **controle financeiro**,  
onde **cada cliente (tenant)** possui seu próprio **subdomínio isolado**, com dados e relatórios exclusivos.  

💡 O sistema foi projetado para explorar **autenticação centralizada**, **mensageria assíncrona**,  
**espelhamento de dados em tempo real** e **dashboards inteligentes** — tecnologias comuns em ambientes **FinTech corporativos**.

---

## 🧱 Arquitetura Geral  

A aplicação é composta por múltiplos serviços que se comunicam de forma **síncrona e assíncrona**:  

| Camada / Serviço | Função | Tecnologia |
|------------------|--------|-------------|
| 🖥️ **Frontend** | Interface web e chamadas à API | ![Next.js](https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nextjs/nextjs-original.svg) |
| ⚙️ **Backend (API)** | Processamento de transações e integração entre microsserviços | ![NestJS](https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nestjs/nestjs-plain.svg) |
| 🔐 **Autenticação** | Gerenciamento de usuários e tokens JWT | ![Keycloak](https://cdn.jsdelivr.net/gh/devicons/devicon/icons/keycloak/keycloak-original.svg) |
| 🧵 **Mensageria** | Comunicação assíncrona entre serviços | ![Apache Kafka](https://cdn.jsdelivr.net/gh/devicons/devicon/icons/apachekafka/apachekafka-original.svg) |
| 🧩 **Espelhamento de dados** | Sincronização automática com o ElasticSearch | ![Kafka Connect](https://img.shields.io/badge/Kafka%20Connect-black?logo=apachekafka) |
| 📊 **Dashboards e Métricas** | Visualização analítica e relatórios financeiros | ![Kibana](https://cdn.jsdelivr.net/gh/devicons/devicon/icons/kibana/kibana-original.svg) |
| 💾 **Banco de Dados** | Armazenamento relacional principal | ![PostgreSQL](https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg) |

---

## 🧠 Principais Funcionalidades

- 🧍‍♂️ **Login e autenticação multitenant** via Keycloak  
- 💰 **Registro de transações financeiras** (ganhos, despesas, investimentos)  
- 📅 **Geração de relatórios personalizados** por período  
- ⚡ **Processamento assíncrono** de relatórios via Apache Kafka  
- 🪶 **Espelhamento de dados** no Elasticsearch com Kafka Connect  
- 📈 **Dashboards de métricas** integrados ao Kibana  
- ☁️ **Armazenamento em nuvem** de relatórios (Cloud Storage simulado)

---

## 🧩 Arquitetura de Microsserviços  

```
[Next.js] ⇄ [NestJS API] ⇄ [PostgreSQL]
        ↘︎
         [Apache Kafka] ⇄ [Relatórios Service] ⇄ [Elasticsearch] ⇄ [Kibana]
             ↘︎
              [Keycloak]
```

---

## 📘 Diagrama de Casos de Uso  

📎 [**Clique aqui para visualizar o Diagrama de Casos de Uso**](./docs/FinTech_Use_Case_fixed.puml)  
> *(adicione o arquivo `.puml` ou exporte a imagem `.svg` dentro da pasta `/docs` do repositório)*

---

## 🧰 Tecnologias e Ferramentas Utilizadas  

| Categoria | Ferramenta / Framework |
|------------|-----------------------|
| Backend | NestJS, Node.js, TypeScript |
| Frontend | Next.js, React |
| Autenticação | Keycloak |
| Mensageria | Apache Kafka, Kafka Connect |
| Banco de Dados | PostgreSQL |
| Observabilidade | Elasticsearch, Kibana |
| DevOps / Infra | Docker, Docker Compose |
| Controle de Versão | Git + GitHub |
| Documentação | Markdown, PlantUML |

---

## 🧑‍💻 Autora  

**👩‍💻 Viviane Aguiar**  
Desenvolvedora Fullstack | Estudante de Engenharia de Software  
📍 Juiz de Fora – MG, Brasil  
📧 [vivianeaguiarc@outlook.com](mailto:vivianeaguiarc@outlook.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/vivianeaguiar) • [GitHub](https://github.com/vivianeaguiar)

---

## 🗂️ Estrutura Inicial do Projeto

```
fintech-multitenancy/
│
├── backend/               # API principal (NestJS)
├── frontend/              # Interface Web (Next.js)
├── keycloak/              # Configurações do servidor Keycloak
├── kafka/                 # Configuração de tópicos e brokers
├── reports-service/       # Serviço de geração de relatórios
├── elasticsearch/         # Índices de dados
├── kibana/                # Dashboards
├── docs/                  # Diagramas e documentação
│   └── FinTech_Use_Case_fixed.puml
└── README.md
```

---

## ⚙️ Como Executar (Em breve)

📦 **Em construção...**  
Os passos de instalação e execução via Docker Compose serão adicionados nas próximas versões.  

---

⭐ **Dê uma estrela no repositório se este projeto te inspirou!**  
> “A melhor forma de aprender é construindo.”
