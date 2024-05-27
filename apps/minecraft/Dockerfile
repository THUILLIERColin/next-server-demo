# find the latest minecraft-server.jar file from https://www.minecraft.net/en-us/download/server
FROM ubuntu

RUN apt-get update && apt-get install -y openjdk-8-jre-headless wget

WORKDIR /minecraft

RUN wget https://launcher.mojang.com/v1/objects/35139deedbd5182953cf1caa23835da59ca3d7cd/server.jar

RUN echo "eula=true" > eula.txt

CMD ["java", "-Xmx1024M", "-Xms1024M", "-jar", "server.jar", "nogui"]