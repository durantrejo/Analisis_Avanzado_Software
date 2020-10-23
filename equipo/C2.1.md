# Inicio de proyecto

## :trophy: C2.1 Reto en clase

Requerimientos funcionales del usuario y del sistema.

___

### :blue_book: Instrucciones

- De acuerdo con la información presentada por el asesor referente al tema, y basado en el caso de estudio indicado responder la sesión indicada en el desarrollo de la actividad.
- Toda actividad o reto se deberá realizar utilizando el estilo **MarkDown con extension .md** y el entorno de desarrollo VSCode, debiendo ser elaborado como un documento **single page**, es decir si el documento cuanta con imágenes, enlaces o cualquier documento externo debe ser accedido desde etiquetas y enlaces, y debe ser nombrado con la nomenclatura **C2.x_NombreApellido_Equipo.pdf.**
- Es requisito que el .MD contenga una etiqueta del enlace al repositorio de su documento en GITHUB, por ejemplo **Enlace a mi GitHub** y al concluir el reto se deberá subir a github.
- Desde el archivo **.md** exporte un archivo **.pdf** que deberá subirse a classroom dentro de su apartado correspondiente, sirviendo como evidencia de su entrega, ya que siendo la plataforma **oficial** (aquí se recibirá la calificación de su actividad).
- Considerando que el archivo .PDF, el cual fue obtenido desde archivo .MD, ambos deben ser idénticos.
- Su repositorio ademas de que debe contar con un archivo **readme.md** dentro de su directorio raíz, con la información como datos del estudiante, equipo de trabajo, materia, carrera, datos del asesor, e incluso logotipo o imágenes, debe tener un apartado de contenidos o indice, los cuales realmente son ligas o **enlaces a sus documentos .md**, evite utilizar texto para indicar enlaces internos o externo.
- Se propone una estructura tal como esta indicada abajo, sin embargo puede utilizarse cualquier otra que le apoye para organizar su repositorio.

``` 
| readme.md
| | blog
| | | C1.1_x.md
| | | C1.2_x.md
| | | C1.3_x.md
| | img
| | docs
| | | A1.1_x.md
| | | A1.2_x.md
```

___

### :pencil2: Desarrollo

1. Identificar como mínimo 10 requisitos funcionales del sistema, dándoles un identificador, nombre, detalle o descripción de su funcionalidad, pre-condiciones, secuencia normal, post-condiciones y excepciones.
2. Se propone utilizar la siguiente tabla, sin embargo puede utilizar cualquier otro formato considerando que se deben incluir los elementos solicitados en el punto anterior.

## Listado de requisitos de usuario
   
Identificador | Nombre | Descripción
:--|:--|:--
RUS-01|Ingreso al sistema| Se deberá ingresar al sistema a través de usuarios y claves únicas; una vez que el sistema determine la validez del usuario, le dará permisos a las funciones que se establezcan por el administrador.
RUS-02|Privilegios y roles|Se deberá permitir a un usuario Administrador la facultad de poder asignar sobre ciertas funciones, privilegios de acuerdo con el rol que se asigne a los usuarios.
RUS-03|Agregación de dispositivos|Se deberá poder agregar cualquier dispositivo sensor sin importar su modelo o marca, almacenando sensor, modelo, zona y parámetros. 
RUS-04|Configuración de parámetros|Se podrán configurar parámetros de control máximos y mínimos, de acuerdo con lo que el administrador del sistema establezca.  
RUS-05|Recolección de datos|El sistema deberá ser capaz de recolectar las condiciones ambientales, tales como la temperatura, humedad e iluminación, de acuerdo a un tiempo establecido.
RUS-06|Gráficos de control|El sistema deberá generar gráficos de barra, mapas de color, pie o cualquier otro que permita observar el comportamiento de la muestra adquirida, utilizando colores para indicar si está dentro o fuera de control.
RUS-07|Historial condición dentro de control|El sistema deberá almacenar valores sensados históricos por rango de hora y el valor promedio registrado durante ese rango de hora, así como el valor mínimo y máximo.
RUS-08|Historial condición fuera de control|El sistema deberá almacenar valores sensados históricos por hora, minutos y segundos, cuando el sensor detecte que el valor medido está fuera de control. 
RUS-09|Reportes de historial|El sistema deberá crear reportes de historial, utilizando filtros como: fecha, hora, zonas y sensor.
RUS-10|Alarmas y notificaciones|El sistema deberá enviar alertas y notificaciones al usuario al momento cuando un valor de control esté fuera del rango que se ha establecido.
___

### :white_check_mark: Actividad

#### Tabla 1: Listado de requisitos funcionales del sistema

| Requisito RFN-01: Configuración de usuarios| 
| ------------- |
|**Detalle:** A través de un administrador será posible agregar, consultar, editar y borrar usuarios; cada usuario cuenta con los campos: nombre, apellido, número identificador, rol, clave, correo electrónico y número celular.|
|**Precondición:**<ol><li>Al registrar un nuevo usuario en el sistema, el administrador deberá contar previamente con los datos del mismo.</li><li>Al consultar, actualizar o eliminar un usuario, el administrador deberá contar con su número identificador.</li><li>El administrador deberá acceder a la interfaz de usuarios.</li></ol>|
|**Secuencia normal:**<ol><li>Al agregar, consultar, editar o borrar un usuario, el administrador deberá teclear su número identificador.</li><li>En caso de que el número identificador exista en los registros, se desplegarán los datos asociados al mismo y se habilitarán las opciones de «editar» y «eliminar».</li><li>Al ingresar nuevos datos o realizar algún cambio en el sistema, se habilitará la opción de «guardar».</li></ol>|
|**Post-condición:**<ol><li>El sistema mostrará un mensaje especificando el tipo de operación que se realizó y confirmará que se efectuó de manera exitosa.</li></ol>|
|**Excepciones:**<ol><li>El sistema mostrará un mensaje indicando que ocurrió un error y especificará su índole.</li></ol>|

| Requisito RFN-02: Asignacion de Privilegios y roles| 
| ------------- |
|**Detalle:** Se deberá permitir a un usuario administrador el poder asignar funciones a los usuarios através de roles y/o privilegios.|
|**Precondición:**<ol>  <li> Si se le asignaran permisos diferentes al usuario normal como eliminar, actualizar, agregar nuevos items, se debera especificar los permisos a asignar por escrito</li>  <li>Si se le asignaran privilegios para acceder a ciertos ap;artados, se debe especificar por escrito a que apartados tendra acceso</li> <li>El usuario administrador entrara al sistema</li></ol>||
|**Secuencia normal:**<ol><li>El usuario que entre a asignar nuevos permisos, deberan coincidir sus datos con los del usuariolos registrado como admin.</li><li>Al coincidira se habilitaran las funciones para asignar diversas configuraciones a otros usuarios</li><li>Al ingresar nuevos roles o privilegios a otros usuarios, se habilitará la opción para guardar dichos cambios.</li></ol>||
|**Post-condición:**<ol><li>Al realizar y guardar los cambios anteriores desplegara que usuario y que roles o privilegios se le han asignado</li></ol>||
|**Excepciones:**<ol><li>Al no coincidir los datos del usuario que desea entrar con los del usuario administrador no permitira acceder al sitio.</li></ol>||

| Requisito RFN-03: Agregación de dispositivos| 
| ------------- |
|**Detalle:** A través de un administrador será posible agregar sensores; cada sensor cuenta con los campos: modelo, marca, zona y parámetros bajo los que realiza lecturas.|
|**Precondición:**<ol><li>Al registrar un nuevo dispositivo en el sistema, el administrador deberá contar previamente con la información y especificaciones del mismo.</li><li>El administrador deberá acceder a la interfaz de usuarios.</li></ol>|
|**Secuencia normal:**<ol><li>Al agregar un dispositivo, el administrador deberá ingresar los datos del sensor.</li><li>Al finalizar de ingresar los datos del dispositivo, se habilitará la opción de «guardar».</li></ol>|
|**Post-condición:**<ol><li>El sistema mostrará un mensaje especificando el tipo de operación que se realizó y confirmará que se efectuó de manera exitosa.</li></ol>|
|**Excepciones:**<ol><li>El sistema mostrará un mensaje indicando que ocurrió un error y especificará su índole.</li></ol>|

| Requisito RFN-04: Configuración de parámetros| 
| ------------- |
|**Detalle:** A través de un administrador será posible establecer un valor de temperatura mínimo y uno máximo para definir los parámetros de control de los sensores.|
|**Precondición:**<ol><li>Al configurar los parámetros de control en el sistema, el administrador deberá tener definido el rango que se establecerá.</li><li>El administrador deberá acceder a la interfaz de configuración de parámetros.</li></ol>|
|**Secuencia normal:**<ol><li>Al configurar los parámetros, el administrador deberá ingresar una temperatura mínima y una máxima.</li><li>Al finalizar de ingresar los datos, se habilitará la opción de «guardar».</li></ol>|
|**Post-condición:**<ol><li>El sistema mostrará un mensaje especificando el tipo de operación que se realizó y confirmará que se efectuó de manera exitosa.</li></ol>|
|**Excepciones:**<ol><li>El sistema mostrará un mensaje indicando que ocurrió un error y especificará su índole.</li></ol>|

| Requisito RFN-05: Recolección de datos|   
| ------------- |
|**Detalle:** El sistema deberá ser capaz de recolectar las condiciones ambientales, tales como la temperatura, humedad e iluminación, de acuerdo a un tiempo establecido. |
|**Precondición:**<ol><li> A traves de los sensores instalados se tomara la temperatuta, iluminacion, humedad, entre otros factores del ambiente</li> </ol>|
|**Secuencia normal:**<ol><li> Se capturaran y almacenara los datos que se tomarons por los sensores </li> </ol>|
|**Post-condición:**<ol><li>El sistema mostrará un mensaje especificando que el almacenamiento de datos se efectuó de manera exitosa.</li><li> Posteriormente se mostraran los datos a los usuarios correspondientes en la interfaz del sistema. </li> </ol>|
|**Excepciones:**<ol><li>El sistema mostrará un mensaje indicando que ocurrió un error.</li></ol>|

| Requisito RFN-06: Gráficos de control| 
| ------------- |
|**Detalle:** El sistema deberá generar gráficos de barra, mapas de color, pie o cualquier otro que permita observar el comportamiento de la muestra adquirida, utilizando colores para indicar si está dentro o fuera de control.|
|**Precondición:**<ol><li> Se extraeran los datos que el usuario solicita, despues de que estos han sido capturados y procesados por los sensores de nuestro gestor de almacenamiento</li></ol>|
|**Secuencia normal:**<ol><li>  El sistema los dividira y asignara algun tipo de grafico segun sea mas conveniente. </li></ol>|
|**Post-condición:**<ol><li>En el apartado de graficos del sistema, mostrara el grafico resultante de la solicitud. </li></ol>|
|**Excepciones:**<ol><li>El sistema mostrará un mensaje indicando que ocurrió un error.</li></ol>|

| Requisito RFN-07: Historial condición dentro de control| 
| ------------- |
|**Detalle:** El sistema deberá almacenar valores sensados históricos por rango de hora y el valor promedio registrado durante ese rango de hora, así como el valor mínimo y máximo dentro del rango de control. |
|**Precondición:**<ol><li>Se debera hacer el RFN-04 que indica al adiministrador asignar un valor minimo y maximo al sensor.</li></ol>|
|**Secuencia normal:**<ol><li>Si los sensores se encuentran dentro del rango de control establecido sera registrado el hitorial de condicion.</li></ol>|
|**Post-condición:**<ol><li>El sistema mostrará una notificacion del evento registrado.</li></ol>|
|**Excepciones:**<ol><li>El sistema mostrará un mensaje indicando que ocurrió un error.</li></ol>|


| Requisito RFN-08: Historial condición fuera de control| 
| ------------- |
|**Detalle:** Tomando el valor asignado al sensor por el adiministrador en base al parametro RFN-04 se tomara registros del sensor que este fuera de la medida de control, la hora, minuto y segundos|
|**Precondición:**<ol><li>Se debera hacer el RFN-04 que indica al adiministrador asignar un valor minimo y maximo al sensor.</li></ol>|
|**Secuencia normal:**<ol><li>Los sensores tiene que estar fuera del rango de control para que sea registrado el hitorial de condicion.</li></ol>|
|**Post-condición:**<ol><li>El sistema mostrará una notificacion del evento registrado.</li></ol>|
|**Excepciones:**<ol><li>El sistema mostrará un mensaje indicando que ocurrió un error y especificará su índole.</li></ol>|


| Requisito RFN-09: Reportes de historial| 
| ------------- |
|**Detalle:** El sistema creara reportes de historial, utilizando filtros como: fecha, hora, zonas y sensor.|
|**Precondición:**<ol><li>Se tendra alamcenado un historial de eventos fuera de control de sensores.</li><li>El administrador deberá acceder a la interfaz de reportes de historial.</li></ol>|
|**Secuencia normal:**<ol><li>El usurio tendra la opcion de poder crear reportes utilizando fechas, horarios, zonas y por sensores.</li></ol>|
|**Post-condición:**<ol><li>El sistema mostrará un mensjae que se a creado exitosamente el reporte.</li></ol>|
|**Excepciones:**<ol><li>El sistema mostrará un mensaje indicando que ocurrió un error y especificará su índole.</li></ol>|


| Requisito RFN-10: Alarmas y notificaciones| 
| ------------- |
|**Detalle:** El sistema deberá enviar alertas y notificaciones al usuario al momento cuando un valor de control esté fuera del rango que se ha establecido.|
|**Precondición:**<ol><li>El administrador debera asignar el rango de control de los sensores como se especifica en RFN-04.</li><li>El usuario deberá acceder al sistema.</li></ol>|
|**Secuencia normal:**<ol><li>En cuanto el sensor este fuera del rango de control se notificara al usuario.</li></ol>|
|**Post-condición:**<ol><li>Sera mantendra en vista la notificacion hasta que la vea el usuario.</li></ol>|
|**Excepciones:**<ol><li>El sistema mostrará un mensaje indicando que ocurrió un error y especificará su índole.</li></ol>|



:house: [Mi GitHub](isitos.md&ust=1603125240000000&usg=AOvVaw2VBbvZHyTdNQOsTsE5Z4HG&hl=es)
