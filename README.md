# Pueba Avanzada 2025

Este proyecto es una aplicación de ejemplo creada con **Java 21** y **Spring Boot 3**. Incluye configuración para conectarse a **MySQL** y utiliza **Lombok** para reducir el código ceremonial en las entidades.

## Requisitos

- Java 21
- Maven 3.9+
- MySQL 8 (o compatible)

## Configuración

Actualiza las credenciales de la base de datos en `src/main/resources/application.properties` con tu usuario y contraseña. Por ejemplo:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/pueba_avanzada_2025
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña
```

## Ejecución

Compila y ejecuta la aplicación con:

```bash
mvn spring-boot:run
```

Si prefieres usar el wrapper de Maven, puedes generarlo ejecutando una vez `mvn -N io.takari:maven:wrapper` y luego utilizar `./mvnw` en lugar de `mvn`.

La API expone un endpoint REST de ejemplo en `GET /api/users` para listar usuarios almacenados en la base de datos.
