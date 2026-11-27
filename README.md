# Proyecto Web y Control de Versiones

---

## Tabla de Contenidos

- [Estructura del Proyecto](#estructura-del-proyecto)
- [Gestión de Ramas](#gestión-de-ramas)
- [Historial de Mejoras Implementadas](#historial-de-mejoras-implementadas)
- [Instalación y Despliegue Local](#instalación-y-despliegue-local)

---

## Estructura del Proyecto

El repositorio está estructurado en torno a una página principal (`index.html`) y dos módulos complementarios desarrollados de forma aislada:

```text
ra1/
├── .gitignore          # Reglas para omitir carpetas y archivos temporales
├── README.md           # Documentación técnica del proyecto y control de versiones
├── index.html          # Página principal y punto de entrada al sitio web
├── contacto.html       # Módulo de información y formulario de contacto
└── calendario.html     # Módulo de planificación y tabla horaria semanal

Gestión de Ramas
Para garantizar que el código principal permanezca siempre funcional y limpio, el trabajo se dividió en tres líneas de desarrollo:

#1. Rama main (Producción / Base)
Propósito: Aloja la versión base y estable del proyecto.

Contenido: Contiene index.html, la configuración de exclusión .gitignore y este archivo de documentación README.md.

Rol: Sirve como punto de partida para las ramas de características y destino final donde convergerán las mejoras mediante fusión (merge).

#2. Rama diseño A: contacto (o primera rama de funcionalidad)
Propósito: Desarrollo exclusivo del canal de comunicación con el usuario.

Archivos implicados: contacto.html y actualización de navegación en index.html.

Aislamiento: Permite iterar sobre el formulario sin alterar la rama principal ni interferir con otros diseños.

#3. Rama DisenoB (calendario de activiades)
Propósito: Línea paralela creada a partir de main para implementar el calendario de actividades.

Archivos implicados: calendario.html (o actividades.html).

Aislamiento: No contiene contacto.html, garantizando que ambas características evolucionen de forma completamente independiente.

Historial de Mejoras Implementadas
Inicialización y Exclusiones:

Creación del repositorio Git local (git init).

Definición de reglas en .gitignore para omitir carpetas no deseadas antes del primer commit.

Línea de Contacto:

Maquetación de datos de atención (teléfono, correo y horario de atención).

Incorporación de formulario de consulta con validación de campos obligatorios (required).

Enlace de retorno a index.html.

Línea de Diseño B (Actividades):

Maquetación de tabla horaria de lunes a domingo con distribución de cargas y disciplinas.

Marcado visual de actividades de alta exigencia física mediante indicador gráfico (🔥).

Documentación y Estandarización:

Redacción de especificaciones técnicas y guía de ramas en Markdown.


#Ultimas modificaciones

Sitio web estático desarrollado para la práctica de control de versiones con Git y GitHub.

## Tabla de contenidos
- [Descripción](#descripción)
- [Mejoras implementadas](#mejoras-implementadas)
- [Estructura del proyecto](#estructura-del-proyecto)

## Descripción
Proyecto base en HTML5 que demuestra el flujo de trabajo colaborativo mediante ramas, resolución de conflictos, uso de `.gitignore` e integración mediante Pull Requests en GitHub.

## Mejoras implementadas
1. **Página de contacto (`contacto.html`):** Desarrollada en la rama `diseñoA` y fusionada con `main`.
2. **Calendario de actividades (`actividades.html`):** Desarrollado en la rama `DisenoB` con resolución de conflictos en `index.html`.
3. **Contenido multimedia (`125222871.jpeg`):** Incorporado mediante la rama `feature/imagen` e integrado en `main` a través de un Pull Request en GitHub.

## Estructura del proyecto
- `index.html`: Página principal del sitio.
- `contacto.html`: Formulario y datos de contacto.
- `actividades.html`: Calendario de actividades.
- `125222871.jpeg`: Recurso gráfico integrado en la página principal.
- `.gitignore`: Exclusión de archivos temporales y ocultos del sistema (`.DS_Store`).