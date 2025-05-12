# 🌈 API RESTful - Gerenciamento de Consultas Médicas | Lacrei Saúde

Este projeto é uma API desenvolvida como parte da contribuição voluntária para a Lacrei Saúde. Seu objetivo é facilitar o **gerenciamento de profissionais da saúde e consultas médicas** voltadas à comunidade LGBTQIAPN+, com foco em **qualidade, segurança, boas práticas** e **preparo para produção**.

---

## 🚀 Tecnologias Utilizadas

- [Python 3.11](https://www.python.org/)
- [Django 4.x](https://www.djangoproject.com/)
- [Django REST Framework](https://www.django-rest-framework.org/)
- [PostgreSQL](https://www.postgresql.org/)
- [Docker + Docker Compose](https://www.docker.com/)
- [Poetry](https://python-poetry.org/)
- GitHub Actions (CI/CD) - _em construção_

---

## 🧱 Funcionalidades da API

- CRUD de Profissionais da Saúde:
  - `nome_social`, `profissão`, `endereço`, `contato`
- CRUD de Consultas Médicas:
  - `data`, `profissional` (vinculado por chave estrangeira)
- Filtro por profissional via `GET /api/consultas/?profissional_id={id}`
- Retornos em JSON
- Validação e segurança de dados

---

## 🐳 Setup do Ambiente com Docker

### Pré-requisitos:
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/lacrei-api.git
cd lacrei-api

# Inicie os containers
docker-compose up --build
