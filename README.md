### Rdkit wasm


#### create docker image
```shell
docker build --platform linux/amd64 -t IMAGE_NAME/TAG_NAME ./

```

#### connect to created image - container
```shell
docker exec -it CONTAINER_ID /bin/sh
```

#### comfile in container
```shell
make -j2 RDKit_minimal && \
  cp Code/MinimalLib/RDKit_minimal.* ../Code/MinimalLib/demo/
```


#### Test in local

test in demo.html
change container Id in sh file.
```shell
./getWasmFile.sh
cd demo
```


