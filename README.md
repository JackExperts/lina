# Baixando o código

1. **Clone o repositório Lina v3.10.7 para o diretório /opt/:**

    ```bash
    cd /opt/
    git clone https://github.com/JackExperts/lina.git
    ```

2. **Instalando Node.js:**

    ```bash
    cd /opt
    wget https://nodejs.org/download/release/v16.14.0/node-v16.14.0-linux-x64.tar.xz
    tar -xf node-v16.14.0-linux-x64.tar.xz
    mv node-v16.14.0-linux-x64 /usr/local/node
    chown -R root:root /usr/local/node
    export PATH=/usr/local/node/bin:$PATH
    echo 'export PATH=/usr/local/node/bin:$PATH' >> ~/.bashrc
    ```

3. **Instalando dependências:**

    ```bash
    cd /opt/lina
    npm install -g yarn
    yarn install
    ```

4. **Iniciando o sistema:**

    ```bash
    npm run dev
    ```

