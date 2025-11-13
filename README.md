# auth-api-programa-ai

API de autenticação desenvolvida como parte do curso de **AppSec da
Programa.AI**, utilizando **Flask**, **SQLAlchemy** e **Flask-Migrate**.

## 🚀 Tecnologias utilizadas

-   Python 3.x\
-   Flask\
-   Flask-Migrate\
-   SQLAlchemy

## 📦 Como rodar o projeto

### 1. Clone o repositório

``` bash
git clone <URL_DO_REPO>
cd auth-api-programa-ai
```

### 2. Crie e ative o ambiente virtual

``` bash
python3 -m venv venv
source venv/bin/activate   # Linux/Mac
# ou
venv\Scripts\activate      # Windows
```

### 3. Instale as dependências

``` bash
pip install -r requirements.txt
```

## 🗄️ Configurando o banco de dados e migrações

### 1. Inicializar o diretório de migrações

``` bash
flask db init
```

### 2. Criar a migração inicial

``` bash
flask db migrate -m "init: users"
```

### 3. Aplicar as migrações

``` bash
flask db upgrade
```

## ▶️ Rodando o servidor Flask

``` bash
flask run
```

O servidor iniciará por padrão em: `http://127.0.0.1:5000`.

## 📝 Estrutura recomendada do projeto

    auth-api-programa-ai/
    │── app/
    │   ├── __init__.py
    │   ├── models/
    │   ├── routes/
    │   └── ...
    │── migrations/
    │── venv/
    │── requirements.txt
    │── README.md
