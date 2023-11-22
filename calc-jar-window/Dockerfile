FROM ubuntu

RUN apt-get update && apt-get install -y x11-apps xauth openjdk-11-jre && rm -rf /var/lib/apt/lists/*

COPY calc.jar /program/

ENV DISPLAY=:0

CMD [ "java", "-jar", "/program/calc.jar" ]