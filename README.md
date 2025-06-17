# Taller Colaborativo: Datos Abiertos de Valencia y Desarrollo Full Stack

¡Bienvenidos a este emocionante taller colaborativo donde fusionaremos el poder del análisis de datos con la robustez del desarrollo web! Este ejercicio está diseñado para que los estudiantes de Ciencia de Datos y Full Stack trabajen juntos en un proyecto real, desde la adquisición de datos hasta la visualización interactiva.

## 1. Introducción al Proyecto

El objetivo de este taller es construir una aplicación que permita explorar los datos de centros educativos del Ayuntamiento de Valencia. Los estudiantes de Ciencia de Datos se encargarán de la ingesta y preparación de los datos, mientras que los estudiantes de Full Stack desarrollarán una API para servir estos datos. Finalmente, los estudiantes de Ciencia de Datos crearán una interfaz de usuario interactiva para visualizar la información.

Este proyecto simula un escenario real de colaboración interdisciplinaria, donde cada equipo aporta su expertise para lograr un producto final completo y funcional.

## 2. Roles y Responsabilidades

### 2.1. Equipo de Ciencia de Datos (DS)

El equipo de Ciencia de Datos será responsable de:

*   **Exploración y Descarga de Datos:** Acceder al portal de Datos Abiertos del Ayuntamiento de Valencia y descargar las tablas de centros educativos. Se recomienda utilizar el formato CSV o JSON para facilitar la ingesta.
*   **Ingesta y Almacenamiento en GCP:** Cargar los datos descargados en una base de datos en Google Cloud Platform (GCP). Se puede utilizar PostgreSQL, MySQL o cualquier otra base de datos relacional compatible con GCP. Es crucial asegurar la calidad y consistencia de los datos durante este proceso.
*   **Visualización con Streamlit:** Una vez que la API esté operativa, construir una aplicación interactiva utilizando Streamlit para visualizar los datos de los centros educativos. La visualización debe ser intuitiva y permitir a los usuarios filtrar y explorar los datos. Se sugiere incluir:
    *   Un desplegable para seleccionar el distrito de Valencia.
    *   Un desplegable para filtrar por tipo de centro (público, privado, concertado).
    *   Gráficos o tablas que muestren la distribución de centros, número de estudiantes, etc.

### 2.2. Equipo de Full Stack Development (FS)

El equipo de Full Stack Development será responsable de:

*   **Diseño y Desarrollo de la API RESTful:** Construir una API robusta y bien documentada para exponer los datos de los centros educativos almacenados en GCP. La API debe ser capaz de:
    *   Obtener todos los centros educativos.
    *   Filtrar centros por distrito.
    *   Filtrar centros por tipo (público, privado, concertado).
    *   Combinar filtros.
*   **Documentación de la API con Swagger/OpenAPI:** Generar una documentación interactiva de la API utilizando Swagger UI o ReDoc. Esto es fundamental para que el equipo de Ciencia de Datos pueda consumir la API de manera eficiente.
*   **Despliegue (Opcional):** Si el tiempo lo permite, desplegar la API en un entorno de nube (por ejemplo, Google App Engine, Cloud Run o una VM en GCP).

## 3. Flujo de Trabajo y Arquitectura

El siguiente diagrama ilustra el flujo de trabajo y la arquitectura propuesta para el taller:

![Diagrama de Arquitectura](https://private-us-east-1.manuscdn.com/sessionFile/LNN3BYeKu5lvTWVfMjz1s7/sandbox/vfGD1HWLimRjGmQ1UyrwRS-images_1750054219818_na1fn_L2hvbWUvdWJ1bnR1L2FyY2hpdGVjdHVyZV9kaWFncmFt.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9wcml2YXRlLXVzLWVhc3QtMS5tYW51c2Nkbi5jb20vc2Vzc2lvbkZpbGUvTE5OM0JZZUt1NWx2VFdWZk1qejFzNy9zYW5kYm94L3ZmR0QxSFdMaW1SakdtUTFVeXJ3UlMtaW1hZ2VzXzE3NTAwNTQyMTk4MThfbmExZm5fTDJodmJXVXZkV0oxYm5SMUwyRnlZMmhwZEdWamRIVnlaVjlrYVdGbmNtRnQucG5nIiwiQ29uZGl0aW9uIjp7IkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNzY3MjI1NjAwfX19XX0_&Key-Pair-Id=K2HSFNDJXOU9YS&Signature=Wz7NN3C4E5GTVta1tGXoyuPyAw1BcUG1f97obpWqBqw5ByvK01R7X~68YKMkJMv41cNYhqsG9KRrga237QNmH1J9YpqpvnPyDsSgc2zJ5k2r3XjA6EkTkbA2fxzhheCE7hY7j-dJUh~dqrCPzxw-HkxcdLU~1~MvFqWRDwzZKzsvKfZJzJwH7BESZ851h~MaqLgL6B2-be2fYQmO70T6gdzpJ04K1ds0u8jXg5xL7K9FvMO1ptF4iIK8mssZEwseLhyC90mt5Ikq05wYvdVFgE4a1Z5qY-LDkMBJHGPg0AJYVabk7snbIP-ANa6BNFUcz3VQ8zUsbCR7J1R7I-56~Q__)

**Explicación del Flujo:**

1.  **Datos Abiertos del Ayuntamiento de Valencia:** El punto de partida son los datos públicos disponibles en el portal de datos abiertos.
2.  **Ingesta de Datos (DS):** El equipo de Ciencia de Datos descarga y procesa estos datos.
3.  **Base de Datos GCP (DS):** Los datos limpios y estructurados se almacenan en una base de datos en Google Cloud Platform.
4.  **API RESTful (FS):** El equipo de Full Stack desarrolla una API que se conecta a la base de datos de GCP para servir los datos.
5.  **Aplicación Streamlit (DS):** El equipo de Ciencia de Datos consume la API para construir una interfaz de usuario interactiva.

## 4. Recursos Útiles

Aquí tienes algunos recursos que te serán de gran ayuda durante el taller:

### 4.1. Datos Abiertos del Ayuntamiento de Valencia

*   **Portal de Datos Abiertos:** [https://valencia.opendatasoft.com/pages/home/](https://valencia.opendatasoft.com/pages/home/)
*   **Dataset de Centros Educativos:** [https://valencia.opendatasoft.com/explore/dataset/centros-educativos-en-valencia/information/](https://valencia.opendatasoft.com/explore/dataset/centros-educativos-en-valencia/information/)
    *   Puedes exportar los datos en diferentes formatos (CSV, JSON, Excel) desde la pestaña 'Export'.
    *   La documentación de la API para este dataset se encuentra en la pestaña 'API'.

### 4.2. Google Cloud Platform (GCP)

*   **Documentación de GCP:** [https://cloud.google.com/docs](https://cloud.google.com/docs)
*   **Bases de Datos en GCP (Cloud SQL):** [https://cloud.google.com/sql/docs](https://cloud.google.com/sql/docs)

### 4.3. Desarrollo Full Stack 

*   **SEQUELIZE:** [sequelize])(https://sequelize.org/)
*   **Node:** [node](https://nodejs.org/es)
*   **Swagger UI:** [https://swagger.io/tools/swagger-ui/](https://swagger.io/tools/swagger-ui/)

### 4.4. Visualización de Datos (Streamlit)

*   **Streamlit Documentation:** [https://docs.streamlit.io/](https://docs.streamlit.io/)

## 5. Consejos y Buenas Prácticas

*   **Comunicación:** La comunicación constante entre ambos equipos es clave para el éxito del proyecto.
*   **Control de Versiones:** Utilización Git y GitHub/GitLab para el control de versiones del código. Esto facilitará la colaboración y el seguimiento de los cambios.
*   **Manejo de Errores:** Implementar un manejo de errores robusto tanto en la ingesta de datos como en la API y la aplicación Streamlit.
*   **Modularidad:** Diseño del código de manera modular para facilitar el mantenimiento y la escalabilidad.
*   **Pruebas:** Realizad pruebas unitarias y de integración para asegurar la calidad del código y la funcionalidad de la aplicación.



## PREGUNTAS FINALES

* Que hace un FS? Que hace un DS?
* Que ventajas tiene hacer un front en JS vs python? Y viceversa?
* Qué ventajas e inconvenientes tiene usar streamlit como front?
* Como de importante es la comunicacion?
* Como os habeis organizado para paralelizar tareas (que el ritmo no pare!)?
