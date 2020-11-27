# sls-gokit-example

```sh
serverless create -t aws-go-dep -p myservice

make build

npm i serverless serverless-offline

sls invoke local -f schedule

sls invoke local -f schedule -d '{"body":"{\"start_date\":\"\"}"}'
```