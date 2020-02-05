# Code Education - desafio 7 (FINAL) - Deploy Contínuo


Deploy automático da aplicação já desenvolvida em Go Lang nas fases passadas.

As regras do processo são:
- Quando qualquer push ou uma PR for relizada no Github em um branch diferente do Master, o processo de CI é executado.
- Quando um merge ou um push entrarem no branch Master, o processo de CI/CD é chamado, fazendo assim o deploy de forma automática no Kubernetes.


### Imagem no Docker Hub:

[https://hub.docker.com/repository/docker/pauloandresoares/go-final](https://hub.docker.com/repository/docker/pauloandresoares/go-final)

Executando container localmente para testes:
```
docker run --name go-final -p 8000:80 --rm pauloandresoares/go-final
```

Verificar aplicação no ambiente local:

**[http://localhost:8000](http://localhost:8000)**

### CI no Cloud Build:
![CI](/desafio-final-ci.png)

### CI e CD no Cloud Build:
![CI](/desafio-final-ci-cd.png)



