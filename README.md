# Baixando o código

1. **Clone o repositório Lina v3.10.7 para o diretório /opt/:**

    ```bash
    cd /opt/
    git clone https://github.com/joaofaria/lina-v3.10.7.git
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
    cd /opt/lina-v3.10.9
    npm install -g yarn
    yarn install
    ```

4. **Configurando variáveis de ambiente:**

    - Edite o arquivo `.env.development` e cole o conteúdo abaixo:

        ```plaintext
        # Global environment variables, do not modify casually
        ENV = 'development'

        # base api
        VUE_APP_BASE_API = ''
        VUE_APP_PUBLIC_PATH = '/ui/'

        # vue-cli uses the VUE_CLI_BABEL_TRANSPILE_MODULES environment variable,
        # to control whether the babel-plugin-dynamic-import-node plugin is enabled.
        # It only does one thing by converting all import() to require().
        # This configuration can significantly increase the speed of hot updates,
        # when you have a large number of pages.
        # Detail:  https://github.com/vuejs/vue-cli/blob/dev/packages/@vue/babel-preset-app/index.js

        VUE_CLI_BABEL_TRANSPILE_MODULES = true

        # External auth
        VUE_APP_LOGIN_PATH = '/core/auth/login/'
        VUE_APP_LOGOUT_PATH = '/core/auth/logout/'

        # Dev server for core proxy
        VUE_APP_CORE_HOST = 'http://localhost:8080'
        VUE_APP_CORE_WS = 'ws://localhost:8080'
        VUE_APP_KAEL_HOST = 'http://localhost:8083'
        VUE_APP_ENV = 'development'
        ```

5. **Iniciando o sistema:**

    ```bash
    npm run dev
    ```

