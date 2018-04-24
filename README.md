# wosm
Servicio web para control de paneles de alarma
#
WOSM, facilita el proceso de integración y control de paneles de alarma a traves de diversos medios, este mecanismo ha sido
diseñado para facilitar la operacion de sistemas de alarma de forma remota por el usuario final y que es controlado por una 
una central de monitoreo, que regula su conectividad.
#
HISTORIAL
#
/*   2018-04-24 */
Version     wosm-v3.zip
            Esta version incluye mecanismo para control de dispositivos de la familia CPX, siguiendo el estandar del aplicativo.
			
WS:         Se libera version 3 del servicio web, a partir de la cual las modificaciones a la base de datos se realizan de forma
            automática siguiendo los siguientes pasos.
			a) Descargar el archivo wosm-vx donde x representa la version ejemplo  wosm-v3.zip  v3 representa la version 3.
			b) Descomprimir el archivo zip en la ubicación del sitio que controla IIS  Ejemplo x:\inetpub\wwwroot\wosm
			c) ingresar al sitio del Ws Ejemplo http://localhost/wosm  (No es necesario autenticarse para que el proceso de actualizacion
			   se lleve a cabo.
         
APP	        Se actualizan los archivos usados por la APP para uso de las nuevas rutinas, se modifica el comportamiento de los
            botones de control de manera que el usuario final conozca la operacion disponible segun el estado del dispositivo.
            Ejemplo si el dispositivo esta ARMADO
            solo visualizara el boton DESARMADO y viceversa, de acuerdo con el tipo de dispositivo que esté operando.
Nota:       Para poder operar la serie CPX, cada usuario debe antes actualizar su codigo de acceso al para que el sistema pueda
            enviar la orden al OSM. El codigo de acceso es igual para todos los dispositivos por usuario.
