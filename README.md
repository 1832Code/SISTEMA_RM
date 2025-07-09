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
git clone https://github.com/tu-usuario/tu-repo.git
cd tu-repo
```



```bash
CREATE DATABASE restaurante_mary;
3. Configuración y Ejecución del Backend
3.1 Configurar application.properties
Dentro de la carpeta del backend:

css
CopiarEditar
backend/src/main/resources/application.properties
Coloca tus credenciales de MySQL y configuración del servidor. Ejemplo:

properties
CopiarEditar
spring.datasource.url=jdbc:mysql://localhost:3306/restaurante_mary
spring.datasource.username=root
spring.datasource.password=tu_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect

server.port=8080
Explicación breve de cada propiedad:

spring.datasource.url: URL de conexión a MySQL.
spring.datasource.username: usuario de MySQL.
spring.datasource.password: contraseña de MySQL.
spring.jpa.hibernate.ddl-auto: permite crear/actualizar tablas automáticamente.
spring.jpa.show-sql: muestra en consola las queries ejecutadas.
spring.jpa.properties.hibernate.dialect: dialecto SQL usado por Hibernate.
server.port: puerto donde correrá el backend.
3.2 Construir y Ejecutar el Backend
Desde la carpeta raíz del proyecto, ingresa al directorio del backend:

bash
CopiarEditar
cd backend
Instala las dependencias y construye el proyecto:

bash
CopiarEditar
mvn clean install
Para correr el backend:

bash
CopiarEditar
mvn spring-boot:run
✅ Esto levantará el servidor Spring Boot en:

arduino
CopiarEditar
http://localhost:8080
4. Configuración y Ejecución del Frontend
4.1 Ir al directorio del frontend
Si estabas en el backend, regresa a la raíz del proyecto:

bash
CopiarEditar
cd ../frontend
4.2 Instalar dependencias del frontend
Si utilizas Bun:

bash
CopiarEditar
bun install
Si utilizas npm:

bash
CopiarEditar
npm install
4.3 Configurar la URL de la API en Angular
Para que el frontend consuma datos del backend, edita el archivo:

bash
CopiarEditar
frontend/src/environments/environment.ts
Y coloca la URL de tu backend. Ejemplo:

ts
CopiarEditar
export const environment = {
  production: false,
  apiUrl: 'http://localhost:8080'
};
4.4 Levantar el frontend
Si usas Bun:

bash
CopiarEditar
bun run start
Si usas npm:

bash
CopiarEditar
npm run start
✅ Esto levantará el frontend en:

arduino
CopiarEditar
http://localhost:4200
✅ Qué Funcionalidades Incluye
Con este sistema podrás:

Registrar pedidos de los clientes.
Consultar y gestionar pedidos existentes.
Administrar menús y productos.
Gestionar usuarios y roles mediante Spring Security.
Disfrutar de una interfaz moderna y responsiva gracias a Angular y Tailwind CSS.
📁 Estructura Recomendada del Proyecto
La estructura del backend recomendada es la siguiente:

css
CopiarEditar
backend
└── src
    └── main
        └── java
            └── com
                └── example
                    └── myapp
                        ├── config
                        ├── controller
                        ├── dto
                        ├── entity
                        ├── exception
                        ├── repository
                        ├── security
                        ├── service
                        └── util
Contenido de cada paquete:

config → Configuraciones globales.
controller → Clases @RestController para manejar endpoints HTTP.
dto → Data Transfer Objects, para no exponer entidades directamente.
entity → Entidades JPA mapeadas a tablas MySQL.
exception → Manejo global de errores.
repository → Interfaces JPA (extienden JpaRepository).
security → Configuración de seguridad (Spring Security).
service → Lógica de negocio.
util → Clases utilitarias o mappers.
🙌 Contribuciones
¡Las contribuciones son bienvenidas! Puedes:

Crear issues para reportar errores o sugerencias.
Enviar pull requests con mejoras.
📄 Licencia
Este proyecto está bajo la licencia MIT.
✨ Autor
[Tu Nombre]

Ingeniero de Sistemas e Informática
markdown
CopiarEditar

---## ✅ Qué debes personalizar- Reemplaza `https://github.com/tu-usuario/tu-repo.git` con la URL de tu repositorio.- Completa tu nombre en la sección **Autor**.- Coloca tus credenciales reales de MySQL en `application.properties`.- Ajusta la URL de tu API en el `environment.ts` si usas otro puerto o dominio.- Puedes añadir más detalles de tu proyecto (screenshots, diagramas, etc.) si lo deseas.

¡Con esto tienes un README **totalmente integrado**, sin partes sueltas, listo para GitHub y para que cualquiera pueda clonar y correr TODO el proyecto de inicio a fin!

¿Quieres algo más breve, en inglés o con más secciones como diagramas o capturas de pantalla?


Preguntar a ChatGPT:damelo en un solo markdown
```
> 
