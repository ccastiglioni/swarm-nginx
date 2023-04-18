# Swarm-nginx
criando swarm com nginx

- Iniciar o Swarm na Aplicação Docker

```sh
docker swarm init
```

- Subir serviços no Swarm

```sh
docker stack deploy -c docker-swarm.yml app
```

- Derrubar serviços no Swarm

```sh
docker stack rm app
```

- Ver serviços em execução

```sh
docker service ls
```

- Ver containers em execução

```sh
docker stats
```

- Entrar em um container:

```sh
# primeiro obtenha o id do container, pode ser via 'docker stats'
# com o id em mãos substitua '{id}' pelo id obtido
docker exec -it {id} bash
```



