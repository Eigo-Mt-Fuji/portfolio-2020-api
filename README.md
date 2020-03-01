# README

```
git clone git@github.com:Eigo-Mt-Fuji/portfolio-2020-api.git portfolio-2020-api
cd portfolio-2020-api
mix deps.get
iex -S mix
mix ecto.migrate
```

## Gigalixir 


### Setup (Install / Login / CreateApp)

* Install

```
sudo pip3 install gigalixir --ignore-installed six
```

* Login / Create App (the name will be assigned to APP_NAME)

```bash
gigalixir login
export APP_NAME=$(gigalixir create)
gigalixir pg:create -a $APP_NAME --free
```

### Continue (Install / Login / CreateApp)

```bash
export APP_NAME=grouchy-crowded-asianelephant
```

* Set Configrations

```bash
gigalixir config:set -a $APP_NAME APP_NAME=$APP_NAME
gigalixir config:set -a $APP_NAME POOL_SIZE=2 # gigalixir free only allow 2 db connections at the same time.
gigalixir config:set -a $APP_NAME PORT=4000
gigalixir config:set -a $APP_NAME SECRET_KEY_BASE=$(mix phx.gen.secret)
```

* Setup Gigalixir Git Remote 

```bash
cat ~/.netrc # check and copy `machine git.gigalixir.com`'s password.
git remote add gigalixir https://efg.river%40gmail.com:be1b4906-3af2-4eee-8b3c-95e28a730336@git.gigalixir.com/$APP_NAME.git
git fetch gigalixir
```

* Push Source

```
git add .
git commit -m "Update sources."
git push gigalixir master
```

* Run Db Migration (Check Logs After Migration Finished)

```
gigalixir run mix ecto.migrate # migration
gigalixir logs 
```

* Open Browser

```
gigalixir open
```

* Check Process Status

```
gigalixir ps
```

