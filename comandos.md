### Terminal
#### - Ver se quais containers estão em execução

###### nova

``` docker container ls ```

###### velha

``` docker ps```

#### - Executar container

``` docker container run -t <nome da imagem docker>```

#### - Executar container com terminal interativo

``` docker container run -ti <nome da imagem docker>```

#### - Mostra todos os containers que já foram executados na máquina

``` docker container ls -a```

#### Conectar ao container que você saiu sem matá-lo

``` docker container attach <containerID ou NAME do container>```

Faz rodar o container em primeiro plano não serve para servidor web

#### Se precisar usar um servidor web como Apache ou Nginx ao invés do terminal interativo usar o deamon

``` docker container run -d <nome da imagem docker>```

e para conectar ao container que saiu sem matá-lo 

``` docker container exec -ti <nome da imagem docker> <comando>```

#### Pausar container 

``` docker container pause <containerID>```

#### Despausar container 

``` docker container unpause <containerID>```

#### Parar container 

``` docker container stop <containerID>```

#### iniciar container 

``` docker container start <containerID>```

#### reiniciar container 

``` docker container restart <containerID>```
#### Ver todas as informações do container 

``` docker container inspect <containerID>```

#### Ver logs do container 

``` docker container logs -f <containerID>```

#### Remover container 

``` docker container rm -f <containerID>```

#### Ver informações de consumo do container (cpu, memoria, rede e blocos)

``` docker container stats <containerID>```

#### Mostra processos que estão sendo executados no container  

``` docker container top <containerID>```

#### Adcinionar maximo de memoria que o container pode consumir

``` docker container run -d -m <memoria>M <nome do container sendo criado>```

#### Adicinionar maximo de cpu (em core) que o container pode consumir

``` docker container run -d --cpus <numero> <nome do container sendo criado>```
``` docker container update --cpus <numero> <containerID>```

#### Criar imagem com Dockerfile
Dentro da pasta onde fica o dockerfile
``` docker image build -t <nome da imagem>:<numero da versao> .```

#### listar imagens que estão no host
Dentro da pasta onde fica o dockerfile
``` docker image ls```
``` docker images```

### Teclado 

#### sair do container sem matá-lo

crtl + p + q

### Conteúdo

### Rodar como deamon 

Não rodar em primeiro plano, não tem interatividade apenas executa a aplicação.







