<img alt="UCU" src="https://www.ucu.edu.uy/plantillas/images/logo_ucu.svg"
width="150"/>

# Universidad Católica del Uruguay

## Facultad de Ingeniería y Tecnologías

### Programación II

# Primera entrega

<br>

En esta primera instancia nos enfocaremos fuertemente en el modelado del problema. A continuación se detallan los artefactos entregables para la primera instancia del proyecto y el formato de cada uno de ellos.

## Medio de entrega

Se entregará en una tarea de WebAsignatura un link al repositorio del equipo
conteniendo todos los artefactos entregables.

Deberán generar un repositorio con siguiente formato en el nombre "ucu_p2_proyecto2026_grupoxx", detallando en "grupoxx" el nombre del grupo, el mismo deberá ser privado e incluir como colaborador al docente.

Un integrante por equipo deberá completar la entrega.

**No se admitirán entregas fuera de fecha.**

**Sólo se admitirán entregas por WebAsignatura en la tarea provista con link a
GitHub y en la rama `main`[^1].**

[^1]: En caso de que WebAsignatura o GitHub no se encuentren en línea para realizar la entrega antes de finalizado el plazo de entrega se aceptará como excepción entrega por correo electrónico del repositorio completo en formato zip.

## Estructura del repositorio

El repositorio del equipo deberá organizarse de la siguiente manera:

```
docs/
src/
  Program/
  Library/
test/
  LibraryTests/
  ...
README.md
```

> [!IMPORTANT]
> Los proyectos deben incluir el atributo `<LangVersion>6</LangVersion>` en la
> primera sección `<PropertyGroup>...</PropertyGroup>` de los archivos `.csproj`.

Todos los entregables que sean de documentación, tales como diagramas, tarjetas,
documentos, etc., deberán entregarse dentro de la carpeta `docs/`.

Los proyectos de código fuente deberán crearse dentro del directorio `src` como
es habitual.

Deberá existir ademas un archivo `README.md` en la raiz del repositorio para
incluír las notas del equipo. Vean [Notas](#notas).

El archivo `README.md` deberá incluir también el link al Trello donde gestionan
las tareas del equipo. Vean [Trello](#trello).

## Entregables

- **Diagrama de clases** Uno o más diagramas UML simples con las clases del
  modelo identificadas

  - Formato: png, jpg, jpeg, pdf, html o markdown.

  - Pueden utilizar tanto [Draw.io](https://app.diagrams.net) como
    [PlantUMl](https://plantuml.com) o [Mermaid](https://mermaid.live).

- **Código C# de las clases de dominio y casos de prueba**

  - Formato: .cs, .csproj

- **Trello**

  - Formato: link incluido en el arhcivo README.md. Vean [Trello](#trello).

## Fecha de entrega

Véase [Tabla de Entregas](../README.md).

## Criterio de calificación

Los profesores vamos a mirar el cumplimiento de los siguientes criterios, alineados con la rúbrica del curso:

| Criterio | Peso |
| --- | ---: |
| Buen diseño orientado a objetos, aplica y documenta el uso de principios/patrones SRP, Expert, Polimorfismo, LSP | 40% |
| Uso de C# y biblioteca .NET Core | 5% |
| Consistencia entre tarjetas CRC, modelo UML, C# | 15% |
| Convenciones de código | 10% |
| Uso del repositorio | 10% |
| Unit tests de clases | 10% |
| Uso y manejo del Trello | 10% |

## Trello

Los equipos deberán crear un tablero en [Trello](https://trello.com). Todos los
integrantes del equipo deberán tener acceso y colaborar en la gestión del
tablero.

El tablero debe tener las siguientes columnas:

- **TODO**. TODO es *to do* o para hacer; aquí van las tareas que identificaron
  y en las que todavía no están trabajando.

- **WIP**. WIP es *work in progress* o trabajo en progreso; aquí van las tareas
  en las que están trabajando.

- **DONE**. DONE es terminado; aquí van las tareas terminadas.

Cada tarea en el tablero debe incluir:

- El estudiante responsable de completar esa tarea. Puede haber un solo
  responsable por tarea.

- Una fecha en la que la tarea debería quedar completada.

Agreguen al tablero, **al menos**, tareas para:

- Modelar en uno o más diagramas de clases UML para las clases de dominio que
  surgen de cada historia de usuario. Recomendamos asignar cada historia de
  usuario a un integrante del equipo de forma que todos los integrantes
  participen en el modelado.

- Codificar en C# las clases de dominio modeladas. Recomendamos asignar una
  clase a cada integrante del equipo de forma que todos los integrantes
  participen en la programación.

- Crear casos de prueba para cada método en cada clase. Recomendamos que el
  integrante que codifique la clase haga también las pruebas.

## Notas

Alentamos al equipo a que utilice el archivo de README en su repositorio para
incluír notas de reflexión durante el desarrollo del proyecto. Estas notas
pueden incluír:

- Qué desafíos de la entrega fueron los más difíciles

- Qué cosas aprendieron enfrentándose al proyecto que no aprendieron en clase como parte de la currícula

- Qué recursos (páginas web, libros, foros, etc) encontraron que les fueron valiosos para sortear los desafíos que encontraron

- Y cualquier otro tipo de reflexión, material o comentarios sobre el trabajo en el proyecto.
