# Projeto conversão de temperatura

### Sobre o projeto
O projeto conversão de temperatura é um projeto desenvolvido em NodeJS. O projeto tem como objetivo ser um exemplo para a criação de ambiente com containers usando NodeJS.

### Observações do projeto
A aplicação é exposta usando a porta 8080

### Comandos de Build
docker container build -t robertotrevisan/conversor-temperatura:latest -f Dockerfile_user .

### Build multistage
docker buildx create --use
docker buildx build --pull -t robertotrevisan/conversao-temperatura:v1 --platform=linux/amd64,linux/arm64 -f Dockerfile_user

