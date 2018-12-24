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

Para fazer deploy (mandar suas modificações para servidor do github que é onde o site está hospedado), você precisa commitar as alterações usando esses comandos (por exemplo) depois de fazer as alterações e conferir elas localmente:

```
git add .
git commit -m "Add post"
git push origin master
```

Depois disso o github vai fazer o build to site (ele vai executar algo como `bundle exec jekyll build`). Não dá pra acompanhar, mas geralmente demora uns 2 minutos.

Depois que o build terminar o site vai estar no ar e você pode verificar no [ipbpedronunes.org](https://ipbpedronunes.org).

### GIT

Você pode testar e modificar à vontade, mas se você quiser voltar ao que estava antes das modificações você pode usar esse comando:

```
git checkout .
```

É sempre bom sempre depois de commitar você executar esse comando para puchar as modificações novas do servidor para a sua máquina:

```
git pull origin master
```

E depois você pode então executar

```
git push origin master
```

### Obrigado
