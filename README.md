<img alt="UCU" src="https://www.ucu.edu.uy/plantillas/images/logo_ucu.svg"
width="150"/>

# Universidad Católica del Uruguay

## Facultad de Ingeniería y Tecnologías

### Programación II

# Consigna proyecto 2026 - Campus Salto

Este semestre, desarrollaremos... ¡chatbots! 🤖

![Bender](https://media.giphy.com/media/mIZ9rPeMKefm0/giphy.gif)

## Contexto

Un chatbot o [bot conversacional](https://es.wikipedia.org/wiki/Bot_conversacional)
es un programa que simula mantener una conversación con una persona al proveer
respuestas automáticas a entradas hechas por el usuario.

Existen gran variedad de chatbots actualmente y varios *sabores*. Hay chatbots
que simplemente responden a comandos pre-establecidos, y otros que integran
algoritmos de [inteligencia artificial](https://es.wikipedia.org/wiki/Inteligencia_artificial)
para procesar los mensajes de los usuarios e [interpretar lo que se está diciendo](https://es.wikipedia.org/wiki/Procesamiento_de_lenguajes_naturales).

Algunas de las aplicaciones más conocidas que abren sus puertas al desarrollo de
chatbots —tienen API— son:

* Telegram
* Messenger
* Whatsapp
* Slack
* Discord

entre otras; y nos integraremos al menos a una de ellas.

--

## 🧩 Descripción general

El sistema debe:

- Gestionar distintos tipos de ítems (por ejemplo: canciones, películas, productos)
- Registrar interacciones de los usuarios con esos ítems
- Analizar preferencias e historial
- Generar recomendaciones personalizadas utilizando distintas estrategias
- Aplicar filtros y ranking sobre los resultados

---

## 🏗️ Requisitos funcionales

El sistema debe permitir:

1. Registrar usuarios  
2. Registrar ítems de al menos un dominio (ej: música)  
3. Registrar interacciones (reproducciones, compras, visualizaciones, etc.)  
4. Definir preferencias de usuario  
5. Ejecutar recomendaciones para un usuario  
6. Filtrar resultados (por ejemplo: excluir ítems ya consumidos)  
7. Ordenar recomendaciones según algún criterio (ranking o score)  
8. Mostrar un listado final de recomendaciones  

---

## 🧠 Requisito clave de diseño

El motor de recomendación debe estar desacoplado del dominio.

Esto implica que:

- No debe depender de clases concretas como “Canción” o “Película”  
- Debe trabajar con abstracciones  
- Debe poder reutilizarse para otro dominio sin modificaciones  

## Historias de Usuario

**HU1**  
Como usuario quiero registrarme para poder utilizar el sistema.  

**Criterios de aceptación:**
- Dado que no estoy registrado, cuando ingreso mis datos, entonces se crea una cuenta válida.
- El sistema valida que el usuario no exista previamente.
- El usuario queda habilitado para usar el sistema.

---

**HU2**  
Como usuario quiero definir mis preferencias para personalizar mi experiencia.  

**Criterios de aceptación:**
- El usuario puede seleccionar uno o más atributos (género, categoría, etc.).
- Las preferencias quedan almacenadas.
- Las recomendaciones consideran dichas preferencias.

---

**HU3**  
Como usuario quiero visualizar un listado de recomendaciones para decidir qué consumir.  

**Criterios de aceptación:**
- El sistema muestra una lista de ítems recomendados.
- La lista contiene al menos un criterio de orden.
- Cada ítem muestra información básica (nombre, atributos relevantes).

---

**HU4**  
Como usuario quiero recibir recomendaciones basadas en mi historial para descubrir contenido relevante.  

**Criterios de aceptación:**
- El sistema utiliza interacciones previas del usuario.
- Se generan recomendaciones distintas al contenido ya consumido.
- Cambios en el historial afectan las recomendaciones.

---

**HU5**  
Como usuario quiero recibir recomendaciones basadas en mis preferencias para mejorar la relevancia.  

**Criterios de aceptación:**
- El sistema utiliza atributos definidos en preferencias.
- Las recomendaciones coinciden con al menos una preferencia.
- Cambiar preferencias modifica los resultados.

---

**HU6**  
Como usuario quiero recibir recomendaciones basadas en usuarios similares para descubrir contenido nuevo.  

**Criterios de aceptación:**
- El sistema identifica usuarios con comportamiento similar.
- Se recomiendan ítems consumidos por usuarios similares.
- No se incluyen ítems ya consumidos por el usuario.

---

**HU7**  
Como usuario nuevo quiero recibir recomendaciones basadas en popularidad o tendencias para tener una buena experiencia inicial.  

**Criterios de aceptación:**
- Si el usuario no tiene historial, se usa una estrategia alternativa.
- Se muestran ítems populares o recientes.
- El sistema no falla ante ausencia de datos.

---

**HU8**  
Como usuario quiero excluir contenido con ciertas características para refinar las recomendaciones.  

**Criterios de aceptación:**
- El usuario puede definir filtros (por atributo).
- Los ítems que cumplen el filtro son excluidos.
- El sistema aplica los filtros antes de mostrar resultados.

---

**HU9**  
Como usuario quiero que las recomendaciones estén ordenadas según un criterio para facilitar la elección.  

**Criterios de aceptación:**
- El sistema define un criterio de orden (score, relevancia, etc.).
- Los resultados se presentan ordenados.
- Cambiar el criterio modifica el orden.

---

**HU10**  
Como usuario quiero registrar mis interacciones para mejorar recomendaciones futuras.  

**Criterios de aceptación:**
- Cada consumo de ítem genera una interacción.
- Las interacciones quedan almacenadas en el historial.
- El sistema utiliza estas interacciones para recomendar.

---

**HU11**  
Como usuario quiero indicar si un contenido me gustó o no para ajustar las recomendaciones.  

**Criterios de aceptación:**
- El usuario puede marcar un ítem como “me gusta” o “no me gusta”.
- Esta información afecta futuras recomendaciones.
- El sistema diferencia entre consumo y valoración.

---

**HU12**  
Como usuario quiero ver el contenido que ya consumí para evitar repetirlo.  

**Criterios de aceptación:**
- El usuario puede consultar su historial.
- El historial muestra los ítems consumidos.
- El historial se actualiza automáticamente.

---

**HU13**  
Como usuario quiero que no se me recomiende contenido ya consumido.  

**Criterios de aceptación:**
- El sistema excluye ítems del historial.
- No aparecen duplicados en recomendaciones.
- El filtro se aplica automáticamente.

---

**HU14**  
Como usuario quiero guardar contenido para consumir más tarde.  

**Criterios de aceptación:**
- El usuario puede guardar ítems.
- Existe una lista de “guardados”.
- Los ítems guardados pueden recuperarse.

---

**HU15**  
Como usuario quiero recibir recomendaciones de contenido relacionado a uno que ya consumí.  

**Criterios de aceptación:**
- El sistema identifica atributos del ítem base.
- Se recomiendan ítems similares.
- El resultado cambia según el ítem seleccionado.

---

**HU16**  
Como administrador quiero eliminar ítems para mantener el catálogo actualizado.  

**Criterios de aceptación:**
- Se pueden eliminar ítems existentes.
- Los ítems eliminados no aparecen en recomendaciones.
- No se rompe el sistema si un ítem fue consumido previamente.

## Roadmap

El proyecto se divide en varias entregas a lo largo del semestre, que se
detallan [más abajo](#entregas).

Cada entrega es una parte del proyecto que construye sobre la anterior. Al final
del semestre tendremos un conjunto de chatbots funcionales con los que podremos
conversar.

La estructura del trabajo en el proyecto será la siguiente:

* [ ] Kick-off
* [ ] Primera entrega
* [ ] Segunda entrega
* [ ] Entrega final
* [ ] Defensa



## Entregas

> [!WARNING]
> **Importante:** Las entregas serán hasta las 23:59 del día indicado.

| Instancia | Fecha | Entregables |
| --- | --- | --- |
| Kick-off | 18 de setiembre | |
| [Primera entrega](Entregas/Entrega1.md) | 4 de octubre | Trello, diagramas de clases, código de clases de dominio + [fachada](https://refactoring.guru/design-patterns/facade) |
| [Segunda entrega](Entregas/Entrega2.md) | 8 de noviembre | Trello actualizado, entrega de [user stories](https://es.wikipedia.org/wiki/Historias_de_usuario) implementadas. Las historias de usuario deberán ser implementadas mediante [casos de prueba](https://en.wikipedia.org/wiki/Test_case) usando la fachada. |
| [Entrega final](Entregas/Entrega3.md) | 25 de noviembre | Trello actualizado, bot funcionando y entregables según se indica en la [consigna de la entrega](./Entregas/Entrega3.md) |
| Defensa | 27 de noviembre |
