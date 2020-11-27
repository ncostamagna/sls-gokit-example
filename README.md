# sls-gokit-example

## Instalacion
```sh
serverless create -t aws-go-dep -p myservice

npm i serverless serverless-offline
```

## Correr local

```sh
# Build del proyecto
make build

sls invoke local -f schedule
sls invoke local -f schedule -d '{"body":"{\"start_date\":\"\"}"}'
```

## Configurar credenciales
```sh
sls config credentials --provider aws --key {key} --secret {secret}
```
Sino podemos configurarlo manualmente agregando los valores en .aws/credentials
```sh
sls deploy
```