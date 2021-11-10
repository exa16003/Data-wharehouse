# data_warehouse
**Data Warehouse es una herramienta que permita a una compañía de Marketing administrar todos los contactos de
sus clientes para sus campañas. 
Realiza CRUD de usuarios, contactos, regiones(paises y ciudades) y compañías. 
Utilizando: 
- HTML, CSS y JavaScript (Frontend)
- Node.js y Express.js (Backend).
- MySQL (MariaDB) (Base de datos) **

# ¿Cómo correr la API localmente?

Para lograr correr la API de forma local es necesario contar con [XAMPP](https://www.apachefriends.org/index.html).
Luego de descargarlo tenés que iniciar el servidor Apache y la base de datos MySQL presionando en "start" en cada uno de ellos.
Luego, al presionar en "admin" en MySQL se abrirá una página de PHPMyAdmin con la base de datos.

## Configurar la base de datos

1. Es necesario editar el archivo [sequelize.js]
y cambiar los datos para que coincida con tu configuración, la estructura es
(**mysql://user:password@host:port/database**).

2. Ahora es necesario importar en PHPMyAdmin los datos de la base de datos.  
En la página de PHPMyAdmin ir a la pestaña "Importar" y ahí seleccionar el archivo: [data_warehouse.sql].


##  correr el servidor

Ir al directorio [Server]
hacé click derecho en el archivo "app.js" y seleccioná "Open in integrated Terminal". 
Se abrirá una terminal en la cual tenemos que escribir:

`nodemon app.js`

En caso de no haber ningún error debe aparecer la leyenda: "Servidor está corriendo en el puerto 3000" seguido de: "Conectado a Sequelize".

## Iniciar la parte del Frontend de la página
Coloca el usuario joaquin y la contraseña "11223344" y podrás ingresar a todas las funciones de la página ya que ingresarás como administrador.
En caso de no querer iniciar como administrador, debes ingresar con cualquiera de los demás usuarios (sus datos están en la base de datos en la tabla de "usuarios")


