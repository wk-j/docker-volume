## Volume

```bash
mkdir -p datas/xyz

docker volume create --driver local --opt type=local --opt o=bind --opt device=./datas/xyz --name xyz
docker volume inspect xyz
docker volume inspect xyz   --format '{{ .Mountpoint }}'
```

## Start

```bash
docker-compose up
```

## Remove

```bash
docker volume rm xyz
```