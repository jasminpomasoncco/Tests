
 Feature: HU35: Como usuario, al retirarme de la sesión quiero que se me dé una función opcional para poder observar todas las actividades realizadas por mí durante el tiempo en el que estuve dentro de la app.
Scenario: E69: Cargar historial de actividades.

CA74:
	Given  que el paciente ha ingresado a la aplicación correctamente y realizo sus actividades 
	When  el paciente ingrese a la opción de “Historial” en el menú de opciones 
	Then  el aplicativo mostrara las actividades que realizo el paciente anteriormente y el paciente podrá hacer uso de buscar por fecha o nombre de la actividad según la preferencia del paciente 

Examples:
	| menu de opciones  |caja de mensajes                             | lista de actividades                         |
	| "historial"       | "usted realizo está lista de actividad hoy" | 1.  Jugar Ludo  Lunes a las 5:34 pm a 7:00 pm|

Scenario: E70: Buscar por fecha 

CA75:
	Given  que el paciente se encuentra en la opción de “Historial” y haga click en “Buscar por fecha”
	When  el paciente elija un rango de hora
	Then  el aplicativo automáticamente las actividades realizadas en ese rango.

Examples:
	| menu de opciones  | opción de historial    | caja de mensaje   |
	| "historial"       | "buscar por fecha"     |  "20/11/2021"     |

Scenario: E71: Buscar por nombre de la actividad 

CA76:
	Given  que el paciente se encuentra en la opción de “Historial” y  haga click en “Buscar por nombre de la actividad”
	When  el paciente escriba el nombre de la actividad 
	Then  se listara la fecha en la que realizo esa actividad. 

Examples:
    | menu de opciones  | opción de historial                   | caja de mensaje   |
	| "historial"       | "buscar por nombre de la acitividad"  |  "Ludo"          |
	Feature: HU09: Como usuario, quiero llamar a mis amigos de la app para dialogar de mi situación actual.
Scenario: E23: Llamar a amigos
CA27
    Given me encuentro en el chat personal
    When seleccione el botón de llamar
    Then el sistema reconocerá que quiero realizar una llamada y me redireccionará al formulario de llamada
Examples:
    | usuario | boton para llamar a amigos | pestaña de inicio de llamada |
    | mt322 | se hace clic | se inicia la llamada |

Scenario: E24: Cancelar llamada a un amigo
CA28
    Given dentro de la aplicación
    When mi amigo me llama y presiono el botón "No contestar"
    Then el sistema reconocerá que estoy rechazando la llamada y se cerrará la pestaña 
Examples:
    | usuario | boton para cancelar llamadas | pestaña de inicio de llamada   |
    | mt322   | "No contestar"               | "Usted ha cancelado la llamada |


Feature: HU15: Como paciente, quiero tener la opción de añadir amigos cuando juego para tener un grupo de apoyo en mis crisis.
Scenario: E33: Agregar amigos
CA37
    Given me encuentro en el juego de la app
    When seleccione el botón “+”
    Then añadiré al usuario con el que estoy jugando e interactuando como amigo
Examples:
    | usuario | perfil de usuario | boton para añadir amigos |
    | mt322 | se observa el perfil | se envia solicitud de amistad |

Scenario: E34: Eliminar amigos
CA38
    Given me encuentro en el juego de la app
    When seleccione el botón “-”
    Then eliminare al usuario con el que estoy jugando como amigo.
Examples:
    | usuario | perfil de usuario | boton para eliminar amigos |
    | mt322 | se observa el perfil | se retira al seleccionado de la lista de amigos |
    Feature: HU19: Como usuario, quiero tener la opción de reclamar a los administradores en caso vea contenido inapropiado para que la app no muestre ese tipo de contenido a otros usuarios.
Scenario: E38: El usuario encuentra contenido inapropiado
CA42
    Given me encuentro usando la app
    When me encuentro algo bizarro
    Then reportaré y reclamaré para que dicho contenido no vuelva a aparecer
Examples:
    | usuario | pestaña de la publicación inapropiada | boton para reportar publicación |
    | mt322 | se observa la publicación | se reporta la publicación |

Scenario: E39: El psicólogo encuentra contenido inapropiado o información fraudulenta
CA43
    Given me encuentro revisando la app
    When me encuentro algo inapropiado o con información engañosa
    Then denunciaré a dicha persona y reportaré la información inapropiada
Examples:
    | usuario | pestaña de la publicación inapropiada | boton para denunciar publicación |
    | mt322 | se observa la publicación | se denuncia la publicación |

Feature: HU16:Como paciente, quiero un botón de pánico para recibir ayuda psicológica en el momento que tenga una crisis.
Scenario: E33: Paciente en crisis
CA37
    Given me encuentro en una crisis debido a mi problema psicológico
    When presione el botón de pánico de la app
    Then el sistema me comunicara con psicólogo especialista para estos casos
Examples:
    | usuario | pestaña para aplicar el botón | boton de pánico |
    | mt322 | se observa el botón y lo que implica presionarlo | se presiona el botón y se muestra que fue presionado en el perfil |

Scenario: E34: Psicólogo queriendo ayudar
CA38
    Given hay un paciente en crisis. 
    When el psicólogo esté dentro de la app. 
    Then habrá un apartado donde se verá que personas necesitan ayuda rápida
Examples:
    | usuario | pestaña de usuarios en crisis | boton de ayuda |
    | mt322 | se observa el usuario que se quiere ayudar | se presiona el botón y se le avisa al usuarion en crisis |

Feature: HU24:Como usuario, quiero tener la opción de ver el horario que dispone cada psicólogo para elegir el horario que más se acomode a mi tiempo.
Scenario: E46: Cargar lista de psicólogos disponibles.

C51: 
	Given que el paciente ha ingresado a la aplicación correctamente. 
	When el paciente ingrese a la opción de “Agenda” en el menú de opciones 
	Then  el aplicativo mostrara los horarios disponibles de cada psicólogo Y el paciente podrá hacer uso de buscar por horario o psicólogo según la preferencia del paciente 
Examples: 
	| Opción de menú de opciones | opción buscar                    |  caja de mensaje                 |
	| "agenda"                   | " buscar hoararios disponibles " | "horario libre hoy a las 4:00pm" |

Scenario: E47: Buscar por horario 

C52: 
	Given que el paciente se encuentra en la opción de agenda Y haga click en “Buscar por horario”. 
	When el paciente elija un rango de hora para la cita. 
	Then el aplicativo automáticamente listara los horarios disponibles en los que se hará el posible registro de cita.

Examples:
	| opción de menú       |                     caja de mensaje                          |
	| "buscar por horario" | " el psicólogo Juan Ramirez está disponible en este horario" |


Scenario: E48: Buscar por psicólogo 

C53: 
	Given  que el paciente se encuentra en la opción de agenda y haga click en “Buscar por nombre del psicólogo”.
	When  el paciente escriba el nombre del psicólogo. 
	Then  se listará los horarios disponibles del psicólogo seleccionado.
Examples:
	| opción de menu                   | caja de texto   |           caja de mensaje                   |
	| "buscar por nombre de psicólogo" | "Juan Ramirez"  | "el psicólogo Juan Ramirez está disponible" |


Feature: HU32: Como usuario, quiero que la aplicación me permita ordenar mis notificaciones para organizarlas en un rango de importancia, por ejemplo, las notificaciones de sesiones psicológicas.
Scenario: E61: recibir notificaciones de sesiones psicológicas

CA66:
	Given  que no me encuentro en la app 
	When tenga alguna sesión programada
	Then  el usuario recibirá un recordatorio de la sesión en la sección de notificaciones.  
Examples:
	| sesión programada        |                    caja de mensaje                   |
	| cita hoy a las 10:00 am  | "usted tiene una cita programada a las 10:00 pm "    |
  
Scenario: E62: recibir notificaciones de los videojuegos de la aplicación

CA67:
	Given  que no me encuentro en la app
	When tenga algún comentario de juegos
	Then  me llegará un mensaje   
Examples:
	| comentario             | caja de mensaje |
	|      "que buen juego"  | "usted tiene un comentario nuevo" |


Scenario: E63: recibir notificaciones priorizadas

CA68:
	Given  que no me encuentro en la app 
	When tenga  sesiones o actualizaciones pendientes
	Then  me llegará un mensaje y mis notificaciones se priorizarán por importancia 
 
Examples:
    | sesión programada        |                    caja de mensaje                 | lista de notificaciones                | 
	| cita hoy a las 10:00 am  | "usted tiene una cita programada a las 10:00 pm "  | Citas de psicología  Importancia: Muy Alta |
    Feature: HU17:Como psicólogo, quiero dar una atención especializada con recursos tecnológicos proporcionados por la app para una mejor atención 
Scenario: E35: Sugerencias de recursos tecnológicos de parte de los psicólogos

CA39: 
    Given que me encuentro dando sesiones psicológicas individuales .
    When culmine la sesión al presionar el botón de sugerencias. 
    Then podré sugerir a los desarrolladores agregar nuevos recursos o artefactos para las sesiones
Examples:
    | boton de sugerencias | caja de texto para mandar mensaje |
    | "Dejar sugerencias"  | "escriba aquí su sugerencia "      |


Feature: HU23:Como usuario, quiero tener una tabla de horarios para ver, programar y archivar los horarios de mi vida cotidiana, ya que a veces hay eventos recientes que no son tomados en cuenta para mi horario. 
Scenario: E44: Querer construir un horario

CA39: 
    Given  Dado que tengo muchas cosas pendientes para hacer. 
    When quiera organizarme mejor.
    Then crearé eventos dentro de mi horario en la app.
Examples:
    | boton de horario  |  caja de texto                 |
    | "crear actividad" | "examen el lunes a las 7:00 am"|

Scenario: E45: Eventos súbitos e imprevistos
CA50: 
    Given que a veces suceden cosas imprevistas tendré nuevas cosas para hacer
    When  tenga nuevos eventos para hacer
    Then crearé dichos eventos dentro de mi horario en la app

Examples:
    | boton de horario    |  botón    | caja de texto|
    | "agregar actividad" | "+"       | "examen el lunes a las 10:00 am"|
