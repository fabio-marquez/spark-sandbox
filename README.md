# spark-sandbox

Guia de instalação do spark:

## 1) Atualizar o java

`sudo apt update`
`sudo apt install openjdk-11-jdk -y`

Verificar com: `java -version`


## 2) Instalar o spark

- Download: `wget https://dlcdn.apache.org/spark/spark-3.5.5/spark-3.5.5-bin-hadoop3.tgz`
- Exportar:
    `tar xvf spark-3.5.5-bin-hadoop3.tgz`

    `sudo mv spark-3.5.5-bin-hadoop3 /opt/spark`

OBS: Caso for necessária outra versão, pegar o link correto correspondente


## 3) Definir variáveis de ambiente

`export SPARK_HOME=/opt/spark`

`export PATH=$PATH:$SPARK_HOME/bin:$SPARK_HOME/sbin`

`export JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64`

Aplicar as alterações: `source ~/.bashrc`

## 4) Verificar a instalação

`spark-shell`