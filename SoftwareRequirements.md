# Software Requirements

## 1 Introducción
### Propósito
El producto que se presenta a continuación en este SRS es la aplicación de ITAM Chat, un programa que facilitaría la comunicación entre estudiantes y maestros que son parte de la comunidad ITAM. ITAM Chat crearía un medio a través del cual los estudiantes que pertenecen a una clase y el maestro que imparte dicha clase puedan comunicarse y organizarse sin necesidad de aplicaciones externas. Este SRS intentará describir el proyecto completo al igual que incluir tres funcionalidades del sistema.
### Convenciones del Documento
Convención | Definición
---------- | -----------
ITAM | Instituto Tecnológico Autónomo de México
1-3 | Se utilizará una escala de 1-3 para las funcionalidades del sistema donde 1 indica una funcionalidad con la más alta prioridad y 3 indica una funcionalidad con baja prioridad.

### Audiencia y Sugerencias al Leer 
Este SRS tiene como objetivo de audiencia a los desarrolladores que crearan y mantendrán la aplicación en el futuro. Se sugiere leer la introducción y la descripción general, y posteriormente utilizar los subtítulos para leer la sección que más sea de su interés.
### Alcance del producto
El software presentado es la aplicación de ITAM Chat que es una plataforma donde maestros y estudiantes de la comunidad ITAM se pueden comunicar entre ellos sin necesidad de aplicaciones exteriores. 

Metas de ITAM Chat:
- Crear una plataforma que facilite y agilice la comunicación entre estudiante y maestro que suele ser tardada utilizando el correo electrónico.
- Aumentar las interacciones que se tienen entre los estudiantes de una clase para fortalecer a la comunidad ITAM.
- Mejorar el rendimiento en general de los estudiantes al proveerles una plataforma donde pueden resolver dudas sobre materias.

## 2 Descripción General
### Perspectiva del Producto
ITAM Chat nace de la necesidad que surge cada semestre de comunicar de manera eficiente a los estudiantes entre ellos y a los estudiantes con los maestros. Esta aplicación seria un producto nuevo que solo reemplazaría al correo electrónico como vía principal de comunicación. ITAM Chat sería parte de Comunidad ITAM, para facilitar el acceso a la aplicación por parte de la comunidad.
### Funciones del Producto
- Tener un chat entre estudiante dentro de una clase.
- Establecer un chat entre todos los estudiantes y el maestro de una clase.
- Tener un chat privado entre cada estudiante y el maestro.
- Crear un foro donde se puedan subir preguntas y comentarios para que el maestro u otros estudiantes puedan contestar.
- Poder conectar integrantes de un equipo con facilidad.
### Clases y Características del Usuario.
Usuario | Descripción
------- | -----------
Estudiantes | Los estudiantes serán los principales usuarios de la plataforma ya que necesitarán comunicarse entre ellos y con los profesores constantemente. La aplicación los debe permitir crear subgrupos con otros estudiantes, recibir y mandar mensajes a estudiantes y maestros y finalmente checar y subir cosas al foro.
Maestros | Los maestros verán dentro de la aplicación los diversos grupos que tienen y podrán crear subgrupos, recibir y mandar mensajes, interactuar con el foro y adicionalmente podrán entregar calificaciones y reportar estudiantes por mala conducta.
Administrativos | Los administrativos tienen control completo sobre la aplicación en caso de que se necesite cambiar ciertos elementos o mover gente de grupos. Los administrativos son los que menos usarán la plataforma pero la mantendrán de pie.
### Ambiente de operación
ITAM Chat funcionará sobre cualquier navegador ingresando a Comunidad y picando la liga hacia ITAM Chat Web. Adicionalmente la aplicación estará disponible en el App Store y Google Store para su uso móbil.
### Limitaciones de Implementación y Diseño
ITAM Chat tiene las siguientes limitaciones
- Los datos utilizados por la aplicación deben de ser controlados completamente por el ITAM.
- El ITAM se encargará de el mantenimiento del software.
- Tiene que haber un límite de los tipos de mensajes que se pueden mandar y el tamaño de los archivos.
### Documentación
- ITAM Chat tendrá una sección de FAQ donde los estudiantes podrán recurrir para resolver dudas sobre como utilizar la aplicación.
- Los ingenieros encargados de mantener el programa estarán completamente capacitados para responder preguntas.
- Comunidad ITAM tendrá un pequeño manual sobre cómo utilizar ITAM Chat.
### Supuestos y Dependencias
- La cantidad de usuarios que utilizaran la plataforma no puede pasar cierto límite.
- El programa al igual que su backend será mantenido de forma adecuada.
- Se asume que los usuarios de ITAM Chat son miembros de la comunidad ITAM y tienen cuenta para poder ingresar.

## 3 Requerimientos de Interfaces Externas
### Interfaces de Usuario

### Interfaces del Hardware
- **Dispositivos Móviles:** ITAM Chat funcionará dentro de los dispositivos móviles donde tendrá la mayoría de usuarios. En este hardware la aplicación tendrá pantallas más pequeñas por lo que habrán ventanas dentro del programa con menos opciones pero se podrá ver y hacer todo, nada más que de manera reducida.
- **Navegador Web:** ITAM Chat adicionalmente va a funcionar sobre un navegador web si es que se necesita acceder a través de una computadora. La aplicación en el navegador web tendrá ventanas con muchas más opciones que elegir y sería inevitablemente más cómodo usarlo.
### Interfaces de Software
La aplicación necesitaría una conexión con una base de datos donde mandaría los mensajes que se están enviando y guardaría dichos mensajes para desplegar las conversaciones que se estén haciendo. En cuanto a la seguridad, los datos del alumno que se guarden tienen que ser limitados y guardados con un alto nivel de seguridad en la base de datos. La aplicación mandaría como output los mensajes que escribe el usuario y como input los mensajes que le están mandando a dicho usuario o al grupo al cual el pertenece.
### Interfaces de Comunicación
Principalmente se ingresará a la aplicación a través de el correo de la institución por lo que ITAM Chat debe de tener una comunicación con el servicio del correo electrónico. Adicionalmente en cuanto a seguridad, los mensajes y la información mandada será encriptada.

## 4 Funcionalidades del sistema
### 4.1 Crear grupos de chat
#### 4.1.1 Descripción y prioridad
Esta funcionalidad se refiere a la habilidad que tendrán los estudiantes de poder crear grupos de chat con otros estudiantes donde los mensajes solo serán visibles a los integrantes del grupo. Esta funcionalidad tiene prioridad 1 porque es vital para una aplicación de chat poder crear grupos y equipos de trabajo.
#### 4.1.2 Secuencias de Estímulo/Respuesta
Estímulo | Respuesta
-------- | ---------
Un usuario seleccionara la opción de crear grupo | La aplicación le brindará una ventana con todos los estudiantes donde podrá elegir quien es integrante del grupo.
#### 4.1.3 Requerimientos funcionales
- **REQ-1:** Acceso a la base de datos con los nombres de todos los alumnos para poder elegir cual meter al grupo.
- **REQ-2:** Un nivel de seguridad donde ninguna persona fuera del grupo pueda acceder a los mensajes dentro del grupo.

### 4.2 Buscar a un alumno o profesor 
#### 4.2.1 Descripción y prioridad
Esta funcionalidad se refiere a la búsqueda de alumnos o profesores de la comunidad ITAM para poder comunicarse con cualquier integrante de la comunidad ITAM. Este tiene una prioridad 1 ya que es esencial que los usuarios puedan comunicarse con quien quieran. 
#### 4.2.2 Secuencias de Estímulo/Respuesta
Estímulo | Respuesta
-------- | ---------
La aplicación tendrá una barra de búsqueda donde podrá ingresar el nombre o clave única de un usuario | La aplicación regresará una ventana con los resultados y la opción de empezar un chat con cualquiera de los usuarios en el resultado.
#### 4.2.3 Requerimientos funcionales
- **REQ-1:** Acceso a la base de datos con los nombres y claves únicas de todos los alumnos y profesores usuarios de la plataforma.
- **REQ-2:** Debería ser posible crear chats privados con cualquier usuario.

### 4.3 Ingresar a la aplicación
#### 4.3.1 Descripción y prioridad
Esta funcionalidad se refiere a la habilidad y la ventana necesaria para poder ingresar a la aplicación. Esta funcionalidad se encarga de checar que los datos ingresados estén correctos para permitir que el usuario ingrese. Esta tiene una prioridad de 1 ya que sin esta funcionalidad no se puede utilizar la plataforma.
#### 4.3.2 Secuencias de Estímulo/Respuesta
Estímulo | Respuesta
-------- | ---------
El usuario ingresará sus datos dentro de unos inputs localizados en una ventana de inicio de sesión | La aplicación mandara un query a la base de datos para verificar que los datos ingresados corresponden a un usuario válido.
#### 4.3.3 Requerimientos funcionales
- **REQ-1:** El programa debe de tener una manera de verificar correos y usuarios.
- **REQ-2:** Los usuarios deben de estar afiliados y registrados en el sistema de correos del ITAM.
- **REQ-3:** Los datos del usuario serán encriptados cuando se manden o se reciban.

### 4.4 Subir preguntas al foro de una clase
#### 4.4.1 Descripción y prioridad
ITAM Chat tendrá una sección que sea el foro de una clase donde un alumno pueda subir preguntas acerca de la materia y el profesor u otro alumno pueda responder. Esta funcionalidad se debe encargar que sea posible subir una pregunta al foro y que sea visible a los demás. Es de prioridad 2 porque es parte de un feature importante pero sin el foro la aplicación sigue funcionando.
#### 4.4.2 Secuencias de Estímulo/Respuesta
Estímulo | Respuesta
-------- | ---------
El usuario ingresará a la pestaña de foros, buscara el foro de su clase, escribirá su pregunta y oprimirá un botón de subir | La aplicación recibirá la pregunta y la desplegará en la ventana del foro.
#### 4.4.3 Requerimientos funcionales
- **REQ-1:** Esta funcionalidad requiere de una ventana para desplegar la pregunta subida al foro.

### 4.5 Conectar al calendario para agendar eventos 
#### 4.5.1 Descripción y prioridad
Esta funcionalidad permitirá a usuarios agendar eventos con otros usuarios como citas, sesiones de estudios, trabajos en equipo etc. Adicionalmente la aplicación se conectará a Google Calendar para automáticamente crear el evento y agregarlo. Este tiene prioridad 3 porque no es esencial para el funcionamiento del programa pero sería una funcionalidad muy útil.
#### 4.5.2 Secuencias de Estímulo/Respuesta
Estímulo | Respuesta
-------- | ---------
Dentro de un chat habra la opción de agendar un evento | La aplicación automáticamente asumira que el evento será con los integrantes del chat y mandará una instancia del evento a Google Calendar para que lo registre. 
#### 4.5.3 Requerimientos funcionales-
- **REQ-1:** Requiere una conexión a través de un API a Google Calendar.
- **REQ-2:** Requiere que los usuarios tengan Google Calendar conectado al dispositivo donde estén utilizando ITAM Chat.
- **REQ-3:** Requiere que la aplicación pueda informar a otros usuarios de eventos creados que los incluyen a ellos.

## 5 Otros Requerimientos No Funcionales
### Requerimientos Operacionales
Los requerimientos para que la aplicación funcione como debe de funcionar se reduce al desempeño y el límite de carga que permitan los servidores que respaldan a la aplicación. Estos deben de poder resistir el uso de alrededor de 6000 usuarios que serían los integrantes de la comunidad ITAM.
### Requerimientos de Protección
Los daños que podría causar la aplicación por su naturaleza son principalmente relacionados al acoso o la agresión que se puede producir a través de una aplicación que permite la comunicación. Los requerimientos para poder proteger ante dichos incidentes sería que la aplicación implemente medidas de seguridad donde se pueda reportar comportamiento de esta índole para eliminar cualquier agresión o acoso. 
### Requerimientos de Seguridad
ITAM Chat se encargara de salvaguardar los datos con los que trabaja a través de varios requerimientos que tomará como regla
- Cuando un usuario ingrese su información dentro de la aplicación esta sera encriptada cuando se manda al servidor para validar.
- Las conversaciones estarán encriptadas para evitar que se expongan.
- Las bases de datos que contengan toda la información sensible será protegida de manera adecuada. 
### Atributos de Software de Calidad
Algunos atributos a considerar para ITAM Chat son
- **Adaptabilidad:** ITAM Chat debería ser accesible desde la mayoría de los dispositivos y todos los navegadores en los que se acceda.
- **Mantenibilidad:** La plataforma debe de incluir un 'toolkit' o portal especial donde los administradores puedan completar las tareas administrativas del sistema y darle mantenimiento.
- **Confiabilidad:** La aplicación será diseñada de modo que en caso de que ocurra un problema, el 'downtime' del sistema sea imperceptible. Sin embargo, si el problema es grande y no se logra reanudar rápidamente la funcionalidad de ITAM Chat, la información será guardada de manera adecuada.
- **Usabilidad:** El UI de la aplicación será amistosa y tendrá una interfaz intuitiva para dar la mínima cantidad de problemas al utilizarlo. Adicionalmente tomará en cuenta a todos los dispositivos para que la aplicación sea usable sin importar el dispositivo en el que la veas.
### Reglas del Negocio
Se debe de considerar el tema de la privacidad de información entonces se restringirá la información que es visible para los estudiantes al igual que los maestros. La información personal del estudiante no será visible y los demás usuarios sólo podrán ver lo que les podría interesar, nada más ni nada menos. Adicionalmente los usuarios tendrán un contacto con los administradores de la aplicación si por alguna razón necesiten ayuda en un problema que ponga en peligro su seguridad.

