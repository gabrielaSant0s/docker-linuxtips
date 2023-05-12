#imagem baseada no debian 
FROM debian

#cria informação metadata
LABEL app="Giropops"
#variavel de ambiente
ENV  GABRIELA="DEV"

#executa um comando em tempo de build
RUN apt-get update && apt-get install -y stress && apt-get clean

#executa comandos no cmd
CMD stress --cpu 1 --vm-bytes 64M --vm 1