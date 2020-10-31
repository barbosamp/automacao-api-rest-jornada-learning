#imagem que será utilizada, é o nosso ponto de partida :)
FROM python:3

LABEL maintainer="contato@etech.dev"

#Copia os arquivos locais para dentro da imagem
COPY . /ServeRest-APITesting-Python

#Indica onde será o repositório de trabalho
WORKDIR /ServeRest-APITesting-Python

#Comando que é executado na imagem acima, ou seja, 
# após criar a imagem o docker realizará os downloads a seguir:
RUN pip install -r requirements.txt

RUN cd Tests

RUN pytest
