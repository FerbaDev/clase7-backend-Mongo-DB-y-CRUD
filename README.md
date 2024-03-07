# Clase 7 de Backend 

instalamos Mongo DB -----------  00:33

Configuramos Mongo shell -----------  01:05

### comandos para crear base de datos

show dbs ---------------------- 01:24

1) use nombreBasedeDatos: crea y se posiciona en una nueva base de datos,  si la base de datos ya existe, no la sobreescribe ni la elimina, sino que solo se posiciona sobre ella. Para que se haga efectiva la creacion de esta base de datos tiene que guardar al menos una coleccion (array). 

2) creamos una nueva coleccion con el comando: db.createCollection("nombredelacoleccion");     ---------- 01:28

voy a test con use test y ejecuto el comando show dbs, y ahora muestra la nueva bbdd

- para ver las colecciones que tiene cada bbdd, estando posicionados sobre ella ejecutamos en comando: show collections

- para borrar una coleccion, estando posicionados sobre la base de datos donde se almacena, 
ejecutamos el comando: db.nombredelacoleccion.drop();
y nos devuelve un true

- y para borrar una base de datos, estando posicionado sobre la misma, ejecutamos db.dropDatabase();     01:34

3) para ingresar un documento en alguna coleccion de una base de datos, db.nombrecollection.insertOne({objeto})                01:39

---- metodo find para MOSTRAR LOS ELEMENTOS de la collection: db.nombrecollection.find()                     01:44

4) para insertar mas de un objeto a la coleccion: db.nombrecollection.insertMany([{obj1},{obj2}])

#### Búsquedas
ver dispositiva 59 ......... min 02:59

CONTEO DE DATOS ------------ 03:22  .::: db.nombrecollection.estimatedDocumentCount()
                                        db.nombrecollection.countDocuments(opt) opt:para que cumplan criterio de conteo

#### Filtros
ver dispositiva 69 ----------- min 03:39

#### Proyecciones, sorts, skips y limits
1)  proyecciones min 03:54

2) sort       min 03:57

#### CRUD 
min 04:07

