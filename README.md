# 🚀 IMPLEMENTACIÓN DE UN SISTEMA DE INFORMACIÓN PARA EL RESTAURANTE MARY

Este proyecto consiste en el desarrollo de un **sistema de información web** para el Restaurante Mary, cuyo objetivo es **automatizar procesos que anteriormente se gestionaban de forma manual**. Actualmente, el restaurante enfrenta problemas en el manejo de pedidos y en la organización de información de sus clientes y servicios. Con este sistema, buscamos **optimizar la gestión de pedidos, mejorar la atención al cliente y brindar mayor control administrativo**.

---

## ✅ Tecnologías Utilizadas

- **Backend:**
  - Java 17
  - Spring Boot
  - Spring Security
  - Maven
  - MySQL

- **Frontend:**
  - Angular 20
  - Tailwind CSS

---

## 📦 Requisitos Previos

Para correr el proyecto localmente, necesitas tener instalado:

- **Java 17**
- **Node.js** (para Angular)
- **Bun** (si estás usando Bun en lugar de npm)
- **MySQL Server**
- **Maven** (para compilar el backend)

---

## ⚙️ Instalación del Proyecto

### 1. Clonar el repositorio

```bash
git clone git@github.com:1832Code/SISTEMA_RM.git
```



```bash
CREATE DATABASE restaurante_mary;
```
3. Configuración y Ejecución del Backend
3.1 Configurar application.properties
Dentro de la carpeta del backend:

```bash
backend/src/main/resources/application.properties
```
Coloca tus credenciales de MySQL y configuración del servidor. Ejemplo:

````bash
spring.datasource.url=jdbc:mysql://localhost:3306/restaurante_mary
spring.datasource.username=root
spring.datasource.password=tu_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect

server.port=8080
````
### /*Explicación breve de cada propiedad:*/

- spring.datasource.url: URL de conexión a MySQL.
- spring.datasource.username: usuario de MySQL.
- spring.datasource.password: contraseña de MySQL.
- spring.jpa.hibernate.ddl-auto: permite crear/actualizar tablas automáticamente.
- spring.jpa.show-sql: muestra en consola las queries ejecutadas.
- spring.jpa.properties.hibernate.dialect: dialecto SQL usado por Hibernate.
- server.port: puerto donde correrá el backend.
### 3.2 Construir y Ejecutar el Backend
-- Desde la carpeta raíz del proyecto, ingresa al directorio del backend:


```bash
cd backend
```
Instala las dependencias y construye el proyecto:

```bash
mvn clean install
```
Para correr el backend:

```bash
mvn spring-boot:run
```
✅ Esto levantará el servidor Spring Boot en:

```bash
http://localhost:8080
```
4. Configuración y Ejecución del Frontend
4.1 Ir al directorio del frontend
Si estabas en el backend, regresa a la raíz del proyecto:


#### Frontend

```bash
cd admin
```
4.2 Instalar dependencias del frontend
Si utilizas Bun:

```bash
bun install
```
Si utilizas npm:

```bash
npm install
```

4.4 Levantar el frontend
Si usas Bun:

```bash
bun run start
```
Si usas npm:

```bash
npm run start
```
✅ Esto levantará el frontend en:

```bash
http://localhost:4200
```
✅ Qué Funcionalidades a implementar
Con este sistema podrás:

Registrar pedidos de los clientes.
Consultar y gestionar pedidos existentes.
Administrar menús y productos.
Gestionar usuarios y roles mediante Spring Security.
Disfrutar de una interfaz moderna y responsiva gracias a Angular y Tailwind CSS.
   
📄 Licencia
Este proyecto está bajo la licencia MIT.
✨ Autor
Students de la UTP
Ingeniero de Sistemas e Informática
markdown
> 
