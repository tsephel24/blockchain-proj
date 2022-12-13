## Build an Image ##

```docker build --tag nci02 .```


## Run an image ##

```docker run --name ncilab02 -p 8090:8080 nci02```

## Run the curl command ##

This transfers ETH:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"0x9D0C4a72012A128aB437fAa1A9b09729e7B7DA5e", "amount":"0.01"}' http://localhost:8090/eth```

This transfers token:

```curl --header "Content-Type: application/json" --request POST --data '{"address":"0x9D0C4a72012A128aB437fAa1A9b09729e7B7DA5e"}' http://localhost:8090/token```

