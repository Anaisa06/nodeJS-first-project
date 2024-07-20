¿Qué es el filesystem (fs) en Node.js y para qué se utiliza?

fs es un módulo de Node.js que proporciona una API para interactuar con el sistema de archivos. Permite realizar operaciones CRUD (create, read, update, delete).

¿Qué es un middleware en Express y cuál es su propósito?

Un middleware en Express es una función que se ejecuta durante el ciclo de vida de una solicitud HTTP. Su propósito es realizar tareas como la manipulación de solicitudes y respuestas, la autenticación, el manejo de errores, la validación de datos y la implementación de lógica de negocio antes de que la solicitud llegue a una ruta específica.

¿Qué es un endpoint en una API RESTful y cuál es su función?

Un endpoint en una API RESTful es una URL específica que expone una función en particular y permite interactuar con ella mediante los diferentes verbos HTTP. Su función es permitir realizar operaciones como crear, leer, actualizar y eliminar datos en el servidor desde el lado de cliente.

¿Qué son los verbos HTTP y cuáles son los más comunes?

Los verbos HTTP son métodos que indican la acción a realizar sobre un recurso en una API. Los más comunes son: Get, que sirve para obtener información, POST, que sirve para enviar datos, PUT, que sirve para actualizar o cambiar datos, DELETE, que sirve para eliminar datos, y PATCH que sirve para actualizar datos de manera parcial.

¿Qué es JSON y por qué es utilizado en las API RESTful?

JSON es un formato de intercambio de datos que es ligero y fácil de leer y escribir para los humanos y de parsear y generar para las máquinas. Es utilizado en las API RESTful porque es independiente del lenguaje y fácil de comprender.

En lo que respecta al envio de datos a lo largo de los verbos http responde:

¿Qué es el body de una petición?

El body de una petición es la parte de la solicitud HTTP donde se envían los datos. Se usa en verbos como POST, PATCH y PUT donde se necesita enviar datos al servidor para crear o actualizar recursos.

¿Qué es el body de una respuesta?

El body de una respuesta es la parte de la respuesta HTTP donde se devuelven los datos solicitados. Contiene la información que el servidor envía al cliente.

¿Qué es el query de una petición?

El query de una petición son los parámetros que se envían en la URL después de un signo de interrogación. Se utilizan para enviar datos no sensibles y realizar filtros o búsquedas.

¿Qué es el params de una petición?

El params de una petición son los parámetros que forman parte de la ruta de la URL y se utilizan para identificar recursos específicos. Por ejemplo, en /tasks/:id, id es un parámetro para encontrar la task que tenga ese id.

En lo que respecta al verbo POST responde:

¿Qué es un verbo POST y cuál es su propósito?

El verbo POST es un método HTTP utilizado para enviar datos al servidor que sirve para crear un nuevo recurso. Los datos enviados en el body de la solicitud se utilizan para crear el recurso en el servidor.

¿Cuándo se utiliza un verbo POST?

Se utiliza un verbo POST cuando se necesita crear un nuevo recurso en el servidor, como agregar una nueva tarea en una base de datos o en este caso en el archibo tasks.json.

¿En qué se diferencia un verbo POST de los otros verbos HTTP como GET, PUT y DELETE?

Se diferencia en que el verbo POST es para crear un recurso completamente nuevo, mientras que los otros trabajan sobre recursos que ya existen.

¿Como se envian datos en un verbo POST?

Los datos se envían en el body de la solicitud. Normalmente se utiliza JSON para estructurar los datos que se envían al servidor.

En lo que respecta al verbo GET responde:

¿Qué es un verbo GET y cuál es su propósito?

El verbo GET es un método HTTP utilizado para solicitar datos de un servidor. Su propósito es recuperar información sin modificar ningún dato.

¿Cuándo se utiliza un verbo GET?

Se utiliza un verbo GET cuando se necesita recuperar información o datos de un servidor, como leer un archivo o consultar una base de datos.

¿En qué se diferencia un verbo GET de los otros verbos HTTP como POST, PUT y DELETE?

El verbo get solo obtiene los datos, más no los modifica. Los otros verbos si modifican el recurso.

En lo que respecta al verbo PUT responde:

¿Qué es un verbo PUT y cuál es su propósito?

El verbo PUT es un método HTTP utilizado para enviar datos al servidor con el propósito de actualizar un recurso existente.

¿Cuándo se utiliza un verbo PUT?

Se utiliza un verbo PUT cuando se necesita actualizar un recurso existente en el servidor o crear uno si no existe.

¿En qué se diferencia un verbo PUT de los otros verbos HTTP como POST, GET y DELETE?

El verbo PUT modifica los datos de un recurso existente, mientras que GET no modifica nada, POST crea un recurso nuevo, y DELETE lo borra por completo.

En lo que respecta al verbo DELETE responde:

¿Qué es un verbo DELETE y cuál es su propósito?

El verbo DELETE es un método HTTP utilizado para eliminar un recurso existente en el servidor.

¿Cuándo se utiliza un verbo DELETE?

Se utiliza un verbo DELETE cuando se necesita eliminar un recurso específico del servidor.

¿En qué se diferencia un verbo DELETE de los otros verbos HTTP como POST, GET y PUT?

Este verbo elimina el recurso por completo de la base de datos o el archivo, los otros verbos crean, modifican u obtienen.

¿Qué es un status code y cuáles son los más comunes?

Un status code es un código numérico que el servidor envía en la respuesta HTTP para indicar el resultado de la solicitud. Los más comunes son:

200 OK: La solicitud fue exitosa.
201 Created: Un recurso fue creado exitosamente.
400 Bad Request: La solicitud es inválida.
401 Unauthorized: Requiere autenticación.
403 Forbidden: La solicitud está prohibida.
404 Not Found: El recurso no fue encontrado.
500 Internal Server Error: Error en el servidor.

¿Cuales son los status code mas comunes para el verbo POST?

201 Created: Indica que el recurso fue creado exitosamente.
400 Bad Request: Indica que la solicitud no es válida.
401 Unauthorized: Falta autenticación.
403 Forbidden: La solicitud está prohibida.
500 Internal Server Error: Error en el servidor.

¿Cuales son los status code mas comunes para el verbo GET?

200 OK: Indica que la solicitud fue exitosa.
400 Bad Request: La solicitud es inválida.
401 Unauthorized: Falta autenticación.
403 Forbidden: La solicitud está prohibida.
404 Not Found: El recurso no fue encontrado.
500 Internal Server Error: Error en el servidor.

¿Cuales son los status code mas comunes para el verbo PUT?

200 OK: Indica que la solicitud fue exitosa.
201 Created: Indica que el recurso fue creado si este no existía.
204 No Content: Indica que la solicitud fue exitosa pero no hay contenido que devolver.
400 Bad Request: La solicitud es inválida.
401 Unauthorized: Falta autenticación.
403 Forbidden: La solicitud está prohibida.
404 Not Found: El recurso no fue encontrado.
500 Internal Server Error: Error en el servidor.

¿Cuales son los status code mas comunes para el verbo DELETE?

200 OK: Indica que la solicitud fue exitosa.
204 No Content: Indica que la solicitud fue exitosa pero no hay contenido que devolver.
400 Bad Request: La solicitud es inválida.
401 Unauthorized: Falta autenticación.
403 Forbidden: La solicitud está prohibida.
404 Not Found: El recurso no fue encontrado.
500 Internal Server Error: Error en el servidor.