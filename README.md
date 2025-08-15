# LoteriaOnline
Sistema de lotería online fundamentado en la blockchain, cuyo propósito sería garantizar la transparencia y hacer crecer la confianza de los participantes en dicho juego. 

README
Proyecto de Lotería Online, que busca resolver los típicos problemas relacionados con la falta de transparencia y el nivel de confianza que se tiene con este tipo de juegos de azar. 
La idea central de proyecto sería poder tener un contrato inteligente desplegado en la blockchain, el cual contendría todas las reglas y normativas de la lotería de forma inmutable, de manera tal que una vez desplegado el contrato estas no se pueden alterar. 
Se buscaría poder automatizar la mayor parte de todo el proceso de juego (venta de boletos, sorteo y distribución de premios) con el fin de eliminar intermediarios, distribuir de forma automática e inmediata los premios y eliminar las posibilidades de reclamos, debido al incumplimiento de normativas.
Funcionamiento.
1. Venta de boletos:
•	Los jugadores comprarían boletos para el sorteo utilizando criptomonedas, podrían ser distintas criptomonedas o con un token propio de la lotería.
•	Para el caso de venta de boletos únicos podría ser con un token no fungible (NFT), lo que garantiza que cada boleto sea único y tenga un dueño verificable. 
•	Para el caso de permitirse múltiples ganadores, un boleto puede ser comprado o adquirido por múltiples participantes y en caso de múltiples ganadores con un mismo boleto, el premio será distribuido de forma equitativa entre los ganadores.   
•	Toda compra del boleto se registraría como una transacción en la blockchain. 
•	Se debe mostrar si un boleto ha sido vendido o está disponible, de igual manera para las múltiples apuestas se debe mostrar que tanta cantidad de boletos se han vendido para un número en particular, tiendo con esto la base para la transparencia en cuanto a la distribución de los premios.
•	El dinero recaudado de la venta de boletos se acumularía automáticamente en el contrato inteligente, formando el pozo o bote. Este bote sería público y cualquiera puede auditar su saldo en cualquier momento, lo que eliminaría cualquier duda sobre la cantidad total de dinero que se ha recaudado. 
2. Generación del número ganador:
•	Este es el punto más crítico para garantizar la imparcialidad. En esta lotería con blockchain, se usaría un método criptográfico para generar el número ganador aleatorio, de forma transparente y verificable.
•	Se pudiera programar una función que pueda tomar un dato aleatorio externo, que sea imposible de predecir, este dato pueda ser usado con semilla para que el contrato inteligente ejecute una función que determine el número ganador.  Todo el proceso sería público, lo que permitiría a cualquier persona verificar el resultado por sí misma.
3. Distribución de premios:
•	Una vez que el número ganador ha sido generado, el contrato inteligente debe ejecutar automáticamente el pago.
•	El contrato compara el número ganador con los boletos comprados. Si hay boleto ganador, el contrato transfiere automáticamente los fondos del pozo a la dirección de la billetera del ganador o los ganadores lo correspondiente al premio a repartir.
•	Se elimina la necesidad de que el ganador o ganadores se presenten con un boleto físico, así como también la intervención de un intermediario o administrador de la lotería. El pago siempre sería instantáneo, automático y sin intermediarios.
Componentes claves del Proyecto
Para desarrollar este proyecto, se necesitarían los siguientes componentes:
•	Contrato Inteligente: El código principal que define la lógica de la lotería, incluyendo la compra de boletos, la generación de número ganador y la distribución de premios. Se escribiría en un lenguaje Move y se desplegaría en la blockchain SUI.
•	Interfaz de Usuario (Front-End): Una aplicación móvil o una página web que permitiría a los usuarios interactuar fácilmente con el contrato inteligente. Los usuarios podrían ver el bote acumulado, realizar la compra de boletos, ver el historial de sorteos y verificar si han ganado.
•	Billetera (Wallet): Los usuarios necesitarían una billetera de criptomonedas para conectar con la interfaz de usuario, comprar los boletos y recibir los premios.
•	Oráculo Descentralizado: Conectar con una herramienta como Chainlink que provea el dato semilla aleatorio verificable para la selección de los números ganadores, eliminando cualquier manipulación.
•	Token (Opcional): Se podría crear un token propio de la lotería que los usuarios usen para comprar boletos. Esto podría tener utilidades adicionales, como descuentos en la compra, sorteos especiales entre los boletos no ganadores comprados con token, etc.
Se ofrece: 
•	Con la inmutabilidad de la blockchain y la transparencia del contrato inteligente se garantiza que no hay manipulación ni fraude. Con esto se busca lograr que los jugadores pueden confiar plenamente en que el juego es justo.
•	Como todo el proceso, desde la venta de boletos hasta el pago del premio, es público y auditable, se garantiza la transparencia, ya que cualquiera puede ver cuánto dinero hay en el pozo y cómo se ha seleccionado al ganador. 
•	Los premios se transfieren automáticamente, eliminando la espera y la necesidad de tener que reclamarlos.
•	Al automatizar el proceso con un contrato inteligente, se reduce la necesidad de personal, intermediarios y sistemas de gestión complejos lo que reduciría los costos operativos en el funcionamiento de la lotería.


