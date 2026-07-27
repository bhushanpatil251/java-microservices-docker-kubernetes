FROM eclipse-temurin:8-jre

COPY target/productcatalogue-0.0.1-SNAPSHOT.jar app.jar
COPY product-catalogue.yml product-catalogue.yml

EXPOSE 8020

ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar","server","/product-catalogue.yml"]
