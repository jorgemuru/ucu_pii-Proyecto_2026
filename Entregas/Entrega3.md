# Universidad Católica del Uruguay
<img src="https://ucu.edu.uy/sites/all/themes/univer/logo.png">

## Facultad de Ingeniería y Tecnologías
### Programación II

## Entrega (Final)

<br>

En esta última instancia terminaremos el desarrollo del nuestro chatbot por completo. Hasta el momento han desarrollado el modelo. Ahora agregarán todas las piezas restantes que rodean al _core_.

## Entregables

**Proyecto de C#** que incluye:

- Código de la solución (`src/Library/`)

- Código para iniciar el chatbot (`src/Program/`)

- Casos de test (en uno o mas proyectos de test dentro del directorio `test/`)

- Documentación (generada con [doxygen](https://www.doxygen.nl/index.html))

> [!IMPORTANT]
> En esta oportunidad sí deberán entregar `Program.cs` con código funcional que inicie el chatbot.

> [!IMPORTANT]
> Como siempre, haremos especial hincapié en las justificaciones de principios y patrones utilizados.

> [!TIP]
> Existe un catálogo de patrones de diseño que es parte de la bibliografía del curso. Si no puedes acceder al libro, existen recursos online como [refactoring.guru/design-patterns](https://refactoring.guru/design-patterns). Es importante que conozcas los patrones del catálogo y los utilices en tu solución.

El bot será implementado en **Discord**. Mira [este ejemplo](https://github.com/ucudal/PII_DiscordBot_Demo) para armar tu próxima entrega.

## Fecha de entrega

Véase [Tabla de Entregas](../README.md#entregas).

## Medio de entrega

Se entregará en una [tarea de WebAsignatura](https://webasignatura.ucu.edu.uy) un link al repositorio del equipo conteniendo todos los artefactos entregables. Si no se entrega link a un commit específico de la rama _main_, el equipo docente evaluará el último commit en _main_ previo a la fecha de entrega.

Un integrante por equipo deberá completar la entrega.

**No se admitirán entregas fuera de fecha.**

**Sólo se admitirán entregas por WebAsignatura en la tarea provista con link a GitHub y en la rama master<sup>1</sup>.**

Todos los entregables que sean de documentación (diagramas, tarjetas, documentos, etc.) deberán entregarse dentro del directorio `docs/`.

Los proyectos de código fuente deberán crearse dentro del directorio `src` (como es habitual).

Deberá existir ademas un archivo README.md en la raiz del repositorio para incluír **la descripción del proyecto** y **las notas del equipo**. Véase [Notas](#notas).

## Criterio de calificación

Los profesores vamos a mirar el cumplimiento de los siguientes criterios, alineados con la rúbrica del curso:

| Criterio | Peso |
| --- | ---: |
| Buen diseño orientado a objetos, aplica y documenta el uso de [patrones GRASP](https://github.com/ucudal/PII_Principios_Patrones/blob/master/GRASP.md) y [principios SOLID](https://github.com/ucudal/PII_Principios_Patrones/blob/master/SOLID.md) | 25% |
| Uso de C# y biblioteca .NET Core | 5% |
| Consistencia entre modelo UML/C# | 5% |
| Aplica patrones de código, por ejemplo, algunos de [estos](https://refactoring.guru/design-patterns) | 5% |
| Excepciones y diseño por contrato | 10% |
| Convenciones de código | 10% |
| Uso del repositorio: branch y merge, pull request, estado de las actions | 5% |
| Unit tests de clases | 5% |
| Unit tests de escenarios | 15% |
| Funcionamiento del bot | 10% |
| Trello | 5% |

## Notas

Alentamos al equipo a que utilice el archivo de README en su repositorio para incluír notas de reflexión durante el desarrollo del proyecto. Estas notas pueden incluír:

- Qué desafíos de la entrega fueron los más difíciles

- Qué cosas aprendieron enfrentándose al proyecto que no aprendieron en clase como parte de la currícula

- Qué recursos (páginas web, libros, foros, etc) encontraron que les fueron valiosos para sortear los desafíos que encontraron

- Y cualquier otro tipo de reflexión, material o comentarios sobre el trabajo en el proyecto.
