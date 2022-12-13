## Build an Image ##

```docker build --tag tenzin-blockchain .```


## Run an image ##

```docker run --name nci20212sem1-main -p 8090:8080 tenzin-blockchain```

## Run the curl command ##

This transfers ETH:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"0x9D0C4a72012A128aB437fAa1A9b09729e7B7DA5e", "amount":"0.01"}' http://localhost:8090/eth```

This transfers token:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"0x9D0C4a72012A128aB437fAa1A9b09729e7B7DA5e"}' http://localhost:8090/token```
