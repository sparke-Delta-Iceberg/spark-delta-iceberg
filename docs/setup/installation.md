---
title: Instalação
---

## Clonar o repositório

```bash
git clone https://github.com/sparke-Delta-Iceberg/spark-delta-iceberg.git
cd spark-delta-iceberg
```

## Instalar o uv (WSL Ubuntu/Debian)

Caso não tenha o `uv` instalado no WSL (Ubuntu/Debian), siga:

```bash
sudo apt update && sudo apt install -y curl ca-certificates
curl -LsSf https://astral.sh/uv/install.sh | sh
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
uv --version
```

## Preparar ambiente Python com uv

```bash
uv sync
```
