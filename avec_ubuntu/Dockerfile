
# Pull base image.
FROM ubuntu

#tag du createur (optionnel)
MAINTAINER aziz.aoues@gmail.com

# Install Java.
RUN \
  apt-get update && \
  apt-get install -y oracle-java8-installer && \
  rm -rf /var/lib/apt/lists/* && \
  rm -rf /var/cache/oracle-jdk8-installer


# Define working directory.

# Define commonly used JAVA_HOME variable
#ENV JAVA_HOME /usr/lib/jvm/java-8-oracle

#exposition du port utilisée par l'application
EXPOSE 8080

#copie du jar de l'application dans le conteneur
ADD ./application/hello-world-0.1.0.jar /data/hello-world-0.1.0.jar

#commande executée au lancement (demarage de l'application)
ENTRYPOINT ["java","-jar","/data/hello-world-0.1.0.jar"]
#CMD java -jar /data/hello-world-0.1.0.jar
