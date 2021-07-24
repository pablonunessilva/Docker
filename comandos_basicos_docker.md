# Docker

## Comandos 
### docker run
- Executa um container 
- "-p" e a porta
- "--link" o link do containet
- "-e" seta a(s) variavel(is) de ambiente
- "-d" joga para segundo plano
### Ex:
```shel
    docker run -p 3000:3000 --link mongodb -e MONGO_URL=mongodb api-exemplo
````

### docker build
- "-t"

### docker ps
- lista os containers
- "-a" lista todos os container, inclusive em segundo plano

### docker status
- informar o id ou apleido

### docker inspect (id da imagem ou container)
- inpessiona uma imagem do docker

### docker rmi (nome da imagem)
- Remove uma imagem local

### docker exec (id_container ou nome_container) 
- "-i" permite interagir com o container
- "-t" associa o seu terminal ao terminal do container
- "-it" é apenas uma forma reduzida de escrever '-i' '-t'
- "--name" algum-nome permite atribuir um nome ao container em execução
- "-p" 8080:80 mapeia a porta 80 do container para a porta 8080 do host
- "-d" executa o container em background
- "-v" /pasta/host:/pasta/container cria um volume '/pasta/container' dentro do container com o conteúdo da pasta '/pasta/host' do host
### docker attach (id_container ou nome_container)
- acesso diretorio dentro do container
- para sair sem para o container pode usar o ctrl+q ou ctrl+p
### docker start (id do container)
- Inicia um container
### Docker stop(id do container)
- Para um container

### docker images
- listas as imagens
### docker search 
- procura uma imagem
### docker pull 
- baixa essa imagem
### docker commit
- Para commitar uma alteração no container

## Comandos úteis
### docker rm $(docker ps -qa)
### docker rmi $(docker images -q)

