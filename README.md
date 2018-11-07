# YouDo Network

Seja bem-vindo(a) a rede social que conecta pessoas baseando-se em seus interesses!

Esse app eu uso para testar coisas novas do Ruby. Então espere por mudanças constantes por aqui. 😉

Aqui vão algumas capturas de tela do projeto...

Há um feed de atualizações das pessoas que você segue:
![Feed](docs/screenshots/feed.png)

Você também pode ver seu próprio perfil...
![Feed](docs/screenshots/user_profile.png)

E fazer uma nova publicação!
![Feed](docs/screenshots/new_post.png)

Pode também pesquisar por outros usuários e posts...
![Feed](docs/screenshots/search.png)

E visualizar e deixar comentários em publicações.
![Feed](docs/screenshots/view_post.png)


### Dependências

É necessário ter o Elasticsearch instalado, pois é usado o Searchkick para pesquisa por usuários e posts. Além disso, uma conta na Amazon AWS também é necessária, pois atualmente uso o S3 para upload de imagens

### Setup

```
$ bundle install
$ rails s
```

### Arquitetura

O YouDo em produção utiliza os serviços RDS (com o Postgres), S3 (para upload de imagens) e EC2 (para manter o projeto em execução). O Elasticsearch também é usado para pesquisa avançada por usuários e publicações.