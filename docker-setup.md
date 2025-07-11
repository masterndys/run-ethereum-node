📄 `docs/docker-setup.md`
```md
# Run Geth with Docker

```bash
docker run -d --name eth-node \
  -v $HOME/.ethereum:/root/.ethereum \
  -p 8545:8545 \
  ethereum/client-go --http --http.addr "0.0.0.0"
