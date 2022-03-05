Inteligencia artificial smart brain Elias Daal 


1 si ya se clono todo el proyecto entonces seguir los pasos de abajo.

2 introducir informacion de la base de datos
 Descargar PostgresSQL crear la base de datos con nombre y contraseña, introducir los datos como nombre, y contraseña en `server.js` donde dice knex.

3 DETALLES BASE DATOS
Para poder correr el programa es necesario la instalacion de postgres y en la base de datos crear dos tablas las cuales almacenaron los datos de el puntuaje de los usuarios y de los usuarios. se pueden crear las tablas facilmente desde
gitbash terminal(descargar Git trae gitbash), se ingresa a la base de datos con el comando "psql -U postgres NOMBRE.BASEDEDATOS" luego se crearan las dos tablas con estos dos codigos

4 PRIMERA TABLA 
CREATE TABLE users (id serial PRIMARY KEY, name VARCHAR(100), email text UNIQUE NOT NULL, entries BIGINT DEFAULT 0, joined  TIMESTAMP NOT NULL);

5 SEGUNDA TABLA 
CREATE TABLE login (id serial PRIMARY KEY, hash varchar(100) NOT NULL, email text UNIQUE NOT NULL);

6 luego de crar las tablas Correr en la terminal en la ruta de la carpeta api en otra terminal que la de front
 `npm install`

7 Correr en la terminal luego
 `npm start`


 NOTA: Se esta trbajando para que la base de datos no se configure de esta manera.
