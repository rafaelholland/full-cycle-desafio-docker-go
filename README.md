## Rodando o projeto

Após clonar o projeto, navegue pelo terminal até a pasta com o arquivo Dockerfile e faça o `build` da imagem

```bash
docker build -t fullcycle-go . -f Dockerfile
```

Em seguida, rode o container com a imagem que acabou de criar

```bash
docker run --name fullcycle-go -v $(pwd):/src fullcycle-go:latest
```

Você deve receber a mensagem `Full Cycle Rocks!!` em seu terminal

## Usando a imagem no dockerhub

Para usar a imagem hospedada no dockerhub, basta usar o seguinte comando:

```bash
docker run hollandr/fullcycle-go:latest
```

Você deve receber a mensagem `Full Cycle Rocks!!` em seu terminal
