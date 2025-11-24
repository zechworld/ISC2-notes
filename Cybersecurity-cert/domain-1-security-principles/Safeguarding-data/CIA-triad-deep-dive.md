# Triada CIA - Analisis en profundidad
### Proteccion de datos (Safeguarding Data)

## Confidencialidad
Este parametro es uno que lleva tiempo balancear cuando muchos usuarios ingresan al sistema. No todos los usuarios que ingresan al sistema, sean invitados o clientes, pueden ser catalogados como seguros dado que no se conoce si los equipos desde los que estan accediendo al sistema poseen algun tipo de riesgo asociado a ellos. Es por esto que los especialistas deben proteger los datos, asegurando que la informacion este disponible solo para aquellos usuarios que tengan un acceso autorizado.

Para entender de mejor manera la *confidencialidad*, debemos entender varios terminos asociados a la misma.

### **PII (Personally Identifiable Information)**
Son todos aquellos datos de un individuo que permiten identificarlo. Algunos ejemplos pueden ser el RUT, nombre completo, direccion de correo electronico o numero telefonico. 

A medida que las personas confian cada vez mas en TI tanto en sus trabajos como en su vida cotidiana, el aumento de **PII** que es compartido entre organizaciones es directament proporcional. El entendimiento de estos datos sensibles les permite a los comercios generar productos a la medida y entender las tendencias de los consumidores. Sin embargo, el crecimiento de estas *Bases de dato* genera un mayor interes a los atacantes.

El robo de los **PII** les permite a los atacantes tener una serie de opciones con las cuales sacar beneficios, como realizar robos de identidad, venta de datos en el mercado negro, o realizar un **ataque Ransomware** con el cual obtener una recompensa.

Los **PII** se pueden clasificar en diferentes criterios: segun sus tipo como directos, indirectos y segun su impacto como sensibles y no sensibles.

#### PII Directos vs PII Indirectos - 
Los **PII directos** son aquellos que identifican directamente a una persona, como el *numero de pasaporte*, *licencia de conducir* o *carnet de identidad*. Este tipo de dato es suficiente como para funcionar por si solo para determinar la identidad de una persona.

Los **PII indirectos** son aquellos datos que ayudan a identificar a una persona, pero por si solos no aportan suficiente informacion como para determinar la identidad de la misma. En este caso podemos encontrar el *genero*, *codigo postal* o *fecha de nacimiento*. 

### PII Sensibles vs PII no sensibles
Para empezar, no todos los datos son considerados como PII. Los habitos de una persona, por ejemplo, no son considerados PII dado que dificultaria mucho identificar a un individuo solo con "cuales son las series que ve en Netflix". Los PII tienen que ser datos que correlacionen datos con una persona en particular, y este aspecto algunos datos son mas sensibles que otros y pueden generar un impacto diferente en caso de una eventualidad de un ataque.

- **PII Sensibles**: Son aquellos datos que pueden generar un impacto o daño significativo en caso de que sean filtrados o robados. En el caso de Chile, el numero de RUT es un dato sensible y directo que puede generar un sinnumero de problemas al ser utilizado de forma maliciosa. Otros tipos de PII sensibles son: *licencia de conducir (en algunos paises se utiliza como ID), el numero de pasaporte o cualquier documento gubernamental, datos biometricos, datos financieros y registros medicos*. Estos PII **no estan disponibles al publico** y ciertas leyes exigen que el almacenamiento de los mismos requieran algun tipo de encriptacion y otras medidas de ciberseguridad.


- **PII No sensibles**: Son aquellos datos que de forma aislada su impacto no causa un daño significativo a la persona en caso de ser filtrados o robados. Este tipo de PII no es necesario que sean unicos para una persona. Por ejemplo, el nombre de cuenta de alguna red social. Este puede identificar a alguien, pero no son lo suficientemente fuerte como para que los atacantes puedan realizar una suplantacion de identidad. Otro tipo de PII no sensibles son: *Nombre completo, apellidos, numero de telefono, direccion IP, lugar de nacimiento, fecha de nacimiento, detalles geograficos, detalles de empleo, correo electronico o correo, raza o etnicidad, religion*. Comunmente estos PII se encuentran disponibles publicamente, no son necesariamente protegidas por las regulaciones, pero algunas compañias deciden de igual manera guardarlas en un lugar seguro.

Es importante tener en cuenta que si bien los PII no sensibles puede que por si solos no generen un daño mayor, pero si un atacante correlaciona varios PII no sensibles, estos se pueden transformar en una amenaza. Por ejemplo, un atacante puede que haya encontrado los siguientes PII no sensibles: Correo electronico, telefono, y apellido materno. Con estos datos, eventualmente, podria acceder al banco y obtener PII sensibles.

Email = Puede obtener el nombre de usuario
Telefono = Obtener codigo de verificacion
Apellido = Responder pregunta de seguridad

[Mas informacion sobre PII](https://www.ibm.com/think/topics/pii)

Como vimos en la seccion anterior, la **sensibilidad** es un topico que podemos definir como la importancia que le asigna a la informacion el dueño de la misma y por ende impacta en el daño que puede realizar a una organizacion o individuo. 

## Integridad
La principal idea detras de la integridad de los datos o de la informacion es determinar que tan **integros** estan, en otras palabras si estan completos, consistentes y correctos. Este concepto aplica para:
- Sistemas y procesos relevantes en la operacion de las organizaciones
- Organizaciones
- Personas y sus acciones

### Integridad de Datos
Que un dato sea integro es la garantia que este mismo no haya sido alterado de una forma no autorizada. Mientras los datos estan siendo almacenados o esten en trasito, se deben tomar medidas de seguridad que los protejan de modificaciones, errores o que haya perdida de informacion. Esto tambien incluye el instante en el que se esta registrando la informacion, asegurando que los datos sean consistentes e integros.

De esta manera, a traves de la consistencia, los datos deben ser los mismos en todos los sistemas en los que se esten usando o almacenando manteniendo su forma, contenido y su significado.

### Integridad del sistema
Se refiere al mantenimiento de una configuracion confiable y su funcionamiento esperado a medida que el sistema procesa la informacion. Para esto se establece el **Estado**, que no es mas que la condicion actual del sistema. 
