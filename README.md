# README

```
git clone git@github.com:Eigo-Mt-Fuji/portfolio-2020-api.git portfolio-2020-api
cd portfolio-2020-api
mix deps.get
iex -S mix
mix ecto.migrate
```

## Gigalixir 

* Install

```
sudo pip install gigalixir --ignore-installed six
```

* Login

```
gigalixir login
```

* Create App (the name will be assigned to APP_NAME)

```
export APP_NAME=$(gigalixir create)
```

* Create Postgres Database On Gigalixir

```
gigalixir pg:create --free
```

* Set Configrations

```
gigalixir config:set APP_NAME=$APP_NAME
gigalixir config:set POOL_SIZE=2 # gigalixir free only allow 2 db connections at the same time.
gigalixir config:set PORT=4000
gigalixir config:set SECRET_KEY_BASE=$(mix phx.gen.secret)
```

* Setup Gigalixir Git Remote 

```
cat ~/.netrc
git remote add gigalixir https://<Mail Address>:<Password>@git.gigalixir.com/$APP_NAME.git # e.g. https://efg.river%40gmail.com:be1b4906-xxxx-4xxx-xxxx-xxxx@git.gigalixir.com/grouchy-crowded-asianelephant.git
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
