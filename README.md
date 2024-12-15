# Starwars-ScreanMatch
crear una aplicación que consulte la API pública de Star Wars (SW API) y guarde la información de las 6 primeras películas en archivos JSON.

---

# 🌌 Aplicación Star Wars API - Desafío JSON

Este proyecto es una aplicación en **Java** que interactúa con la **API pública de Star Wars (SWAPI)** para obtener información sobre las 6 primeras películas de la saga y guardarlas en archivos JSON. El objetivo del desafío es aprender a realizar solicitudes HTTP, procesar datos de la API y guardarlos en un formato estructurado como JSON.

## 🚀 ¿Qué hace esta aplicación?

1. **Consumo de la API de Star Wars (SWAPI)**:
   - La aplicación consulta la API pública de Star Wars ([SWAPI](https://swapi.dev/)) para obtener detalles sobre las películas.

2. **Procesamiento de Datos**:
   - Filtra la información relevante de cada película, como:
     - Título.
     - Director.
     - Productor.
     - Fecha de lanzamiento.
     - Sinopsis.

3. **Generación de Archivos JSON**:
   - La información de cada película se guarda en un archivo JSON individual, estructurado de forma clara y legible.

4. **Aprendizajes Clave**:
   - Realizar solicitudes HTTP en Java.
   - Procesar y estructurar datos en formato JSON.
   - Manejar operaciones de escritura de archivos con buenas prácticas.

---

## 📂 Estructura del Proyecto

```plaintext
.
├── src
│   ├── Main.java            # Clase principal del programa
│   ├── ApiClient.java       # Clase para manejar las solicitudes HTTP a la API
│   ├── Movie.java           # Modelo para representar las películas
│   ├── JsonFileWriter.java  # Clase para guardar datos en archivos JSON
│   └── Utils.java           # Métodos auxiliares y validaciones
├── README.md                # Documentación del proyecto
├── movies                   # Carpeta con los archivos JSON generados
│   ├── movie_1.json
│   ├── movie_2.json
│   ├── ...
└── resources
    └── config.properties    # Configuración (URL base, headers, etc.)
```

---

## 🛠️ Tecnologías Utilizadas

- **Lenguaje**: Java.
- **HTTP Client**: `HttpURLConnection` para realizar solicitudes HTTP.
- **Gestión de JSON**: Biblioteca `Gson` o `Jackson` para procesar y generar archivos JSON.
- **Escritura de Archivos**: Clases como `BufferedWriter` y `FileWriter`.

---

## 🔧 Configuración y Ejecución

1. **Clonar el Repositorio**:
   ```bash
   git clone https://github.com/tuusuario/starwars-api-json.git
   cd starwars-api-json
   ```

2. **Configurar la API**:
   - El archivo `config.properties` debe contener la URL base de la API:
     ```properties
     API_BASE_URL=https://swapi.dev/api
     ```

3. **Compilar y Ejecutar**:
   - Compilar el proyecto:
     ```bash
     javac src/*.java
     ```
   - Ejecutar el programa:
     ```bash
     java -cp src Main
     ```

4. **Resultado**:
   - Se crearán 6 archivos JSON en la carpeta `movies/`, cada uno con información de una película.

---

## 📝 Ejemplo de Salida (Archivo JSON)

Cada archivo generado contiene información relevante de la película, por ejemplo:

**Archivo: `movie_1.json`**
```json
{
  "title": "A New Hope",
  "director": "George Lucas",
  "producer": "Gary Kurtz, Rick McCallum",
  "release_date": "1977-05-25",
  "opening_crawl": "It is a period of civil war..."
}
```

---

## 🎯 Aprendizajes

Este desafío me permitió:

1. **Consumo de APIs REST**:
   - Aprendí a realizar solicitudes HTTP desde Java y procesar las respuestas en formato JSON.

2. **Procesamiento y Estructuración de Datos**:
   - Manejar objetos JSON y almacenarlos en archivos estructurados utilizando herramientas como Gson o Jackson.

3. **Gestión de Archivos**:
   - Implementar buenas prácticas para guardar datos en archivos locales y estructurar carpetas de salida.

4. **Fortalecimiento de Lógica de Programación**:
   - Aplicar conceptos de modularidad, reusabilidad y manejo de excepciones en Java.

---

## 🌟 Funcionalidades Futuras

- Implementar una interfaz gráfica para mostrar las películas en tiempo real.
- Añadir soporte para descargar datos de personajes, naves espaciales y planetas.
- Generar un archivo consolidado con todas las películas.

---

## 🏷️ Etiquetas

`#Java` `#APIs` `#SWAPI` `#JSON` `#DesarrolloBackend`

---

Espero que este `README` sea útil para documentar tu proyecto. Si necesitas personalizarlo más o añadir detalles específicos, ¡avísame! 🚀
