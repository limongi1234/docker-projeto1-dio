# Docker Compose — Apache (DIO) 🐳

> 🔱 **Fork** de material da [DIO](https://www.dio.me), originalmente criado por **Denilson Bonatti**. Mantido aqui como referência de estudo — o código pertence ao autor original.

Exemplo introdutório de **Docker Compose** que sobe um servidor web **Apache (httpd)** em container, servindo arquivos de um diretório local.

## ⚙️ O que faz

O `compose.yml` define um serviço:

- **apache** — imagem `httpd:latest`, container `my-apache-app`
- Publica na **porta 80** (`80:80`)
- Monta o diretório local **`./website`** como raiz do servidor (`/usr/local/apache2/htdocs`)

## 🛠️ Tecnologias

![Docker](https://img.shields.io/badge/Docker_Compose-2496ED?style=flat&logo=docker&logoColor=white)
![Apache](https://img.shields.io/badge/Apache-D22128?style=flat&logo=apache&logoColor=white)

## 🚀 Como usar

```bash
git clone https://github.com/limongi1234/docker-projeto1-dio.git
cd docker-projeto1-dio

# coloque seus arquivos HTML na pasta ./website e suba o serviço
docker compose up -d
```

Acesse `http://localhost` no navegador. Para encerrar: `docker compose down`.

> 📚 Material de estudo sobre Docker Compose (curso DIO / Denilson Bonatti).
