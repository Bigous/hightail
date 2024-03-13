FROM rust:latest

# Instalar ferramentas de desenvolvimento e utilitários
RUN apt-get update && apt-get install -y \
    git \
    build-essential \
    pkg-config \
    libssl-dev \
    cmake \
    curl \
    lldb \
    musl-tools \
    mingw-w64 \
    --no-install-recommends \
    && rm -rf /var/lib/apt/lists/*

# Configurações adicionais, se necessário

# Evita que o cargo crie arquivos como root, o que poderia impedir a limpeza do container.
# USER rust

# # Atualiza o cargo e instala as ferramentas necessárias
# RUN cargo install cargo-edit cargo-watch

# # Cria um diretório para o seu código
# WORKDIR /workspace