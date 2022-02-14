# Prueba de Evaluación Práctica 1 - Obra

Realización de un modelo operativo simple de la aplicación destinada al Servicio de Orientación Laboral del Ayuntamiento de Vigo.

Para llevar a cabo esta aplicación, nos dividimos en tres grupos: documentación, diseño y programación. Cada uno de ellos tiene funciones separadas, pero ponemos el trabajo en común en todo momento para que cada una de las personas participantes sepa siempre en qué estadio está el proyecto.

Yo soy integrante del grupo de programación, así que los pasos que se presentan a continuación corresponden a los realizados por dicho grupo.

## Pasos

1. Creación de una base de datos con cada una de las tablas correspondientes (usuarios para las personas funcionarias y personas para los ciudadanos y ciudadanas que se registrarán en la aplicación del S.O.L). Para ello utilizamos *phpmyadmin*

2. En cada una de las tablas se deciden los campos (columnas) a cubrir, en el caso de "personas" son una aproximación a los campos que se corresponderían con los del formulario de entrada de la  app.

3. Dentro de la tabla "usuarios" se crean 3 entradas (también mediante  phpmyadmin), que representan posibles trabajadores del SOL con acceso a la aplicación.

4. Antes de nada, es necesario instalar algunos paquetes en el proyecto:  npm,  bootstrap,  parcel y  popper, para obtener @dito dependencias de funcionalidad.

5. Como siempre, hacemos un . gitignore para no subir al repositorio los archivos innecesarios.

6. También creamos los archivos  style. scss (estilos) y  index. php (primera pantalla de datos).

7. Y hacemos algunos cambios en las rutas de  package. json para que se cree una carpeta " build", que representará el contenido de la  app.
Una vez iniciada la base de datos y las dependencias del proyecto, comenzamos la  construir el  esquelete de programación de la  app:

Primero es imprescindible un  php de conexión con la base de datos "obra", seguido de un formulario de  login donde se identifican los usuarios y se inicia la sesión.
En el  index. php  incluimos uno 'requiere' a la  conexion. php, un pequeño formulario de  búsqueda por nombre y una parte con html para la salida de los datos de la base "personas" por pantalla.

Si el futuro  login funciona con los usuarios creados, obtenemos una pantalla en la que podemos  incluir nuevas "personas" con un formulario en el que los campos a cubrir corresponden con las columnas de la tabla "personas" ( nuevo. php).
Además, se crean los  respetivos archivos  php con las funciones de guardar, modificar, eliminar y actualizar registros de personas, adaptados siempre a los campos de la tabla.
En cuanto al  login inicial por lo que acceden los usuarios (trabajadores de SOL), se hizo mediante la creación de dos archivos:  conexion. php (a la base de datos "obra") y  login. php (formulario simple y código  php que reconoce los datos). También hay un  salir. php que los devuelven al  login y un inicio. php de prueba para confirmar la funcionalidad de esta entrada de datos.

En la carpeta empresas se encuentran los archivos para la visualización de la tabla del mismo nombre y la opción de hacer un nuevo registro como en personas.

Se añadió el trabajo del equipo de diseño sobre el apartado de personas, de este modo tenemos la página  estilada con  header y menú,  footer y un  layout completo de aplicación.

Se reestructutó el árbol de directorios para una mejor organización de carpetas y se hizo un index principal en la base del proyecto.

Continuación del punto 6: se mejoró el sistema de  login de forma que al abrir la aplicación el primero que se pide son las credenciales de usuario y contraseña, una vez son correctas los envían la un  index que será la página de inicio de la  app.  Ahí ya encontraremos el  layout general con el menú superior para navegar por las distintas funcionalidades del sitio. También funciona el  logout de cerrar sesión, de forma que sí volvemos a abrir la aplicación se pide de nuevo la autenticación.

continuación punto 7: se revisó el código y se rehizo la tabla de datos "empresas", y tras unos mínimos cambios ya  conseguemos que esta parte funcione como la de las "personas". También se añadieron las  funión de modificar, eliminar y  update.

Calendario y Citas: se hizo una tabla nueva y su  php correspondiente para sacar las citas por pantalla. También se mejoró el  index. php (pantalla inicial) para que se vean  ahí las citas del día.

Se puso en común el código de programación y lo de diseño del  login, personas y empresas. Se modificaron diversos archivos para su mejora y la óptima  referenciación de rutas absolutas.


## Uso de  Git y  Github

Se elaboró un repositorio común con una rama " master" principal y diversas ramas hijas con añadidos de diferentes personas del equipo de programación, con el objetivo de no interferir con el trabajo individual pero al mismo tiempo poder ver el progreso de los compañeros y rescatar los elementos necesarios en cada momento de la elaboración de las distintas carpetas o funcionalidades.

## Capturas


<img src="https://user-images.githubusercontent.com/89069423/153570520-88311ce3-6312-44df-bbad-bbc7622dd4f7.png"/>
<img src="https://user-images.githubusercontent.com/89069423/153570383-4bfcf451-3d50-4a7d-8652-e4f393b820da.png"/>
<img src="https://user-images.githubusercontent.com/89069423/153570394-8d652070-f0cf-4b9b-8b09-e8173feb2657.png"/>
<img src="https://user-images.githubusercontent.com/89069423/153570403-82fd4a9b-6db7-4e04-83ca-73b3dd265f57.png"/>
<img src="https://user-images.githubusercontent.com/89069423/153570411-7fe2b539-a2cc-4f22-97fc-d306874b1812.png"/>

