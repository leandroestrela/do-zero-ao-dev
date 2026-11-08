# 🏢 CondoSmart — Plataforma Inteligente de Gestão de Condomínios

**Tudo o que seu condomínio precisa, em um só lugar.**

O **CondoSmart** é uma proposta de plataforma web desenvolvida para centralizar e modernizar a gestão de condomínios residenciais. O projeto busca facilitar a comunicação entre moradores e administração, organizar processos administrativos e proporcionar maior controle sobre as atividades do condomínio.

A solução reúne funcionalidades de gerenciamento de moradores, unidades residenciais, visitantes, reservas de áreas comuns, comunicados, ocorrências e cobranças condominiais.

---

## 🎯 Objetivo do Projeto

Desenvolver uma plataforma centralizada que simplifique a administração de condomínios residenciais, reduzindo processos manuais, melhorando a organização das informações e proporcionando mais transparência, segurança e praticidade aos usuários.

## ✨ Principais Funcionalidades

- **Gestão de moradores e unidades:** cadastro, consulta e gerenciamento de moradores e unidades residenciais.
- **Controle de visitantes:** autorização antecipada de visitantes e registro de entrada e saída pela portaria.
- **Reserva de áreas comuns:** agendamento e cancelamento de espaços compartilhados do condomínio.
- **Comunicados:** publicação de avisos e informações importantes pela administração.
- **Ocorrências e manutenção:** registro e acompanhamento de problemas e solicitações dos moradores.
- **Gestão de funcionários:** cadastro e gerenciamento dos colaboradores do condomínio.
- **Gestão financeira:** gerenciamento de cobranças condominiais e consulta da situação financeira.
- **Notificações:** atualização dos usuários sobre comunicados, reservas e ocorrências.
- **Relatórios administrativos:** geração e consulta de informações para auxiliar a administração.

## 🛠️ Tecnologias e Ferramentas

A arquitetura tecnológica planejada para o projeto contempla:

| Tecnologia | Aplicação |
|---|---|
| React | Desenvolvimento da interface |
| TypeScript | Tipagem e organização do frontend |
| Java 21 | Desenvolvimento do backend |
| Spring Boot | Construção da API REST |
| PostgreSQL | Banco de dados relacional |
| Docker | Containerização da aplicação |
| GitHub Actions | Automação de CI/CD |
| Flyway | Gerenciamento de migrações do banco |
| OpenAPI / Swagger | Documentação da API |

## 🏗️ Arquitetura do Sistema

O CondoSmart foi projetado utilizando uma arquitetura cliente-servidor com backend organizado em um **monólito modular**.

A estrutura contempla três componentes principais:

- **Frontend:** interface web responsiva desenvolvida com React e TypeScript.
- **Backend:** aplicação Java com Spring Boot, responsável pelas regras de negócio, autenticação e disponibilização dos serviços por meio de uma API REST.
- **Banco de dados:** PostgreSQL, responsável pelo armazenamento e gerenciamento das informações.

A comunicação entre frontend e backend ocorre por meio de requisições HTTP utilizando JSON e HTTPS.

## 📁 Estrutura do Repositório

```text
condosmart/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── Dockerfile
│
├── backend/
│   ├── src/
│   ├── pom.xml
│   └── Dockerfile
│
├── database/
│   └── migrations/
│
├── docs/
│   ├── arquitetura/
│   ├── uml/
│   └── api/
│
├── docker-compose.yml
├── .env.example
└── README.md
```

## 🔐 Segurança

A proposta considera mecanismos de segurança para proteger as informações dos usuários e do condomínio:

- Autenticação utilizando e-mail e senha.
- Autorização baseada em perfis de acesso (RBAC).
- Utilização de JWT para autenticação.
- Criptografia de informações sensíveis.
- Armazenamento seguro de senhas com BCrypt ou Argon2.
- Comunicação protegida por HTTPS.
- Registros de auditoria para operações sensíveis.
- Adequação às diretrizes da Lei Geral de Proteção de Dados (LGPD).

## 👥 Perfis de Usuário

O sistema prevê cinco perfis principais:

| Perfil | Responsabilidade |
|---|---|
| Morador | Consultar informações, autorizar visitantes, realizar reservas e registrar ocorrências. |
| Síndico | Administrar o condomínio, gerenciar cobranças, funcionários e comunicados. |
| Porteiro | Consultar autorizações e registrar entradas e saídas de visitantes. |
| Funcionário | Acessar as funcionalidades relacionadas às atividades operacionais autorizadas. |
| Administrador | Gerenciar usuários, configurações e aspectos de segurança da plataforma. |

## 📋 Metodologia de Desenvolvimento

O planejamento do projeto utiliza a metodologia **Scrum**, com organização das atividades em sprints de duas semanas.

O desenvolvimento foi planejado considerando etapas de:

1. Levantamento e análise de requisitos.
2. Modelagem e arquitetura do sistema.
3. Planejamento e estruturação do banco de dados.
4. Desenvolvimento do frontend e backend.
5. Integração dos componentes.
6. Testes e validação.
7. Documentação e preparação da entrega.

---

**CondoSmart — Gestão inteligente, organização e praticidade para o seu condomínio.**
