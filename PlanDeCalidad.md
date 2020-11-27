# Plan de Calidad

## 1 Identificador del plan de prueba

El presente plan está identificado bajo el nombre clave QP-LICH-1.0

## 2 Referencias

No se han identificado referencias

## 3 Introducción

En el presente Plan de Calidad se delinearán los diversos elementos a ser probados, así como los riesgos identificables, las pruebas llevadas a cabo de dichas funciones, la estrategia general para la liberación, los criterios de aprobación y falla (considerando el diseño de métricas), así como los entregables de las pruebas, entre otras cosas. Tiene como propósito principal el establecer la pauta para la entrega del proyecto con un alto nivel de satisfacción, así como delinear las prácticas y métricas que serán usadas. 

De igual forma, se establecerá la estrategia general de revisiones, niveles de las mismas y proceso para asegurar la satisfacción de los usuarios finales. Para ello también será necesario asignar responsables de cada una de las tareas y, por supuesto, establecer aquellas funciones sobre las que se tendrán que realizar las demostraciones. 


## 4 Elementos de prueba (funciones)

Los siguientes elementos se van a probar:

• La funcionalidad correcta de la interfaz

• La funcionalidad de mandar mensajes y que se reciban correctamente

• La funcionalidad de crear grupos y mandar mensajes en ellos y que se reciban correctamente.

• La funcionalidad de foros y poder usarlos como se deben usar.

• La funcionalidad del API con Google Calender para crear y modificar eventos desde la aplicación

## 5 Riesgos del software

Los principales riesgos con la aplicación “ITAM Chat” están relacionados con la seguridad de los datos y conversaciones, así como con el uso de estos para una eventual optimización de su funcionamiento. Además, los chats son lugares que, en tanto que promueven una conversación entre dos personas en un ambiente semi controlado, pueden usarse de forma inapropiada. En concreto, los riesgos principales son los siguientes:

•	Que el software sea usado para agredir o acosar a estudiantes de la institución, activa o pasivamente.

•	Que alguna parte del flujo, o bien los repositorios de datos no sean lo suficientemente seguros para garantizar la privacidad y seguridad de los usuarios del mismo.

•	Que los datos compartidos sean usados sin el consentimiento de los usuarios para explotaciones de mercadotecnia, o compartidos ilegítimamente con otros partidos involucrados. 


## 6 Funciones por probar

Los siguientes puntos son las funcionalidades que hay que probar:

•	Funcionamiento de la interfaz.

•	Requests de información (query) de la base de datos del ITAM para buscar usuarios

•	Funcionamiento de iniciar sesión y cerrar sesión.

•	Mandar mensajes entre usuarios.

•	Creación de grupos por los usuarios.

•	Creación, modificación y eliminación de eventos desde ITAM Chat en Google Calendar.

•	Funcionamiento de mandar documentos entre usuarios.

•	Funcionamiento de los foros que sean visibles y accesible a todos los interesados.


## 7 Funciones que no deben probarse

Los siguientes puntos son las funcionalidades que todavía no hay que probar:

• Búsqueda de mensajes anteriores.

• Funcionamiento para que los usuarios se puedan salir del grupo.

• Funcionamiento para poder cerrar foros.


## 8 Estrategia

8.1 Descripción general

El acercamiento principal para llevar a cabo las pruebas será de específico a general. Esto es, se plantea que las funcionalidades se evalúen primero una por una, posteriormente en la integración entre ellas, y finalmente la aplicación en su totalidad.

Ahora bien, este proceso ha de llevarse a cabo tanto para control interno como para satisfacción del cliente. No obstante, si bien internamente sí se llevará a cabo la prueba de todas ellas, de forma externa se hará únicamente cuando existan cambios en la usabilidad de la aplicación, “visibles” para el cliente. Esto tiene como propósito tener un desarrollo ágil y veloz, sin perder de vista la retroalimentación y la satisfacción requeridas para que el proyecto cumpla con las expectativas. 
De esta forma, a nivel:

•	Funcionalidad: las pruebas serán conducidas por el desarrollador únicamente, y por el product manager, si el caso así lo requiere.

•	Integración: estas pruebas serán conducidas primero internamente por el product manager y posteriormente se le presentarán al cliente para que otorgue su retroalimentación. Una vez incorporada la retroalimentación del cliente, se procederá a realizar los cambios y luego la prueba general.

•	General: previo a la entrega del producto, se llevará a cabo una prueba general interna y posteriormente una con el cliente, quien podrá dar retroalimentación para posteriormente llevar a cabo hacer la entrega final.

Además, las etapas son incrementales. Esto es, no se podrá pasar al nivel “Integración”, sin previamente haber realizado y corregido todo lo necesario en la etapa de “Funcionalidad”; la misma relación existe entre el segundo y tercer nivel.

 8.2 Control de cambios
 
Se debe de mantener un ambiente de control de cambios estricto, con procesos establecidos para llevar a cabo los mismos, así como un registro y un historial de lo realizado. Esto permitirá, dado el caso, volver a versiones anteriores si así lo solicitan agentes externos, o bien si dadas las circunstancias, se decide que es el mejor camino para lograr los objetivos planteados. En cuanto a los niveles dos y tres de la sección 8.1, los cambios requerirán la aprobación del product manager, y en su caso del cliente. Para el nivel uno, los cambios podrán realizarse por el mismo desarrollador, sin consulta previa, siempre y cuando se haga la documentación requerida y ésta se entregue al product manager.

8.3 Reuniones

Se llevarán a cabo dos reuniones generales semanales, en martes y viernes, para monitorear el avance general. Además, se podrán establecer otras si así se considera pertinente.


## 9 Criterios de aprobación y falla

En cuanto a las funcionalidades de requiere, el criterio de aprobación es binario; es decir, 1 si funciona, o 0 si no funciona. En cuanto a la integración se refiere, habrá dos criterios, a saber: (a) el primero de ellos será binario, análogo al de las funcionalidades, y (b) el segundo será a discreción de product manager, quien habrá de verificar que se cumplan con las expectativas de interacción y calidad que se han prometido al cliente. Finalmente, para el último de los niveles, será el cliente quien establezca la decisión final de aprobación. 

## 10 Criterios para la suspensión y requerimientos de reanudación

El proyecto podrá suspenderse o retrasarse en caso de emergencia sanitaria, o en caso de que un miembro del equipo o de la familia inmediata de los mismos resulte afectado por la presente pandemia. 

También el proyecto se detendrá si por alguna razón el cliente se ve impedido de realizar las revisiones necesarias. En dicho caso, la reanudación se hará cuando se efectúen los VoBos necesarios y se obtenga la retroalimentación requerida.

## 11 Entregables de la prueba
El entregable debe ser un reporte detallando el grado de éxito de las pruebas propuestas. Por ejemplo, debe detallar el tiempo que duran las pruebas y si fueron llevaron a cabo su función correctamente. El reporte debe tomar en cuenta todas las pruebas propuestas y en caso de que una no funcione de manera adecuada.

## 12 Tareas de prueba restantes

A continuación se puede encontrar un listado de las pruebas que aún se tienen que hacer:

• Una prueba para que el usuario pueda buscar mensajes anteriores.

• Una prueba para probar que un usuario pueda salirse de un grupo en el que se encuentra.

• Una prueba para comprobar que el usuario pueda cerrar y borrar de su historial foros que ha abierto.

## 13 Necesidades ambientales

Para poder llevar a cabo las pruebas necesarias se requerirá:

•	Del acceso a la base de datos en modo sandbox para las funcionalidades iniciales y la integración.

•	Del acceso a la base de datos en modo producción para la revisión final

•	Tener una línea de comunicación con el cliente para compartir información, según lo requiera la situación.

•	Acceso a los servidores donde se almacena el código del sitio web actual.


## 14 Necesidades del personal

Para poder realizar las pruebas será necesario que los desarrolladores se apeguen a las prácticas aquí mencionadas, y que sigan las guías establecidas por el product manager. De igual forma, será vital tener comunicación con el representante establecido por el cliente para los niveles 2 y 3. 

## 15 Responsabilidades

A continuación se muestra una lista con las actividades y los responsables de cada una:

•	Aceptación final del proyecto (C y PM)
•	Testeo de las funcionalidades, a nivel individual (D)
•	Integración de funcionalidades, en un segundo nivel (D)
•	Revisión de la integración de funcionalidades, en un segundo nivel (PM)
•	Documentación de funcionalidades (D)
•	Documentación a nivel negocio (PM)


## 16 Agenda

La agenda para esté proyecto está planeado para que se pueda entregar antes de verano de 2021 para que se pueda probar durante ese periodo con una carga menor de usuarios. Los detalles de la agenda aún faltan de definir formalmente.

## 17 Planeación de riesgos y contingencias

Actualmente todo el equipo se encuentra laborando activamente en diversos proyectos, de modo que el PM podría demorarse en la revisión de algunas documentaciones y al momento de realizar las pruebas. Por ende, es importante preveer tales retrasos en los tiempos establecidos. De igual forma, el cliente generalmente tarda en realizar las revisiones correspondientes.

## 18 Aprobaciones

Product Manager ---------------------
Cliente ----------------------------

## 19 Glosario







