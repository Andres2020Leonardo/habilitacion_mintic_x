# habilitacion_mintic_x
habilitacion ciclo 3
# Andres eonardo Muñeton Escobar
HABILITACIÓN - Sprint 6
CICLO 3
1. Título: Creación de una aplicación web de ventas
2.Modalidad: Célula de desarrollo (Trabajo en equipo o individual 
previamente validado con el equipo de permanencia)
3.Resultado de aprendizaje: Se espera que, al finalizar la 
actividad los estudiantes conozcan cómo desarrollar y desplegar sitios 
web en un entorno Cloud.
4.Recursos: Para lograr acceder a la información, deben ir a los 
documentos correspondientes a cada una de las semanas del Ciclo 3, 
como son el material de estudio y el material de apoyo, para ver los 
tutoriales y las guías que allí se presentan. 
5.Indicaciones: 
● Creen un equipo de trabajo para el desarrollo de las historias de usuario 
del proyecto y asígnenle un nombre.
● Asignen los diferentes roles para la ejecución del sprint. Estos roles están 
definidos en la siguiente tabla:
Rol Función del rol 
1. Desarrollador Generar las fuentes para el frontend y el backend
2. Analista Levantar las necesidades del negocio para convertirlas en 
requerimientos del sistema 
3. Product Owner Conocer el producto software que se va a elaborar en el 
proyecto 
4. Administrador de BD Gestionar y disponer el motor de base de datos para el 
proyecto de desarrollo de software
5. Scrum master Gestionar todas las ceremonias y actividades de la 
metodología Scrum, y asignar los recursos a cada rol
● Cada integrante debe aportar a las actividades correspondientes para 
desarrollar y desplegar el proyecto dado, estas actividades se derivan de 
las historias de usuario descritas más adelante, siguiendo las 
instrucciones en el apartado de recursos.
6. ¿Cuál es el proyecto a desarrollar?
Planteamiento de la situación problema a desarrollar 
Se propone analizar, diseñar, construir y desplegar una aplicación de 
software que permita realizar el seguimiento de las ventas de un producto 
y/o servicio en una empresa (Los equipos que ya tenían acordado con un 
tutor el tipo de producto y/o servicios que ofrece la empresa, continúan 
trabajando con ese tipo de productos; para los equipos que apenas 
comenzarán el desarrollo, deben definir ellos mismos el tipo de producto 
que ofrece la empresa para la que desarrollarán el sistema de 
información).
Nota: La empresa de la que se habla es una empresa 
hipotética/inventada (No es real).
7. ¿Qué debo alcanzar para desarrollar la 
aplicación web? 
Realizar el seguimiento de las ventas requiere la construcción de unas 
interfaces de usuario que permitan: el ingreso a la aplicación, registro de 
productos, maestro de productos, registro de venta, maestro de las 
ventas y maestro de usuarios.
Para que puedas desarrollar el proyecto que se te planteó, la aplicación 
web debe contar con los siguientes módulos: 
● Gestión de ingreso al sistema de información. El sistema tendrá 
una interfaz gráfica para el ingreso a la aplicación (registro e inicio de 
sesión), la autorización de ingreso a la aplicación estaría a cargo de un 
tercero (Gmail) mediante “Oauth 2”; todos los usuarios que se 
registran entran en estado pendiente.
● Módulo administrador de productos. El sistema tendrá una interfaz 
gráfica para el registro de productos y otra para listar, buscar y 
actualizar productos, cada uno debe contar con los siguientes 
atributos: Identificador único (Inmutable), descripción, valor unitario 
y estado (disponible, no disponible).
● Módulo administrador de ventas. El sistema tendrá una interfaz 
gráfica para el registro de las ventas y otra para listar, buscar y 
actualizar las ventas realizadas (Actualizar se refiere a establecer los 
diferentes estados de la venta: En proceso, cancelada o entregada, o 
editar alguno de sus otros campos modificables). Cada venta debe 
contar con los siguientes atributos: Identificador único de venta 
(Inmutable), el valor total de la venta, identificador, cantidad y precio 
unitario de cada producto, fecha de venta, el documento de 
identificación y nombre del cliente, y, además, deberá contar con un 
encargado de gestionar dicha venta (vendedor).
● Gestión de usuarios. Permite ver y actualizar el rol (administrador y 
vendedor) y el estado del usuario (pendiente/autorizado/no 
autorizado)
8.Precisiones. 
1. Se requiere que el proyecto cumpla con las historias de usuario 
presentadas en este documento, pero se da libertad para que el 
equipo de desarrollo pueda acordar realizar cualquier 
funcionalidad adicional.
2. No se requiere módulo de inventario, clientes o uno diferente a los 
que se presenta anteriormente. 
3. No se requiere contemplar impuestos o valores adicionales en la 
venta.
4. La palabra usuario es usada en el contexto del proyecto como una 
persona cualquiera que se registra en su aplicativo web, esta 
puede ser alguien que no tiene relación con la empresa, por lo que 
por defecto el usuario tiene estado pendiente y no tiene rol, dicha 
persona solo podrá ingresar a la aplicación exitosamente cuando 
el administrador le cambie el estado a autorizado y le asigne un rol. 
El administrador tiene acceso total a la aplicación, mientras que el 
vendedor únicamente a las interfaces de usuario correspondientes 
a la de registro y maestro de ventas. 
9.Arquitectura de la solución propuesta para el 
proyecto final
10. Product backlog (Historias de usuario) 
Feature: como analista/desarrollador requiero crear todo el entorno 
necesario para el manejo de la Gestión de la configuración, tanto en el 
equipo local como en el repositorio GitHub, para administrar todos los 
artefactos que se generan durante el proceso de desarrollo de software.
Historia de usuario: HU_001
Dado una herramienta para administrar las fuentes/artefactos en la nube
Cuando necesite crear un repositorio con mi propia cuenta
Entonces dispondré de un lugar en GitHub para almacenar la 
información/artefactos/fuentes de los proyectos de desarrollo
Historia de usuario: HU_002
Dado que tengo un repositorio de GitHub en la nube
Cuando necesite subir artefactos
Entonces podré tener artefactos ordenados en GitHub con la información 
del proyecto
Historia de usuario: HU_003
Dado que tengo instalado la aplicación Git en la máquina local
Cuando requiera enlazar un directorio con un repositorio en GitHub
Entonces podré subir nuevos artefactos al repositorio en GitHub
Historia de usuario: HU_004
Dado que tengo instalado la aplicación Git en la máquina local
Cuando requiera enlazar un directorio con un repositorio en GitHub
Entonces podré subir artefactos actualizados al repositorio en GitHub
Feature: Como vendedor o administrador necesito administrar la 
información de las ventas para gestionar la información del día a día.
Historia de usuario: HU_005
Como usuario
Dado que voy a ingresar al sistema de gestión de ventas
Cuando necesite validar mis credenciales
Entonces podré ver las opciones para ingresar mediante Gmail
Historia de usuario: HU_006
Como vendedor o administrador
Dado que ingreso al sistema de ventas
Cuando necesite registrar una venta
Entonces podré ingresar los datos relacionados a una venta
Historia de usuario: HU_007
Como vendedor o administrador
Dado que ingreso al sistema de ventas
Cuando registre una venta
Entonces podré ver que se almacenó correctamente
Historia de usuario: HU_008
Como vendedor o administrador
Dado que ingreso al sistema de ventas
Cuando requiera listar la información de las ventas
Entonces podré ver la información de las ventas realizadas
Historia de usuario: HU_009
Como vendedor o administrador
Dado que ingreso al sistema de ventas
Cuando requiera verificar o actualizar la información de las ventas 
registradas en el sistema
Entonces podré realizar una búsqueda mediante el identificador de la 
venta, documento de identidad del cliente o nombre del cliente en la 
información de las ventas registradas en el sistema.
Historia de usuario: HU_010
Como vendedor o administrador
Dado que ingreso al sistema de ventas
Cuando requiera actualizar la información de las ventas
Entonces podré editar la información de la venta que deseo actualizar 
(Menos el identificador de la venta).
Historia de usuario: HU_011
Como vendedor o administrador
Dado que ingreso al sistema de ventas
Cuando actualice una venta
Entonces podré ver que se almacenó correctamente
Historia de usuario: HU_012
Como administrador
Dado que ingreso al sistema de ventas
Cuando necesite registrar un producto
Entonces podré ingresar los datos relacionados a un producto
Historia de usuario: HU_013
Como administrador
Dado que ingreso al sistema de ventas
Cuando registre un producto
Entonces podré ver que se almacenó correctamente
Historia de usuario: HU_ 014
Como administrador
Dado que ingreso al sistema de ventas
Cuando requiera listar la información de los productos
Entonces podré ver la información de los productos
Historia de usuario: HU_015
Como administrador
Dado que ingreso al sistema de ventas
Cuando requiera verificar o actualizar la información de los productos 
registrados en el sistema
Entonces podré realizar una búsqueda mediante el identificador del 
producto o descripción del producto en la información de los productos 
registrados en el sistema.
Historia de usuario: HU_016
Como administrador
Dado que ingreso al sistema de ventas
Cuando requiera actualizar la información de los productos
Entonces podré editar la información del producto que deseo actualizar 
(Menos el identificador del producto)
Historia de usuario: HU_017
Como administrador
Dado que ingreso al sistema de ventas
Cuando actualice un producto
Entonces podré ver que se almacenó correctamente
Historia de usuario: HU_018
Como administrador
Dado que ingreso al sistema de información de ventas
Cuando requiera listar la información de los usuarios del sistema
Entonces podré ver la información de los usuarios
Historia de usuario: HU_019
Como administrador
Dado que ingreso al sistema de información de ventas
Cuando requiera actualizar la información de los usuarios del sistema
Entonces podré editar la información de los usuarios del sistema que 
deseo actualizar (Estado y rol)
Historia de usuario: HU_020
Como administrador
Dado que ingreso al sistema de ventas
Cuando actualice el estado o rol de un usuario
Entonces podré ver que se almacenó correctamente
Feature: Como usuario del sistema requiero ingresar a la aplicación de 
ventas desplegada en la nube dado la URL de la aplicación de ventas.
Historia de usuario: HU_021
Dado que quiero ingresar a la aplicación de ventas mediante un 
navegador
Cuando intente ingresar a la aplicación mediante una URL
Entonces podré interactuar con la aplicación web
11. Metodología Scrum:
● Con la metodología Scrum debes realizar entregas parciales y regulares 
del producto final. Las actividades se priorizan de acuerdo a las 
necesidades para lograr la entrega de un producto completo.
● Para llevar a cabo dichas entregas, debes primero registrar los objetivos 
trazados por cada integrante del equipo según las historias de usuario 
dadas, para lo cual se empleará el programa Trello. De igual forma, todos 
los días se deben reunir los integrantes de manera virtual para realizar 
la ceremonia del Daily, que es una reunión de 15 minutos en la que cada 
uno de los integrantes deberá responder las siguientes preguntas: 
o ¿Qué hiciste ayer?
o ¿Qué harás hoy?
o ¿Hay impedimentos en tu camino? (blockers)
● NOTA: Para la nota de la habilitación no se tendrá en cuenta el 
registro de los Dailies en los formularios usados durante el 
ciclo, aún así se recomienda realizar esta ceremonia para que 
el equipo se coordine en el desarrollo del proyecto planteado. 
● Esta entrega recibirá una nota que será el soporte para la certificación, 
pero, aunque el trabajo sea grupal, la nota será de manera individual. 
12. Criterios de valoración de la evidencia:
Debes entregar la URL para acceder al sistema de ventas desplegado en 
la nube. Esta actividad tiene un valor del 100% y debes entregarla en la 
semana 9 (Primera semana del ciclo 4). 
13. Protocolo de entrega
1) Formato: El documento a entregar debe contener de lo 
siguiente:
● Portada con los nombres de los integrantes del equipo
● Descripción del proceso que se llevó a cabo para cumplir con 
los requerimientos de este sprint
● Evidencia de la funcionalidad de aplicación (pantallazos)
Se requiere compartir el enlace de Trello, en el que se deberán 
evidenciar los diferentes aportes de cada uno de los integrantes 
del proyecto. 
Debes nombrar el archivo entregado indicando 
Sprint6_Equipo_XX, (XX depende del nombre que le asignaron al 
equipo).
2) Medio
● Recurso tarea (Sprint 6), disponible en el aula virtual, semana 
7, en la plataforma Moodle.
3) Plazo máximo de entrega
● De acuerdo con el cronograma de actividades (Domingo 7 de 
noviembre, hasta las 23:59).
