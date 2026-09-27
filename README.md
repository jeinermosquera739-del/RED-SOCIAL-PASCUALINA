# Modelo Lógico de Base de Datos - Red Social Estudiantil Pascualina

##  Integrantes del Equipo
* Luis Rojas Cano
* Emily Quintero Rivera
* Sofia Hidalgo Cordoba
* Jeiner Andres Mosquera



##  Breve Descripción del Caso

El objetivo de este proyecto es el análisis, diseño y normalización de un **modelo lógico de base de datos** para la **Red Social Estudiantil Pascualina**. Esta plataforma está orientada exclusivamente a la comunidad estudiantil, permitiendo la interacción académica y social entre alumnos sin la inclusión de entidades de gestión administrativa o docente.

El sistema soporta funcionalidades clave divididas en módulos:
* **Identidad y Perfil:** Registro de estudiantes, fotos y biografías (relación 1:1).
* **Contenido e Interacción:** Creación de publicaciones, comentarios y reacciones.
* **Comunidad:** Gestión de grupos de estudio y roles de moderación dentro de las membresías.
* **Eventos y Comunicación:** Organización de eventos estudiantiles y salas de chat (individuales y grupales).
* **Vida Académica:** Módulos para compartir cursos e investigaciones académicas.

###  Normalización y Estructura
El diseño relacional consta de **18 tablas lógicas** obtenidas mediante un riguroso proceso de normalización:
1. **1FN (Atomicidad):** Descomposición de atributos multivaluados (intereses, grupos) en entidades independientes.
2. **2FN (Dependencia Funcional Completa):** Eliminación de dependencias parciales en tablas puente con claves primarias compuestas (`menbresia`, `estudiantes, etc.).
3. **3FN (Eliminación de Transitividades):** Desvinculación de campos redundantes para evitar anomalías en inserciones, actualizaciones y borrados.
