FROM openjdk:23-jdk-slim
WORKDIR /app

RUN apt-get update && apt-get install -y findutils

COPY . .

#ARG JAR_FILE=build/libs/*.jar
#COPY ${JAR_FILE} app.jar

RUN chmod +x ./start-dev.sh
ENTRYPOINT ["sh","./start-dev.sh"]
