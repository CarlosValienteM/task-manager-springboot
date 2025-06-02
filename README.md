# Task Manager – Módulo Principal (Spring Boot)

Este módulo representa la lógica principal del sistema **Task Manager**, integrando las estructuras personalizadas y el acceso a la base de datos mediante JPA. Además, expone toda la funcionalidad mediante **APIs REST** documentadas con Swagger.

---

## 🚀 Funcionalidad Principal

### 1️⃣ Árbol de Subtareas
- Crear nodo raíz
- Agregar subtareas
- Consultar nodo por ID
- Consultar todos los nodos

### 2️⃣ Pila de tareas (Stack)
- Agregar (`push`)
- Eliminar (`pop`)
- Ver el tope (`peek`)
- Ver si está vacía (`isEmpty`)
- Ver tamaño (`size`)

### 3️⃣ Cola de tareas (Queue)
- Encolar (`enqueue`)
- Desencolar (`dequeue`)
- Ver al frente (`peek`)
- Vacía / llena
- Ver tamaño

### 4️⃣ Cola con Prioridad
- Encolar valor con prioridad
- Desencolar valor más prioritario
- Ver todos los elementos

### 5️⃣ Gestión de Tareas y Usuarios (JPA)
- Crear, consultar, eliminar tareas
- Asociar tareas a usuarios
- Registrar historial de tareas

---

## 🛠️ Tecnologías

- Java 22
- Spring Boot 3.5.0
- Spring Data JPA
- Maven
- Swagger (OpenAPI)
- MariaDB
- RabbitMQ (opcional)

---

## 📦 Estructura del Proyecto

```text
umg.edu.gt.taskmanagerspringboot
├── controller
│   ├── StackController.java
│   ├── QueueController.java
│   ├── PriorityQueueController.java
│   ├── SubtaskTreeController.java
│   ├── TaskController.java
│   └── TaskHistoryController.java
├── service
│   ├── StackService.java
│   ├── QueueService.java
│   ├── PriorityQueueService.java
│   ├── SubtaskTreeService.java
│   ├── TaskManagerService.java
│   └── TaskHistoryService.java


