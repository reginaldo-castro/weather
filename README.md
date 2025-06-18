# 🌦️ Weather Dashboard

Um dashboard simples de previsão do tempo, desenvolvido com **Django**, integrado com a API da **OpenWeather**, e containerizado utilizando **Docker**.

## 🚀 Funcionalidades

- 🔍 Busca da previsão do tempo atual por cidade.
- 🌤️ Exibe informações como:
  - Temperatura atual
  - Sensação térmica
  - Descrição do clima (ex.: céu limpo, nublado)
- 🌎 Suporte para múltiplas cidades e países.
- 🔧 Pronto para desenvolvimento local via Docker Compose.

## 🛠️ Tecnologias

- Django 🐍
- Python 3.12
- Docker 🐳
- PostgreSQL 🐘
- OpenWeather API ☁️

## 🗂️ Estrutura do Projeto
    
    ├── docker-compose.yml
    ├── Dockerfile
    ├── .env
    ├── requirements.txt
    ├── weather_dashboard/ # Projeto Django
    │ ├── weatherapp/ # App Django
    │ ├── static/ # Arquivos estáticos
    │ └── templates/ # Templates HTML


## ⚙️ Configuração e Execução

### 🔑 1. Obter a API Key

- Crie uma conta gratuita em [https://openweathermap.org/](https://openweathermap.org/)
- Obtenha sua **API Key**.

### 🗒️ 2. Criar o arquivo `.env`

Crie um arquivo chamado `.env` na raiz do projeto com o seguinte conteúdo:

```env
POSTGRES_DB=weatherdb
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres
OPENWEATHERMAP_API_KEY=sua_api_key_aqui
DB_HOST=db
DB_PORT=5432
```

🐳 3. Subir os containers
```
docker-compose up --build
```
🔗 4. Acessar a aplicação
```
Acesse no navegador: http://localhost:8000
```
🐘 Acesso ao banco PostgreSQL (opcional)

Host: localhost
Porta: 5432
Usuário: postgres
Senha: postgres
Banco: weatherdb

🗑️ Parar os containers
```
docker-compose down
```

✅ Melhorias Futuras
⏰ Previsão horária e semanal
🗺️ Localização automática por IP
🎨 Interface responsiva e aprimorada
🌍 Suporte a múltiplos idioma

🤝 Contribuição
Sinta-se livre para abrir issues, sugerir melhorias ou enviar pull requests.

📜 Licença
Este projeto está licenciado sob a licença MIT. Consulte o arquivo LICENSE para mais informações.

