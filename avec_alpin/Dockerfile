#telechargement de l'image docker de base
FROM openjdk:8-jdk-alpine

#tag du createur (optionnel)
MAINTAINER aziz.aoues@gmail.com

#exposition du port utilisée par l'application
EXPOSE 8080

#copie du jar de l'application dans le conteneur
ADD ./application/hello-world-0.1.0.jar /data/hello-world-0.1.0.jar

#commande executée au lancement (demarage de l'application)
ENTRYPOINT ["java","-jar","/data/hello-world-0.1.0.jar"]
#CMD java -jar /data/hello-world-0.1.0.jar
