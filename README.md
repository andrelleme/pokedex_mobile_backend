# Pokédex – Agenda Pokémon (Backend)

Este repositório contém o backend da aplicação **Pokédex**, desenvolvido para a disciplina de **Desenvolvimento para Dispositivos Móveis**.  
A API foi construída em **Python** com **Django**, sendo responsável por fornecer os dados consumidos pelo aplicativo Android.

---

## Tecnologias Utilizadas

- **Linguagem:** Python 3.8  
- **Framework:** Django 4.2 (LTS)  
- **Banco de Dados:** PostgreSQL  
- **Arquitetura:** MVC com camada de Negócio separada (Business Objects – BO)  
- **Outros:** Django REST (utilizado para CORS), Psycopg2  

---

## Estrutura do Projeto

```
backend/
│
├── api/                # Views (Controllers) e Models
├── BO/                 # Regras de negócio
│   ├── bo.py           # Lógica principal dos Pokémons
│   ├── auth_bo.py      # Lógica de autenticação
│   └── scripts_dados/  # Scripts para popular o banco
│
└── setup/              # Configurações globais do Django (settings.py)
```

---

## Instalação e Configuração

Siga os passos abaixo para executar o projeto localmente.

### 1. Pré-requisitos

- Python 3.8  
- PostgreSQL  
- Banco de dados criado no PostgreSQL com o nome: `pokedex_db`

---

### 2. Clonagem do Repositório

```bash
git clone <link-do-seu-repositorio>
cd backend
```

---

### 3. Criação do Ambiente Virtual

```bash
python -m venv venv
```

Ative o ambiente:

**Windows**
```bash
.\venv\Scripts\activate
```

**Linux / macOS**
```bash
source venv/bin/activate
```

---

### 4. Instalação das Dependências

```bash
pip install -r requirements.txt
```

---

### 5. Configuração do Banco de Dados

Execute as migrações para criar as tabelas:

```bash
python manage.py migrate
```

---

### 6. Popular o Banco de Dados

O comando abaixo cria automaticamente:

- 3 usuários  
- 10 pokémons  

```bash
python popular_banco.py
```

---

### 7. Executar o Servidor

```bash
python manage.py runserver
```

Após isso, a API estará disponível para consumo pelo aplicativo mobile.
=======
# projeto_mobile_webservice_pokedex
>>>>>>> f0b26395df47a672eaaa4fa4c9b3b15934b0eeb0
