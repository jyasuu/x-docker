FROM alpine

RUN apk update && apk add openssh-server && ssh-keygen -A

EXPOSE 22

CMD ["/usr/sbin/sshd", "-D"]

