
```sh
docker buildx build . -t jyasu/openssh-server:latest

docker run -d --name ssh-server -p 22 jyasu/openssh-server

cat ~/.ssh/id_rsa.pub | docker exec -i ssh-server /bin/sh -c "cat >> /root/.ssh/authorized_keys"

```