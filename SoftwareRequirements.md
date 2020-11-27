# Software Requirements

## 1 Introducción
### Propósito
El producto que se presenta a continuación en este SRS es la aplicación de ITAM Chat, un programa que facilitaría la comunicación entre estudiantes y maestros que son parte de la comunidad ITAM. ITAM Chat crearía un medio a través del cual los estudiantes que pertenecen a una clase y el maestro que imparte dicha clase puedan comunicarse y organizarse sin necesidad de aplicaciones externas. Este SRS intentará describir el proyecto completo al igual que incluir tres funcionalidades del sistema.
### Convenciones del Documento
Convención | Definición
---------- | -----------
ITAM | Instituto Tecnológico Autónomo de México


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
- Poder desplegar calificaciones y trabajos que se necesitan entregar.
- Poder conectar integrantes de un equipo con facilidad.
### Clases y Características del Usuario.
Usuario | Descripción
------- | -----------
Estudiantes | Los estudiantes serán los principales usuarios de la plataforma ya que necesitarán comunicarse entre ellos y con los profesores constantemente. La aplicación los debe permitir crear subgrupos con otros estudiantes, recibir y mandar mensajes a estudiantes y maestros y finalmente checar y subir cosas al foro.
Maestros | Los maestros verán dentro de la aplicación los diversos grupos que tienen y podrán crear subgrupos, recibir y mandar mensajes, interactuar con el foro y adicionalmente podrán crear tareas, entregar calificaciones y reportar estudiantes por mala conducta.
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
#### 4.1.2 Secuencias de Estímulo/Respuesta
#### 4.1.3 Requerimientos funcionales

### 4.2 Buscar a un alumno o profesor 
#### 4.2.1 Descripción y prioridad
#### 4.2.2 Secuencias de Estímulo/Respuesta
#### 4.2.3 Requerimientos funcionales

### 4.3 Ingresar a la aplicación
#### 4.3.1 Descripción y prioridad
#### 4.3.2 Secuencias de Estímulo/Respuesta
#### 4.3.3 Requerimientos funcionales

### 4.4 Subir preguntas al foro de una clase
#### 4.4.1 Descripción y prioridad
#### 4.4.2 Secuencias de Estímulo/Respuesta
#### 4.4.3 Requerimientos funcionales

### 4.5 Conectar al calendario para agendar eventos 
#### 4.5.1 Descripción y prioridad
#### 4.5.2 Secuencias de Estímulo/Respuesta
#### 4.5.3 Requerimientos funcionales

## 5 Otros Requerimientos No Funcionales
### Requerimientos Operacionales
### Requerimientos de Protección
### Requerimientos de Seguridad
### Atributos de Software de Calidad
### Reglas del Negocio

## 6 Otros Requerimientos
