# 🚀 API Hola Mundo - Spring Boot

Proyecto desarrollado como parte de la actividad individual:  
Implementar un endpoint tipo **GET** que muestre un **"Hola Mundo!"** utilizando el framework Spring Boot.

---

## 📌 Información del Proyecto

- 👤 **Nombre:*Deybi Samuel Payco Huamani*   
- 🆔 **Repositorio:*ase251s3_DeybiPayco_be *  
- 📚 **Asignatura:*TSW*   
- 🏫 **Institución:*valle grande * 

---

## 🎯 Objetivo

Desarrollar un servicio REST con un endpoint GET que retorne el mensaje:

```text
Hola Mundo!
```

---

## 🛠️ Tecnologías Utilizadas

- ☕ Java 17  
- 🌱 Spring Boot  
- 📦 Maven  
- 🧪 Postman  

---

## ⚙️ Pasos para la Implementación

### 1️⃣ Crear el proyecto

Se creó el proyecto desde **Spring Initializr** con las siguientes configuraciones:

- **Project:** Maven  
- **Language:** Java  
- **Spring Boot:** Última versión estable  
- **Group:** com.DeybiPayco  
- **Artifact:** holamundo  
- **Packaging:** Jar  
- **Java:** 17  
- **Dependencies:**
  - Spring Web  

---

### 2️⃣ Crear el controlador

Se creó la clase `HolaMundoController` dentro del paquete `controller`:

```java
package com.tunombre.holamundo.controller;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class HolaMundoController {

    @GetMapping("/hola")
    public String holaMundo() {
        return "Hola Mundo!";
    }
}
```

---

### 3️⃣ Ejecutar la aplicación

Desde la terminal:

```bash
mvn spring-boot:run
```

O ejecutando la clase principal del proyecto.

---

### 4️⃣ Probar el endpoint

Abrir el navegador o Postman y acceder a:

```text
http://localhost:8080/hola
```

Resultado esperado:

```text
Hola Mundo!
```

---

## 📂 Estructura del Proyecto

```text
holamundo
│── src
│   └── main
│       ├── java
│       │   └── com.tunombre.holamundo
│       │       ├── HolamundoApplication.java
│       │       └── controller
│       │           └── HolaMundoController.java
│       └── resources
│           └── application.properties
└── pom.xml
```

---

