# 📚 Bookstore App (Projeto Prático)

> Este projeto foi desenvolvido durante um curso prático de Backend em Python na EBAC. Embora tenha sido acompanhado passo a passo pelo professor, considero esta aplicação fundamental para conhecer e consolidar as tecnologias envolvidas.

---

## 🔍 Descrição

Bookstore App é uma aplicação de exemplo construída para exercitar conceitos de backend em Python, utilizando boas práticas de desenvolvimento, gerenciamento de dependências e conteinerização. Este projeto serve como base para compreender:

- Arquitetura de projetos Django
- Gerenciamento de dependências com Poetry
- Contêineres Docker e orquestração com Docker Compose
- Processos de migração e testes automatizados

Mesmo tendo sido implementado de forma orientada, obtenho neste exercício uma visão clara de cada etapa essencial para criar, manter e escalar uma API em Python.

---

## 🛠️ Tecnologias e Ferramentas

- **Python 3.5+**
- **Poetry**: Gerenciamento de dependências e ambiente virtual
- **Django**: Framework web para construção do backend
- **Docker** & **Docker Compose**: Conteinerização e orquestração de serviços

---

## 🚀 Pre requisitos

Antes de começar, certifique-se de ter instalado:

- Python 3.5 ou superior
- [Poetry](https://python-poetry.org/)
- [Docker](https://www.docker.com/) e [Docker Compose](https://docs.docker.com/compose/)

---

## 🏁 Quickstart

### 1️⃣ Clonar o repositório

```bash
git clone git@github.com:drsantos20/bookstore.git
cd bookstore
```

### 2️⃣ Instalar dependências (Poetry)

```bash
poetry install
```

### 3️⃣ Executar localmente (sem Docker)

```bash
# Aplicar migrações
poetry run python manage.py migrate

# Iniciar servidor de desenvolvimento
poetry run python manage.py runserver
```

Acesse a aplicação em `http://127.0.0.1:8000/`.

### 4️⃣ Executar com Docker

```bash
# Construir e iniciar containers em background
docker-compose up -d --build

# Aplicar migrações dentro do container web
docker-compose exec web python manage.py migrate
```

### 5️⃣ Executar testes automatizados

```bash
docker-compose exec web python manage.py test
```

---

## 📝 Observações

- Este projeto foi desenvolvido como parte de um treinamento prático e serve como ponto de partida para projetos reais em Python.
- Recomendado revisar individualmente cada configuração (Poetry, Docker, Django) para aprofundar o entendimento.

---

## 🤝 Contribuições

Fique à vontade para abrir issues ou pull requests com sugestões de melhorias!

---

##### Desenvolvido como projeto prático durante o curso de Backend Python na EBAC
