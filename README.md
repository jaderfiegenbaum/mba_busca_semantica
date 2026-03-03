# mba_busca_semantica

## Requisitos

- Python 3.10+
- Docker

## Instalação

Clone o repositório e entre na pasta do projeto. Em seguida, crie e ative um ambiente virtual:

```bash
python -m venv .venv
source .venv/bin/activate
```

Instale as dependências:

```bash
pip install -r requeriments.txt
```

Copie o arquivo de exemplo e preencha com suas credenciais:

```bash
cp .env.example .env
```

## Banco de dados

Suba o PostgreSQL com a extensão PGVector via Docker:

```bash
docker compose up -d
```

## Ingestão

Com o banco rodando e o `.env` configurado, execute:

```bash
python src/ingest.py
```
