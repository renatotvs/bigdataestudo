
### Instalação Nifi no Linux Ubuntu

Passos:

- sudo apt-get update
- sudo apt-get install openjdk-8-jdk

Criar arquivo para adicionar configurações do java

- vi /etc/profile.d/java.sh
- export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64

Criar novo diretório para baixar o nifi:
- mkdir /downloads/apache-nifi -p
- cd /downloads/apache-nifi
- wget https://dlcdn.apache.org/nifi/1.14.0/nifi-1.14.0-bin.tar.gz

Descompactar arquivo:
- tar -zxvf nifi-1.14.0-bin.tar.gz

