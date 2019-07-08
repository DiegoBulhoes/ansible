# Ansible

Container criado a parir da imgem do [docker-ssh-keygen](https://hub.docker.com/r/diegobulhoes/docker-ssh-keygen/) com o propósito de criar um container básico para praticar a utilização da ferramenta Ansible

```
docker run -d diegobulhoes/ansible
```

Você pode especificar a senha do root utilizando o argumento **PASSWORD_ROOT**, a do usuário app utilizando **PASSWORD_USER_SSH** e da frase de segurança referente a chave de segurança **NEW_PASSPHRASE**. Por padrão esses argumentos estão armazenando nos seguintes argumentos.

```
PASSWORD_ROOT='passwordRoot'
PASSWORD_USER_SSH='passwordUserSSH'
NEW_PASSPHRASE='newPassphrase'
```

O acesso root via utilizando a senha **bloqueado**

- O ssh esta configurado para buscar as chaves dos workers autorizados no seguinte caminho **.ssh/workers/AuthorizedKeysFile** e a chave do master **.ssh/master/AuthorizedKeysFile**
