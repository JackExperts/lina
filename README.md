# Lina

Lina é o projeto de interface de usuário (UI) frontend do JumpServer, desenvolvido principalmente utilizando [Vue](https://cn.vuejs.org/) e [Element UI](https://element.eleme.cn/). O nome é inspirado na heroína do Dota [Lina](https://baike.baidu.com/item/%E8%8E%89%E5%A8%9C/16693979).

## Execução do Desenvolvimento

```
0. Pré-requisito: Certifique-se de ter o servidor JumpServer API em execução.

1. Instale as dependências
$ yarn install

2. Modifique .env.development VUE_APP_CORE_HOST
# ...
VUE_APP_CORE_HOST = 'JUMPSERVER_APIHOST'

3. Execute
$ yarn serve

4. Construa
$ yarn build:prod
```

## Implantação em Produção
Baixe o arquivo RELEASE, coloque-o em um diretório apropriado e modifique o arquivo de configuração nginx da seguinte maneira:
```
server {
  listen 80;

  location /ui/ {
    try_files $uri / /ui/index.html;
    alias /opt/lina/;
  }

  location / {
    rewrite ^/(.*)$ /ui/$1 last;
  }
}
```

## Agradecimentos
- [Vue](https://cn.vuejs.org) - Framework frontend
- [Element UI](https://element.eleme.cn/) - Biblioteca de componentes de UI do Eleme
- [Vue-element-admin](https://github.com/PanJiaChen/vue-element-admin) - Esqueleto do projeto

## Licença e Direitos Autorais
Mantenha a consistência com [jumpserver](https://github.com/jumpserver/jumpserver)
