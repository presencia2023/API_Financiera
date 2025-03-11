* API REST web de banco, clientes, transacciones financieras

** Descripción y arquitectura de la aplicación
*** Descripción general
API REST de ejemplo para simular un sencillo servicio de transacciones financieras. 

Se podrán realizar las siguientes operaciones:
- Ver la lista de cuentas disponibles
- Abrir una cuenta
- Cerrar una cuenta
- Ver los detalles de una cuenta (titular, autorizado)
- Ver la lista de movimientos de una cuenta
- Hacer un ingreso en una cuenta
- Hacer un reintegro en una cuenta
- Hacer una transferencia entre cuentas(TRANSACCIONES FINANCIERAS).

Se desarrollará también un cliente de una sola página para interactuar con la API. 
Dicho cliente está con el nombre cliente-banco.

*** Arquitectura
La aplicación está estructurada en tres grandes bloques:

- Web API :: Proporciona la lógica de la aplicación y el punto de acceso para interactuar 
con ella. La API puede dar servicio a clientes web, aplicaciones móviles o a plataformas 
de terceros que deseen interactuar con ella.
- Cliente web :: Se trata de un cliente de una sola página. 
En la primera carga se descargan todos los archivos necesarios para su 
funcionamiento y a continuación se realizan llamadas a la API 
para obtener los datos correspondientes. 

- Base de datos :: Almacena la lógica de negocio
Esta base de datos se encuentra con el nombre banco.sql 
Paraesta base de datos utilizamos Mysql como Sistema Gestor de Base de Datos.


*** Formato de datos
Se utilizará el formato JSON para el intercambio de datos entre la API y el cliente (NodeJS).

################ cliente-banco

> Cliente VueJS para utilizar con una API REST de api-banco

El cliente está realizada en [NodeJS](https://nodejs.org/es/).