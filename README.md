IPB Pedro Nunes
---------------

Esse é um site estático feito com `jekyll`.


### Instale as dependências

Também conhecidas como ruby `gems`. Antes você precisa instalar a gem `bundler` para gerenciar as dependências com esse comando:

```
gem install bundler
```

E para instalar as dependências:

```
bundle install
```

### Servindo o site localmente

```
bundle exec jekyll serve --watch
```

### Deploy

Para fazer deploy (mandar suas modificações para servidor do gitlab que é onde o site está hospedado), você precisa commitar as alterações usando esses comandos (por exemplo) depois de fazer as alterações e conferir elas localmente:

```
git add .
git commit -m "Add post"
git push origin master
```

Depois disso o gitlab vai fazer o build to site (ele vai executar algo como `bundle exec jekyll build` além de outros comandos para servir o site com `https`), dá para acompanhar indo na página do projeto no gitlab e clicar nos menus `CI/CD > Jobs`.

Depois que o build terminar o site vai estar no ar e você pode verificar no [ipbpedronunes.org](https://ipbpedronunes.org).




