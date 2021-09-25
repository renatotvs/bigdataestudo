
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

Mover diretório:
- mv nifi-1.14.0 /opt/ - > mv nifi-1.14.0 /tmp
- ln -s /tmp/nifi-1.9.2/ /tmp/nifi
- cd /tmp/nifi

Instalar serviço
- bin/nifi.sh instal

Output: Service nifi installed

Iniciar o serviço do nifi:
- /etc/init.d/nifi start ou nifi/nifi.sh start

Abrir o navegador e testar o endereço web:
- localhost:8443/nifi

Tela inicial do Nifi:

![image](https://user-images.githubusercontent.com/42357180/134785564-f19b49a0-8f8f-4c85-9005-e9e6f05a0af4.png)
