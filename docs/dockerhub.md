# Uploading to Docker Hub

```bash
ETHEREUMETL_VERSION=1.6.5
docker build -t ethereum-etl:${ETHEREUMETL_VERSION} -f Dockerfile .
docker tag ethereum-etl:${ETHEREUMETL_VERSION} blockchainetl/ethereum-etl:${ETHEREUMETL_VERSION}
docker push blockchainetl/ethereum-etl:${ETHEREUMETL_VERSION}

docker tag ethereum-etl:${ETHEREUMETL_VERSION} blockchainetl/ethereum-etl:latest
docker push blockchainetl/ethereum-etl:latest
```