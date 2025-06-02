# Task Manager – Módulo Principal (Spring Boot)

Este es el módulo central del proyecto **Task Manager**, desarrollado con Spring Boot. Se encarga de coordinar la lógica principal, exponer APIs REST, y utilizar los módulos de estructuras y persistencia como dependencias.

## 📈 Funcionalidades principales

* Exponer APIs REST para:

  * Crear, listar y eliminar tareas
  * Gestionar el historial de tareas
  * Operaciones con estructuras: pila, cola, cola con prioridad, árbol de subtareas
* Uso de anotaciones `@RestController`, `@Service` y `@Autowired`
* Documentación de endpoints con Swagger UI
* Persistencia con JPA y base de datos MariaDB

## ✨ Tecnologías

* Java 22
* Spring Boot 3.5.0
* Maven
* MariaDB
* Swagger UI (OpenAPI 3)

---

## 🌍 Documentación Swagger

Una vez iniciada la aplicación, accede a:

```
http://localhost:8080/swagger-ui/index.html
```

Desde ahí podés probar todos los endpoints de forma visual.

---

## ⚙️ Configuración de la Base de Datos

En el archivo `application.properties`:

```properties
spring.datasource.url=jdbc:mariadb://localhost:3306/task_manager_db
spring.datasource.username=root
spring.datasource.password=

spring.datasource.driver-class-name=org.mariadb.jdbc.Driver
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MariaDBDialect

server.port=8080
```

---

## 📊 Dependencias internas

Este módulo depende de los otros dos:

### task-manager-structures

```xml
<dependency>
    <groupId>umg.edu.gt</groupId>
    <artifactId>task-manager-structures</artifactId>
    <version>1.0.0</version>
</dependency>
```

### task-manager-persistence

```xml
<dependency>
    <groupId>umg.edu.gt</groupId>
    <artifactId>task-manager-persistence</artifactId>
    <version>1.0.0</version>
</dependency>
```

---

## 🚀 Ejecución

1. Clonar el repositorio
2. Configurar la base de datos `task_manager_db` en XAMPP o similar
3. Ejecutar `TaskManagerSpringbootApplication.java`
4. Acceder a Swagger: [http://localhost:8080/swagger-ui/index.html](http://localhost:8080/swagger-ui/index.html)

---

## 📖 Estructura del paquete principal

```
umg.edu.gt.taskmanagerspringboot
├── controller
├── service
├── model
├── config
└── TaskManagerSpringbootApplication.java
```

---

## 🎓 Autor

Carlos Valiente - Proyecto final UMG 2025
