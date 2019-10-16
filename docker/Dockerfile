FROM java:8

# 将本地文件夹挂载到当前容器
VOLUME /tmp

ADD target/eureka-server-0.01-SNAPSHOT.jar /app.jar

RUN bash -c 'touch /app.jar'

EXPOSE 8761

ENTRYPOINT ["java", "-Djava.security.egd=file:J:\prj\eureka-server", "-jar", "/app.jar"]