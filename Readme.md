¿Qué es una API?
Aplication
Programing
Interface

Interfaz de programación de aplicaciones.

Herramientas:
Noción Básica de Programación
Cualquier lenguaje de programación
Herramienta cURL
JQ texto json


Now.sh (Buscar esta herramienta)

¿Qué es HTTP?
(Hypertext Transfer Protocol)
Protocolo de transferencia de hipertexto
Protocolo de comunicador entre aplicaciones
Basado en el intercambio de texto

Petición HTTP
Internet
Petición al servidor
Respuesta a Internet
Respuesta HTTP

¿Qué significa REST? 
Representation State Transfer
Estilo de arquitectura de software enfocado en el intercambio de recursos y basado en HTTP, intercambio de archivos.

¿Qué es una API RESTful?
Una API diseñada alrededor de los conceptos de REST.

Conceptos REST
- Recurso: Cual es el recurso que queremos usar sobre una acción
- URI cual es efectivamente el recurso sobre el que vamos a actuar
- Acción cual es la acción que queremos ejecutar

Petición REST:
URL: A diferencia de la URI incluye el dominio, el protocolo, etc.
Verbo HTTP
Get Post Put Delete

El recurso puede ser cualquier cosa. Ejemplo una librería el recurso podría ser un libro, un autor, un género, etc.

Ejemplos REST
- GET/books/1
	obtener la información del libro que se identifica con el #1
- DELETE/books/50
	Que elimine el libro que se enumera con el 50.

Un cliente solicita una petición HTTP, EL SERVIDOr indica que no tiene los recursos y hace una segunda petición a otro recurso, va la petición REST al servidor y la envía al cliente.

¿Cuándo conviene utilizar REST?
	Ya que RESTful no es la única forma para utilizar servicios web existen otros.

* Interacciones simples 
	Por ejemplo solo agregar, quitar, modificar recursos 

* Recursos limitados
	y cuando lo srecursos en general son limitados.

No se recomienda cuando las operaciones son complejas que no es suficiente solo con la petición de recursos, si no que también se necesita que el servidor aporte más lógica. Por ejemplo la validación de algún documento.

Consumo vía REST
Realizar peticiones HTTP e interpretar las respuestas HTTP, este tipo de consumo no necesariamente la dispara la acción de un humano. Lo que son tareas programadas.


xkcd.com (página de chistes de programación) se puede consultar la API del algún comic. Ejemplo

https://xkcd.com/info.0.json

Nos mostrará un json con la información del cómic.

Abrimos inspect

Y nos va a dar la información de las solicitudes.

El consumo de la API vía REST se basa en los conceptos HTTP que  mencionabamos anteriormente.
GET: Se basa en buscar un recurso y traerlo. (es el más utilizado). Cuando se utiliza este método, toda la información que se envía viaja a través de la URL, por lo que es perfectamente para cualquiera.
POST: Con este método se crean recursos en el servidor.
PUT: Se modifican recursos en el servidor.
Cuando se usan los métodos POST y PUT la información es más privada y más segura.
DELETE: Se eliminan recursos del servidor.