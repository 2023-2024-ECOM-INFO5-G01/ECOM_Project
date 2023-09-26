# Personal computer install

## Java / Openjdk (17.0.6)

Installer OpenJDK
```
sudo apt-get install openjdk-17-jdk
sudo apt-get install openjdk-17-jre
```

Vérification avec 
```
java -version
```

## Docker (24.0.6)

Vérification avec 
```
docker -v
```

## IDE Eclipse (Java) & VSC (autre)

## JHipster

Conteneur Docker

## Maven (3.9.4)

Pour avoir la dernière version stable de Maven (3.9.4), il faut récupérer l'archive via : 
```
wget https://archive.apache.org/dist/maven/maven-3/3.9.4/binaries/apache-maven-3.9.4-bin.tar.gz
```

Décompresser l'archive
```
tar -zxvf apache-maven-3.9.4-bin.tar.gz
```

Déplacer Maven vers le répertoire d'installation
```
sudo mv apache-maven-3.9.4 /opt
```

Configurer les variables d'environnement pour pouvoir utiliser Maven de partout sur le système
```
export M2_HOME=/opt/apache-maven-3.9.4
export M2=$M2_HOME/bin
export PATH=$M2:$PATH
```

Vérifier la version
```
mvn -v
```

# Config Azure VM

Série de screen de la config de notre VM
![Screen config 1](https://cdn.discordapp.com/attachments/1156120927466172426/1156120943719096380/image.png?ex=6513d108&is=65127f88&hm=e890c3c6c3543de6e03c77e60ee983563db820221ba414d5f406c5a940b53fba&)
![Screen config 2](https://cdn.discordapp.com/attachments/1156120927466172426/1156120985624387644/image.png?ex=6513d112&is=65127f92&hm=172c0444255d44000b0a2a70ea72342322d0df5ffa493681e43f126a6f5286f7&)
![Screen config 3](https://cdn.discordapp.com/attachments/1156120927466172426/1156121029798793266/image.png?ex=6513d11d&is=65127f9d&hm=dc1315d606f2d5cd882b7bb4501fe5faa7fda56c856d42a9787f143c04a647b2&)
![Screen config 4](https://cdn.discordapp.com/attachments/1156120927466172426/1156121062065586247/image.png?ex=6513d124&is=65127fa4&hm=643854f031b53634ef66292d50ce796929430507a92a2099774b19773b9c1b22&)

Voici un screen du firewall de notre VM
![Firewall VM](https://cdn.discordapp.com/attachments/1156120927466172426/1156146622930100234/Capture_decran_du_2023-09-26_10-33-14.png?ex=6513e8f3&is=65129773&hm=646eaffe09d933d9ce5abcd4f816c01db88813f2fa78a06e3991bc82646e5f91&)

# Install in Azure VM 

Avant d'installer quelque chose, mettez à jour votre système pour vous assurer que vous disposez des dernières mises à jour de sécurité.

```
sudo apt update  
sudo apt upgrade -y
```

## Docker

Installez Docker
```
sudo apt install docker.io
```

Démarrer et activer Docker
```
sudo systemctl start docker
sudo systemctl enable docker
```

Vérifiez l'installation de Docker
```
docker --version
```

## Docker compose

Téléchargez Docker Compose
```
sudo curl -L "https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```

Donnez les droits d'exécution
```
sudo chmod +x /usr/local/bin/docker-compose
```

Vérifiez l'installation de Docker Compose
```
docker-compose --version
```

## OpenJDK

Installer OpenJDK
```
sudo apt install openjdk-17-jdk
```

Vérifier l'installation
```
java -version
```



