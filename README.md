Prova 1 de Computação em Nuvem
Nome: João Pedro Ramos Soares RA: a086e378f0dabc4351

##O que fiz
Executei uma página web em um contêiner Docker chamado atendimento. Usei a imagem nginx:alpine e a porta 8082 do ambiente.

##Verficação do contêiner
Cole aqui a saída do comando docker ps: CONTAINER ID   IMAGE          COMMAND                  CREATED        STATUS                  PORTS                                     NAMES
96b0362192a5   nginx:alpine   "/docker-entrypoint.…"   1 second ago   Up Less than a second   0.0.0.0:8082->80/tcp, [::]:8082->80/tcp   atendimento

##Teste da página
Cole aqui a resposta do comando curl http://localhost:8082: root@ubuntu:~$ curl http://localhost:8082

html lang="pt-BR">

<title>atendimento</title>
atendimento disponivel

##Explicação
Com minhas palavras, qual é a diferença entre a imagem nginx:alpine e o contêiner atendimento? Para que serviu o mapeamento 8082:80

A imagem ngix:alpine é uma imagem padrão usada como modelo e o contêiner atendimento é a instancia sendo executada

O mapeamento 8082:80 é 8082 sendo a porta do host(que no caso era meu notebook). Já a 80 é a porta do contêiner. Na pratica eu referencio a porta 8082 do meu notebook(localhost) para a porta 80 do contêiner.
