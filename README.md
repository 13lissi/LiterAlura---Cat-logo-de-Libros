# LiterAlura - Catálogo de Libros 📚

¡Bienvenido al desafío LiterAlura! Este proyecto es una aplicación de consola desarrollada como parte del programa **Oracle Next Education (ONE)** en conjunto con **Alura Latam**. El objetivo es consumir la API de Gutendex para buscar libros, procesar los datos y persistirlos en una base de datos relacional.

## 🚀 Funcionalidades

- **Búsqueda de libros por título**: Consulta la API externa y registra el libro y su autor en la base de datos.
- **Listar libros registrados**: Muestra todos los libros que han sido persistidos.
- **Listar autores registrados**: Muestra una lista única de autores con sus datos básicos.
- **Listar autores vivos en un año determinado**: Filtra autores basados en su año de nacimiento y fallecimiento.
- **Listar libros por idioma**: Permite filtrar la colección local por siglas de idioma (ES, EN, FR, PT).
- **Validaciones**: Control de duplicados en la base de datos y manejo de búsquedas sin resultados.

## 🛠️ Tecnologías utilizadas

* **Java 17**
* **Spring Boot 3.x**
* **Spring Data JPA**
* **PostgreSQL**
* **Jackson** (para manipulación de JSON)
* **API Gutendex** (Proyecto Gutenberg)

## 📋 Requisitos Previos

1.  **Java JDK 17** instalado.
2.  **PostgreSQL** en ejecución.
3.  Una IDE (IntelliJ IDEA, Eclipse, VS Code).
4.  Configurar el archivo `src/main/resources/application.properties` con tus credenciales:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/literalura
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contrasena
spring.jpa.hibernate.ddl-auto=update
