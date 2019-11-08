# **Proyecto Ingeniería de Software C** 

## **Introducción**
VetZoo es un sistema de información enfocado a pequeñas veterinarias que buscan optimizar sus procesos administrativos. 

Es natural que dentro del desarrollo de software se busque la calidad total, por lo que es necesaria la implementación 
de un modelo de calidad que ayude a obtenerla. 

El modelo de calidad aplicado al siguiente proyecto de software es el ISO/IEC 9126 el cual es un estándar internacional para la evaluación del software que surge debido
a la necesidad de un modelo único para expresar la calidad de un software.

## **Objetivos**

### **Objetivo General**

> Herramienta digital que permite automatizar y administrar el proceso que tienen las veterinarias facilitando al usuario su actividad laboral. Mediante el registro y guardado de información de los pacientes, su historial y medicamentos usados, además de tener un mejor control de los medicamentos en la bodega.

### **Objetivos Específicos**

- Administración de información de:
  - Médicos Veterinarios 
  - Pacientes
  - Consultas 
  - Medicamentos 
   
- La Veterinaria se beneficiará realizando un aprovechamiento eficiente de recursos. 
- Generación automática de reportes tales como recetas, inventarios de medicamentos, etc. 
- Ahorro de tiempo y espacio de almacenamiento de reportes.
- Se tendrá un menor tamaño de inventarios de medicamentos susceptibles de caducidad próxima. 

## **Módulos del proyecto**

Número | Módulos
-----|--------
1 | Busca Pacientes
2 | Consulta
3 | Login 
4 | Menú
5 | PantallaCitas
6 | PantallaInicio
7 | PrimerControlDeUsuario
8 | Receta Medicamentos
9 | Registro Compra
10 | RegistroDoctores
11 | RegistroDueño
12 | RegistroPaciente
13 | RegistroProveedor
14 | RegistroVenta
15 | VentanaCompra
16 | VentanaVenta

## **Descripción de Módulos**
### **Modulo BuscaPaciente**

Función | Descripción
--------|------------
button1_Click | Captura el evento que permite que se visualice el paciente consultado
button2_Click| Captura el evento que limpia la pantalla donde se muestran los pacientes

### **Modulo Consulta**
Función | Descripción
--------|------------
llenacombobox | Enlista los pacientes de la tabla
button3_Click | Captura el evento que muestra la ventana de receta
button4_Click | Captura el evento que muestra la ventana para poder crear pacientes
openConnection | Se realiza la conexión con la base de datos
closeConnection|Se finaliza la conexión con la base de datos
executeMyQuery | Validación al interactuar con la base de datos
btRegistro_Click | Se crea una consulta guardándola en la base de datos
btLimpiar_Click | Limpia la pantalla 


### **Modulo Login**
Función | Descripción
--------|------------
button1_Click | Evento que permite iniciar sesión del usuario dentro del sistema
btncerrar_Click | Evento que cierra la aplicación.
txtUsuario_Click | Evento que limpia el cuadro de texto para usuario

### **Modulo Menú**
Función | Descripción
--------|------------
ocultaBotones | Captura el evento que permite ocultar los botones de la sección de registro
muestraBotones | Captura el evento que permite mostrar los botones de la sección de registro
button1_Click | Evento que envía a la pantalla principal
button2_Click | Evento que acomoda la interfaz según el usuario
btRU_Click | Evento que muestra la pantalla de registro de Usuarios
btRD_Click | Evento que muestra la pantalla de registro de Doctores
btRP_Click | Evento que muestra la pantalla de registro de Pacientes
btRDueño_Click | Evento que muestra la pantalla de registro de los dueños
btCitas_Click | Se muestra la pantalla para generar citas
btConsulta_Click | Evento que muestra la pantalla con todo lo referente a una consulta
btVentas_Click | Evento que muestra la pantalla con todo lo referente a una Venta
btCompra_Click | Evento que muestra la pantalla con todo lo referente a una Compra
bloquear | Evento que interactuá con los botones para activarlos o desactivarlos


### **Modulo PantallaCitas**
Función | Descripción
--------|------------
dataGridView1_MouseClick | Evento que muestra en el cuadro de texto la celda seleccionada de la tabla 
llenacombobox | Evento que llena un combobox según la tabla de Pacientes
llenacombobox2 | Evento que llena un combobox según la tabla de Doctores
PantallaCitas_Load | Evento que carga la información al entrar a la ventana
openConnection | Se genera la conexión con la base de datos
closeConnection | Se finaliza la conexión con la base de datos
executeMyQuery | Validación al interactuar con la base de datos
MuestraTabla | Genera la tabla con los datos de la cita
btRegistro_Click | Se genera una sentencia para ingresar registros a la tabla de Citas
btEliminar_Click | Eliminación de un elemento de la tabla de cita
btActualiza_Click | Actualización de la tabla cita
btLimpiar_Click | Se realiza una limpieza en la pantalla

### **Modulo PantallaInicio**
Función | Descripción
--------|------------
PantallaDeRegistros_Load | N/A
btUsuarios_Click | N/A

### **Modulo PrimerControlDeUsuario**

Función | Descripción
--------|------------
dataGridView1_MouseClick | Evento que muestra la celda seleccionada en un textbox.
PrimerControlDeUsuario_Load | Evento que carga el contenido de la ventana
openConnection | Se genera la conexión con la base de datos
closeConnection | Se finaliza la conexión con la base de datos
executeMyQuery | Validación en la consulta a la base de datos 
btRegistro_Click | Evento que inserta registros en la base de datos de usuarios 
button2_Click | Actualización en la base de datos 
button1_Click| Evento que elimina un elemento de la tabla
btLimpiar_Click | Evento que limpia los cuadros de texto en pantalla

### **Modulo RecetaMedicamentos**

Función | Descripción
--------|------------
llenacombobox | Enlista los Doctores disponibles en la base de datos
llenacombobox2 | Enlista los Pacientes disponibles en la base de datos
openConnection | Se genera la conexión con la base de datos
closeConnection | Se finaliza la conexión con la base de datos 
executeMyQuery| Se realiza la validación de la consulta de la base de datos
button1_Click | Se captura el evento para crear recetas


### **Modulo RegistroCompra**

Función | Descripción
--------|------------
dataGridView1_MouseClick | Evento que muestra en un cuadro de texto la celda seleccionada 
llenacombobox | Enlista los Doctores disponibles en la base de datos
RegistroCompra_Load | Evento que carga la información de la ventana
openConnection | Se genera la conexión con la base de datos
closeConnection | Se finaliza la conexión con la base de datos 
executeMyQuery| Se realiza la validación de la consulta de la base de datos
MuestraTabla | Se muestra la tabla con los datos referentes a las compras
btRegistro_Click | Se genera un registro de Compra
btActualiza_Click | Se actualiza los datos del registro de compra
btEliminar_Click | Evento que elimina un registro de la tabla Compra
btLimpiar_Click | Evento que limpia la ventana 


### **Modulo RegistroDoctores**

Función | Descripción
--------|------------
dataGridView1_MouseClick | Evento que muestra en un cuadro de texto la celda seleccionada 
RegistroDoctores_Load | Evento que carga la información al entrar a la ventana
openConnection | Se establece la conexión con la base de datos
closeConnection | Se finaliza la conexión con la base de datos 
executeMyQuery| Se realiza la validación de la consulta de la base de datos
MuestraTabla | Se muestra la tabla con los datos
btRegistro_Click | Se inserta un registro en la tabla doctor
btActualiza_Click | Se actualiza el registro de la tabla doctor
btEliminar_Click | Se elimina el registro de la tabla doctor
btLimpiar_Click | Evento que limpia todos los cuadros de texto de la ventana

### **Modulo RegistroDueño**

Función | Descripción
--------|------------
dataGridView1_MouseClick | Evento que muestra en un cuadro de texto la celda seleccionada 
RegistroDueño_Load | Evento que carga la información al entrar a la ventana
openConnection | Se establece la conexión con la base de datos
closeConnection | Se finaliza la conexión con la base de datos 
executeMyQuery| Se realiza la validación de la consulta de la base de datos
MuestraTabla | Se muestra la tabla con los datos
btRegistro_Click | Se inserta un registro en la tabla dueño
btActualiza_Click | Se actualiza el registro de la tabla dueño
btEliminar_Click | Se elimina el registro de la tabla dueño
btLimpiar_Click | Evento que limpia todos los cuadros de texto de la ventana

### **Modulo RegistroPaciente**

Función | Descripción
--------|------------
dataGridView1_MouseClick | Evento que muestra en un cuadro de texto la celda seleccionada 
RegistroPaciente_Load | Evento que carga la información al entrar a la ventana
openConnection | Se establece la conexión con la base de datos
closeConnection | Se finaliza la conexión con la base de datos 
executeMyQuery| Se realiza la validación de la consulta de la base de datos
MuestraTabla | Se muestra la tabla con los datos
btRegistro_Click | Se inserta un registro en la tabla paciente
btActualiza_Click | Se actualiza el registro de la tabla paciente
btEliminar_Click | Se elimina el registro de la tabla paciente
btLimpiar_Click | Evento que limpia todos los cuadros de texto de la ventana
### **Modulo RegistroProovedor**

Función | Descripción
--------|------------
dataGridView1_MouseClick | Evento que muestra en un cuadro de texto la celda seleccionada 
RegistroProveedor_Load | Evento que carga la información al entrar a la ventana
openConnection | Se establece la conexión con la base de datos
closeConnection | Se finaliza la conexión con la base de datos 
executeMyQuery| Se realiza la validación de la consulta de la base de datos
MuestraTabla | Se muestra la tabla con los datos
btRegistro_Click | Se inserta un registro en la tabla promovedor
btActualiza_Click | Se actualiza el registro de la tabla proovedor
btEliminar_Click | Se elimina el registro de la tabla paciente
btLimpiar_Click | Evento que limpia todos los cuadros de texto de la ventana

### **Modulo RegistroVenta**

Función | Descripción
--------|------------
dataGridView1_MouseClick | Evento que muestra en un cuadro de texto la celda seleccionada 
RegistroVenta_Load | Evento que carga la información al entrar a la ventana
openConnection | Se establece la conexión con la base de datos
closeConnection | Se finaliza la conexión con la base de datos 
executeMyQuery| Se realiza la validación de la consulta de la base de datos
MuestraTabla | Se muestra la tabla con los datos
btRegistro_Click | Se inserta un registro en la tabla venta
btActualiza_Click | Se actualiza el registro de la tabla venta
btEliminar_Click | Se elimina el registro de la tabla venta
btLimpiar_Click | Evento que limpia todos los cuadros de texto de la ventana

### **Modulo VentanaCompra**

Función | Descripción
--------|------------
button2_Click | Evento que muestra la ventana de proveedores
button3_Click | Evento que muestra la ventana de registro de compra
button1_Click | Evento que realiza una consulta en la tabla compra
VentanaCompra_Load | Carga de información de la ventana
button4_Click | Evento que limpia los cuadros de texto de la pantalla
### **Modulo VentanaVentas**

Función | Descripción 
--------|-------------
button2_Click | Evento que muestra la ventana de proveedores|dd
button3_Click | Evento que muestra la ventana de registro de venta
button1_Click | Evento que realiza una consulta en la tabla venta
VentanaVentas_Load | Carga de información de la ventana
button4_Click | Evento que limpia los cuadros de texto de la pantalla

## Tabla 2 Validación de Módulos

### **Modulo BuscaPacientes**
Funciones | Validaciones
----------|-------------
button1_Click | No valida si el cuadro de texto esta vació

### **Modulo Consulta**
Funciones | Validaciones
----------|-------------
openConnection | Si esta cerrado, si se puede abrir la conexión
closeConnection | Si esta abierto, si se puede cerrar la conexión
executeMyQuery | Se valida si se puede hacer o no la conexión con la base de datos
btRegistro_Click | No valida si los campos a llenar se dejan vacíos o no coinciden con el tipo

### **Modulo Login**
Funciones | Validaciones
----------|-------------
button1_Click | Si se valida que el usuario coincida con la contraseñá
txtUsuario_Click | Validación de campos
txtContraseña_Click | Validación de campos


### **Modulo Menu**
Funciones | Validaciones
----------|-------------
Menu | No se valida si las cadenas están vaciás
bloquear | Validación dependiendo del usuario, cambia la interfaz

### **Modulo PantallaCitas**
Funciones | Validaciones
----------|-------------
dataGridView1_MouseClick | No valida si la tabla no contiene la información para pasar a los cuadros de texto
openConnection | Si esta cerrado, si se puede abrir la conexión
closeConnection | Si esta abierto, si se puede cerrar la conexión
executeMyQuery | Se valida si se puede hacer o no la conexión con la base de datos
btRegistro_Click | No valida si los campos a llenar se dejan vacíos o no coinciden con el tipo
btEliminar_Click | No valida si el campo Id está vació
btActualiza_Click | No se valida si no se seleccionaron los combo o se llenaron todos los datos antes de realizar un UPDATE

### **Modulo PantallaInicio**
Funciones | Validaciones
----------|-------------
PantallaDeRegistros_Load | N/A
btUsuarios_Click | N/A

### **Modulo PrimerControlDeUsuario**
Funciones | Validaciones
----------|-------------
dataGridView1_MouseClick | No se valida, pero puede hacerse la validación si el campo está vacío
openConnection | Si esta cerrado, si se puede abrir la conexión
closeConnection | Si esta abierto, si se puede cerrar la conexión
executeMyQuery | Se valida si se puede hacer o no la conexión con la base de datos
btRegistro_Click | No valida si los campos a llenar se dejan vacíos o no coinciden con el tipo
btEliminar_Click | No valida si el campo Id está vació
btActualiza_Click | No se valida si no se seleccionaron los combo o se llenaron todos los datos antes de realizar un UPDATE


### **Modulo RecetaMedicamentos**
Funciones | Validaciones
----------|-------------
openConnection | Si esta cerrado, si se puede abrir la conexión
closeConnection | Si esta abierto, si se puede cerrar la conexión
executeMyQuery | Se valida si se puede hacer o no la conexión con la base de datos
button1_Click | No valida si los campos a llenar se dejan vacíos o no coinciden con el tipo

### **Modulo RegistroCompra**
Funciones | Validaciones
----------|-------------
dataGridView1_MouseClick | No se hace validación si al seleccionar un elemento de la tabla está vacío o no para que se cargue en el cuadro de texto
openConnection | Si esta cerrado, si se puede abrir la conexión
closeConnection | Si esta abierto, si se puede cerrar la conexión
executeMyQuery | Se valida si se puede hacer o no la conexión con la base de datos
btRegistro_Click | No valida si los campos a llenar se dejan vacíos o no coinciden con el tipo
btEliminar_Click | No valida si el campo Id está vació
btActualiza_Click | No se valida si no se seleccionaron los combo o se llenaron todos los datos antes de realizar un UPDATE

### **Modulo RegistroDoctores**
Funciones | Validaciones
----------|-------------
dataGridView1_MouseClick | No se hace validación si al seleccionar un elemento de la tabla está vacío o no para que se cargue en el cuadro de texto
openConnection | Si esta cerrado, si se puede abrir la conexión
closeConnection | Si esta abierto, si se puede cerrar la conexión
executeMyQuery | Se valida si se puede hacer o no la conexión con la base de datos
btRegistro_Click | No valida si los campos a llenar se dejan vacíos o no coinciden con el tipo
btEliminar_Click | No valida si el campo Id está vacío
btActualiza_Click | No se valida si no se seleccionaron los combos o se llenaron todos los datos antes de realizar un UPDATE

### **Modulo RegistroDueño**
Funciones | Validaciones
----------|-------------
dataGridView1_MouseClick | No se hace validación si al seleccionar un elemento de la tabla está vacío o no para que se cargue en el cuadro de texto
openConnection | Si esta cerrado, si se puede abrir la conexión
closeConnection | Si esta abierto, si se puede cerrar la conexión
executeMyQuery | Se valida si se puede hacer o no la conexión con la base de datos
btRegistro_Click | No valida si los campos a llenar se dejan vacíos o no coinciden con el tipo
btEliminar_Click | No valida si el campo Id está vacío
btActualiza_Click | No se valida si no se seleccionaron los combos o se llenaron todos los datos antes de realizar un UPDATE

### **Modulo RegistroPaciente**
Funciones | Validaciones
----------|-------------
dataGridView1_MouseClick | No se hace validación si al seleccionar un elemento de la tabla está vacío o no para que se cargue en el cuadro de texto
openConnection | Si esta cerrado, si se puede abrir la conexión
closeConnection | Si esta abierto, si se puede cerrar la conexión
executeMyQuery | Se valida si se puede hacer o no la conexión con la base de datos
btRegistro_Click | No valida si los campos a llenar se dejan vacíos o no coinciden con el tipo
btEliminar_Click | No valida si el campo Id está vacío
btActualiza_Click | No se valida si no se seleccionaron los combos o se llenaron todos los datos antes de realizar un UPDATE

### **Modulo RegistroProveedor**
Funciones | Validaciones
----------|-------------
dataGridView1_MouseClick | No se hace validación si al seleccionar un elemento de la tabla está vacío o no para que se cargue en el cuadro de texto
openConnection | Si esta cerrado, si se puede abrir la conexión
closeConnection | Si esta abierto, si se puede cerrar la conexión
executeMyQuery | Se valida si se puede hacer o no la conexión con la base de datos
btRegistro_Click | No valida si los campos a llenar se dejan vacíos o no coinciden con el tipo
btEliminar_Click | No valida si el campo Id está vacío
btActualiza_Click | No se valida si no se seleccionaron los combos o se llenaron todos los datos antes de realizar un UPDATE

### **Modulo RegistroVenta**
Funciones | Validaciones
----------|-------------
dataGridView1_MouseClick | No se hace validación si al seleccionar un elemento de la tabla está vacío o no para que se cargue en el cuadro de texto
openConnection | Si esta cerrado, si se puede abrir la conexión
closeConnection | Si esta abierto, si se puede cerrar la conexión
executeMyQuery | Se valida si se puede hacer o no la conexión con la base de datos
btRegistro_Click | No valida si los campos a llenar se dejan vacíos o no coinciden con el tipo
btEliminar_Click | No valida si el campo Id está vacío
btActualiza_Click | No se valida si no se seleccionaron los combos o se llenaron todos los datos antes de realizar un UPDATE

### **Modulo VentanaCompra**
Funciones | Validaciones
----------|-------------
button1_Click | Si el cuadro de texto está vacío no se aplica una validación

### **Modulo VentanaVentas**
Funciones | Validaciones
----------|-------------
button1_Click | Si el cuadro de texto está vacío no se aplica una validación



> **Norma ISO 9126** <br>
Es un estándar internacional para la evaluación de la calidad del Software. <br>
El estándar está dividido en cuatro partes las cuales dirigen realidad, métricas externas, métricas internas y calidad en las métricas de uso. <br>
El modelo de calidad establece en la primera parte del estándar, <i>ISO 9126 - 1</i> clasifica la calidad del Software en un conjunto estructurado de características y subcaracterísticas.

## Funcionalidad
Un conjunto de atributos que se relacionan con la existencia de un conjunto de funciones y sus  propiedades específicas.
* Adecuación
    * Atributos del software relacionados con la presencia y aptitud de un conjunto de funciones para tareas especificadas.
* Exactitud
    * Atributos de software relacionados con la disposición de resultados o efectos correctos.
* Interoperabilidad 
    * Atributos de software que se relacionan con su habilidad para la interacción con sistemas.
* Seguridad
    * Atributos de software relacionados con su habilidad para prevenir acceso no autorizado a programas y datos.

#### <b> Criterios para la evaluación del sistema</b>
1. Autentificación. Identidad de Usuarios <br>   
2. Autorización. Autentifica los usuarios y aplicaciones que tienen derechos definidos de acceso a los recursos del sistema.
3. Algoritmo implementado de manera correcta.
4. Funciona correctamente.
5. Manejo adecuado de la base de datos. 

## Tabla 3 Funcionalidad 

### Modulo BuscaPacientes
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
button1_Click | 5,6|6,7,5|7|5
BuscaPacientes_Load | 6|5,6,7|7|5
button2_Click | 5,6|5,6|7|7 

#### Modulo Consulta
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
Consulta_Load | 6 | 6|5,6|6
llenacombobox | 5,6 | 5 | 6| 5,7
llenacombobox2| 5,6 | 5 | 6| 5,7
button3_Click | 5 | 5 | 6| 5,6
button4_Click | 5 | 5 | 6| 5,6
openConnection|5,6,7 | 6,7|6|6,7
closeConnection|5,6,7 | 6,7|6|6,7
executeMyQuery | 4,5,6|4,5|6|5,6,7
btRegistro_Click|6| 6,7|6|7
btLimpiar_Click|5,6| 5,6 | 6|5

#### Modulo Login
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
button1_Click|3,4,5,6,7|3,4,5,6,7|3,4,5,6,7|3,4,5,6,7
btncerrar_Click | 6 | 6 | 6| 6
btnmini_Click | 6 | 6 | 5,6 | 6
txtContraseña_TextChanged |  6 | 6 | 5,6 | 6
txtUsuario_Click |  6,5 | 5,6 | 5,6 | 6
txtContraseña_Click |  6,5 | 6 | 5,6 | 6
txtContraseña_Enter | 6 | 5,6 | 5,6 | 6
Login_MouseDown | 6 | 6 | 5,6 | 6
panel1_MouseDown | 6 | 5,6 | 5,6 | 6

#### Modulo Menu
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------


#### Modulo PantallaCitas
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
dataGridView1_MouseClick |4,5,6|4,5|6|5,6,7
llenacombobox | 5,6 | 5 | 6| 5,7
llenacombobox2| 5,6 | 5 | 6| 5,7
PantallaCitas_Load|6 | 6|5,6|6
openConnection|5,6,7 | 6,7|6|6,7
closeConnection|5,6,7 | 6,7|6|6,7
executeMyQuery | 4,5,6|4,5|6|5,6,7
MuestraTabla | 6 | 6|5,6|6
btRegistro_Click|4,6| 6,7|6|7
btLimpiar_Click|5,6| 5,6 | 6|5
btEliminar_Click |4,6| 6,7|6|7
btActualiza_Click|4,6| 6,7|6|7


#### Modulo PantallaInicio
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
PantallaDeRegistros_Load | N/A| N/A|N/A|N/A
btUsuarios_Click|N/A| N/A|N/A|N/A
#### Modulo PrimerControlDeUsuario
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
dataGridView1_MouseClick | 4,5,6|4,5|6|5,6,7
llenacombobox | 5,6 | 5 | 6| 5,7
llenacombobox2| 5,6 | 5 | 6| 5,7
PrimerControlDeUsuario_Load|6 | 6|5,6|6
openConnection|5,6,7 | 6,7|6|6,7
closeConnection|5,6,7 | 6,7|6|6,7
executeMyQuery | 4,5,6|4,5|6|5,6,7
MuestraTabla | 6 | 6|5,6|6
btRegistro_Click|4,6| 6,7|6|7
btLimpiar_Click|5,6| 5,6 | 6|5
btEliminar_Click |4,6| 6,7|6|7
btActualiza_Click|4,6| 6,7|6|7


#### Modulo RecetaMedicamentos
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
dataGridView1_MouseClick | 4,5,6|4,5|6|5,6,7
llenacombobox | 5,6 | 5 | 6| 5,7
llenacombobox2| 5,6 | 5 | 6| 5,7
RecetaMedicamentos_Load|6 | 6|5,6|6
openConnection|5,6,7 | 6,7|6|6,7
closeConnection|5,6,7 | 6,7|6|6,7
executeMyQuery | 4,5,6|4,5|6|5,6,7
MuestraTabla | 6 | 6|5,6|6
btRegistro_Click|4,6| 6,7|6|7
btLimpiar_Click|5,6| 5,6 | 6|5
btEliminar_Click |4,6| 6,7|6|7
btActualiza_Click|4,6| 6,7|6|7

#### Modulo RegistroCompra
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
dataGridView1_MouseClick | 4,5,6|4,5|6|5,6,7
llenacombobox | 5,6 | 5 | 6| 5,7
llenacombobox2| 5,6 | 5 | 6| 5,7
RegistroCompra_Load|6 | 6|5,6|6
openConnection|5,6,7 | 6,7|6|6,7
closeConnection|5,6,7 | 6,7|6|6,7
executeMyQuery | 4,5,6|4,5|6|5,6,7
MuestraTabla | 6 | 6|5,6|6
btRegistro_Click|4,6| 6,7|6|7
btLimpiar_Click|5,6| 5,6 | 6|5
btEliminar_Click |4,6| 6,7|6|7
btActualiza_Click|4,6| 6,7|6|7

#### Modulo RegistroDoctores
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
dataGridView1_MouseClick | 4,5,6|4,5|6|5,6,7
llenacombobox | 5,6 | 5 | 6| 5,7
llenacombobox2| 5,6 | 5 | 6| 5,7
RegistroDoctores_Load|6 | 6|5,6|6
openConnection|5,6,7 | 6,7|6|6,7
closeConnection|5,6,7 | 6,7|6|6,7
executeMyQuery | 4,5,6|4,5|6|5,6,7
MuestraTabla | 6 | 6|5,6|6
btRegistro_Click|4,6| 6,7|6|7
btLimpiar_Click|5,6| 5,6 | 6|5
btEliminar_Click |4,6| 6,7|6|7
btActualiza_Click|4,6| 6,7|6|7
#### Modulo RegistroDueño
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
dataGridView1_MouseClick | 
llenacombobox | 5,6 | 5 | 6| 5,7
llenacombobox2| 5,6 | 5 | 6| 5,7
RegistroDueño_Load|6 | 6|5,6|6
openConnection|5,6,7 | 6,7|6|6,7
closeConnection|5,6,7 | 6,7|6|6,7
executeMyQuery | 4,5,6|4,5|6|5,6,7
MuestraTabla | 6 | 6|5,6|6
btRegistro_Click|4,6| 6,7|6|7
btLimpiar_Click|5,6| 5,6 | 6|5
btEliminar_Click |4,6| 6,7|6|7
btActualiza_Click|4,6| 6,7|6|7

#### Modulo RegistroPaciente
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
dataGridView1_MouseClick | 
llenacombobox | 5,6 | 5 | 6| 5,7
llenacombobox2| 5,6 | 5 | 6| 5,7
RegistroPaciente_Load|6 | 6|5,6|6
openConnection|5,6,7 | 6,7|6|6,7
closeConnection|5,6,7 | 6,7|6|6,7
executeMyQuery | 4,5,6|4,5|6|5,6,7
MuestraTabla | 6 | 6|5,6|6
btRegistro_Click|4,6| 6,7|6|7
btLimpiar_Click|5,6| 5,6 | 6|5
btEliminar_Click |4,6| 6,7|6|7
btActualiza_Click|4,6| 6,7|6|7


#### Modulo RegistroProveedor
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
dataGridView1_MouseClick | 
llenacombobox | 5,6 | 5 | 6| 5,7
llenacombobox2| 5,6 | 5 | 6| 5,7
RegistroProveedor_Load|6 | 6|5,6|6
openConnection|5,6,7 | 6,7|6|6,7
closeConnection|5,6,7 | 6,7|6|6,7
executeMyQuery | 4,5,6|4,5|6|5,6,7
MuestraTabla | 6 | 6|5,6|6
btRegistro_Click|4,6| 6,7|6|7
btLimpiar_Click|5,6| 5,6 | 6|5
btEliminar_Click |4,6| 6,7|6|7
btActualiza_Click|4,6| 6,7|6|7

#### Modulo RegistroVenta
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
dataGridView1_MouseClick | 
llenacombobox | 5,6 | 5 | 6| 5,7
llenacombobox2| 5,6 | 5 | 6| 5,7
RegistroVenta_Load|6 | 6|5,6|6
openConnection|5,6,7 | 6,7|6|6,7
closeConnection|5,6,7 | 6,7|6|6,7
executeMyQuery | 4,5,6|4,5|6|5,6,7
MuestraTabla | 6 | 6|5,6|6
btRegistro_Click|4,6| 6,7|6|7
btLimpiar_Click|5,6| 5,6 | 6|5
btEliminar_Click |4,6| 6,7|6|7
btActualiza_Click|4,6| 6,7|6|7

#### Modulo VentanaCompra
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
button2_Click | 6 | 6 | 6| 6
button3_Click |6 | 6 | 6| 6
button1_Click |6 | 5,6 | 6| 6,7
VentanaCompra_Load |6 | 5,6 | 6| 6,7
button4_Click | 6 | 5,6 | 5,6| 6,7

#### Modulo VentanaVentas
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------
button2_Click | 6 | 6 | 6| 5,6
button3_Click |6 | 6 | 6| 5,6
button1_Click |6 | 5,6 | 6| 5,6,7
VentanaVentas_Load |6 | 5,6 | 6| 6,7
button4_Click | 6 | 5,6 | 5,6| 6,7


## Fiabilidad
Conjunto de atributos relacionados con la capacidad del Software de mantener su nivel de presentación durante un periodo establecido.

- **Madurez:** Atributos del Software que se relacionan con la frecuencia de fallas en el software.
- **Recuperabilidad:** Atributos del software que se relacionan con la capacidad para restablecer su nivel de desempeño y recuperar los datos.
-  **Tolerancia a Fallos:** Habilidad para mantener un nivel especificado o de una operación a su interfaz especficada. 


### **Criterios para la evaluación del sistema**

'#' | Criterio
-|----------
8 | Tolerancia a fallas
9 | Respaldo a la información automáticamente cada cierto tiempo
10| Recuperación de la información
11| Solo permite valores válidos
12| Manejo de excepciones

## Tabla 4 Fiabilidad 

### Modulo BuscaPacientes
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
button1_Click | N/A | 11|8
BuscaPacientes_Load |N/A | 11|8
button2_Click |N/A | 11|8


### Modulo Consulta
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
llenacombobox | 10, 11 | 10, 11 | 11
llenacombobox2| 10, 11 | 10, 11 | 11 
button3_Click | N/A | N/A | N/A
button4_Click | N/A | N/A | N/A
openConnection|8 |  8 | 8
closeConnection| 8 |  8 | 8
executeMyQuery | 8, 11, 12 | 8, 11, 12| 8, 11, 12
btRegistro_Click |11 | 11 | 11
btLimpiar_Click | N/A | N/A | N/A

### Modulo Login
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
button1_Click | 8, 10 | 10 | 8, 11, 12
btncerrar_Click |N/A | N/A | N/A
btnmini_Click | N/A | N/A | N/A
txtContraseña_TextChanged |N/A | N/A | N/A
txtUsuario_Click |N/A | N/A | N/A
txtContraseña_Click |N/A | N/A | N/A
txtContraseña_Enter |N/A | N/A | N/A
Login_MouseDown | N/A | N/A | N/A
panel1_MouseDown | N/A | N/A | N/A
### Modulo Menu
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
button2_Click | 8,11,12 | 12 | 8
bloquear | 8,11,12 | 12 | 8,11

### Modulo PantallaCitas
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
dataGridView1_MouseClick | 10 | 10 | 10
llenacombobox |8,11,12 | 8 | 8,11
llenacombobox2 |8,11,12 | 8 | 8,11
PantallaCitas_Load | 10 | 10,11 | 10
openConnection | 8 |  8 | 8
closeConnection | 8 |  8 | 8
executeMyQuery | 8, 11, 12 | 8, 11, 12| 8, 11, 12
MuestraTabla | 8, 11, 12 | 8, 11, 12| 8, 11, 12
btRegistro_Click |11 | 11 | 11
btEliminar_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btActualiza_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btLimpiar_Click | n/a | n/a | n/a
### Modulo PantallaInicio
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
PantallaDeRegistros_Load | N/A | N/A | N/A
btUsuarios_Click |N/A | N/A | N/A

### Modulo PrimerControlDeUsuario
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
dataGridView1_MouseClick | 10 | 10 | 10
llenacombobox |8,11,12 | 8 | 8,11
llenacombobox2 |8,11,12 | 8 | 8,11
PrimerControlDeUsuario_Load | 10 | 10,11 | 10
openConnection | 8 |  8 | 8
closeConnection | 8 |  8 | 8
executeMyQuery | 8, 11, 12 | 8, 11, 12| 8, 11, 12
MuestraTabla | 8, 11, 12 | 8, 11, 12| 8, 11, 12
btRegistro_Click |11 | 11 | 11
btEliminar_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btActualiza_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btLimpiar_Click | n/a | n/a | n/a


### Modulo RecetaMedicamentos
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
dataGridView1_MouseClick | 10 | 10 | 10
llenacombobox |8,11,12 | 8 | 8,11
llenacombobox2 |8,11,12 | 8 | 8,11
RecetaMedicamentos_Load | 10 | 10,11 | 10
openConnection | 8 |  8 | 8
closeConnection | 8 |  8 | 8
executeMyQuery | 8, 11, 12 | 8, 11, 12| 8, 11, 12
MuestraTabla | 8, 11, 12 | 8, 11, 12| 8, 11, 12
btRegistro_Click |11 | 11 | 11
btEliminar_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btActualiza_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btLimpiar_Click | n/a | n/a | n/a
### Modulo RegistroCompra
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
dataGridView1_MouseClick | 10 | 10 | 10
llenacombobox |8,11,12 | 8 | 8,11
llenacombobox2 |8,11,12 | 8 | 8,11
RegistroCompra_Load | 10 | 10,11 | 10
openConnection | 8 |  8 | 8
closeConnection | 8 |  8 | 8
executeMyQuery | 8, 11, 12 | 8, 11, 12| 8, 11, 12
MuestraTabla | 8, 11, 12 | 8, 11, 12| 8, 11, 12
btRegistro_Click |11 | 11 | 11
btEliminar_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btActualiza_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btLimpiar_Click | n/a | n/a | n/a

### Modulo RegistroDoctores
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
dataGridView1_MouseClick | 10 | 10 | 10
llenacombobox |8,11,12 | 8 | 8,11
llenacombobox2 |8,11,12 | 8 | 8,11
RegistroDoctores_Load | 10 | 10,11 | 10
openConnection | 8 |  8 | 8
closeConnection | 8 |  8 | 8
executeMyQuery | 8, 11, 12 | 8, 11, 12| 8, 11, 12
MuestraTabla | 8, 11, 12 | 8, 11, 12| 8, 11, 12
btRegistro_Click |11 | 11 | 11
btEliminar_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btActualiza_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btLimpiar_Click | n/a | n/a | n/a


### Modulo RegistroDueño
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
dataGridView1_MouseClick | 10 | 10 | 10
llenacombobox |8,11,12 | 8 | 8,11
llenacombobox2 |8,11,12 | 8 | 8,11
RegistroDueño_Load | 10 | 10,11 | 10
openConnection | 8 |  8 | 8
closeConnection | 8 |  8 | 8
executeMyQuery | 8, 11, 12 | 8, 11, 12| 8, 11, 12
MuestraTabla | 8, 11, 12 | 8, 11, 12| 8, 11, 12
btRegistro_Click |11 | 11 | 11
btEliminar_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btActualiza_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btLimpiar_Click | n/a | n/a | n/a
### Modulo RegistroPaciente
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
dataGridView1_MouseClick | 10 | 10 | 10
llenacombobox |8,11,12 | 8 | 8,11
llenacombobox2 |8,11,12 | 8 | 8,11
RegistroPaciente_Load | 10 | 10,11 | 10
openConnection | 8 |  8 | 8
closeConnection | 8 |  8 | 8
executeMyQuery | 8, 11, 12 | 8, 11, 12| 8, 11, 12
MuestraTabla | 8, 11, 12 | 8, 11, 12| 8, 11, 12
btRegistro_Click |11 | 11 | 11
btEliminar_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btActualiza_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btLimpiar_Click | n/a | n/a | n/a
### Modulo RegistroProveedor
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
dataGridView1_MouseClick | 10 | 10 | 10
llenacombobox |8,11,12 | 8 | 8,11
llenacombobox2 |8,11,12 | 8 | 8,11
RegistroProveedor_Load | 10 | 10,11 | 10
openConnection | 8 |  8 | 8
closeConnection | 8 |  8 | 8
executeMyQuery | 8, 11, 12 | 8, 11, 12| 8, 11, 12
MuestraTabla | 8, 11, 12 | 8, 11, 12| 8, 11, 12
btRegistro_Click |11 | 11 | 11
btEliminar_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btActualiza_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btLimpiar_Click | n/a | n/a | n/a
### Modulo RegistroVenta
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
dataGridView1_MouseClick | 10 | 10 | 10
llenacombobox |8,11,12 | 8 | 8,11
llenacombobox2 |8,11,12 | 8 | 8,11
RegistroVenta_Load | 10 | 10,11 | 10
openConnection | 8 |  8 | 8
closeConnection | 8 |  8 | 8
executeMyQuery | 8, 11, 12 | 8, 11, 12| 8, 11, 12
MuestraTabla | 8, 11, 12 | 8, 11, 12| 8, 11, 12
btRegistro_Click |11 | 11 | 11
btEliminar_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btActualiza_Click |8, 11, 12 | 8, 11, 12| 8, 11, 12
btLimpiar_Click | n/a | n/a | n/a
### Modulo VentanaCompra
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
button2_Click |  n/a | n/a | n/a
button3_Click | n/a | n/a | n/a
button1_Click | 8, 11, 12 | 8, 11, 12| 8, 11, 12
VentanaCompra_Load | 10,11 | 10,11| 11
button4_Click | 10,11 | 11| 10,11
### Modulo VentanaVenta
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------
button2_Click |  n/a | n/a | n/a
button3_Click | n/a | n/a | n/a
button1_Click | 8, 11, 12 | 8, 11, 12| 8, 11, 12
VentanaVenta_Load | 10,11 | 10,11| 11
button4_Click | 10,11 | 11| 10,11


## Usabilidad
Conjunto de atributos relacionados con el esfuerzo necesario para su uso y en la valoración individual de tal uso, por los usuarios

- **Aprendizaje:** Se relacionan al esfuerzo de los usuarios para reconocer el concepto lógico y sus aplicaciones.
- **Comprensión:** Se relacionan al esfuerzo de los usuarios  para reconocer el concepto lógico y su comprensión.
-  **Operatividad:** Se relacionan con el esfuerzo de los usuarios para la operación y control del software. 


### **Criterios para la evaluación del sistema**

'#' | Criterio
-|----------
13 | Fácil navegación entre las interfaces del usuario
14 | Que el usuario se pueda familiarizar fácilmente con el sistema
15 | Información comprensible por el usuario
16 | Diseño coherente de todas las interfaces.
17 | Cuenta con manual de usuario
18 | Diseño atractivo visualmente


## Tabla 5 Usabilidad 
Modulo | Aprendizaje | Comprensión | Operatividad
----------|-------------|-------------|-------------
Busca Pacientes |13,14,17,18 | 13,15, 18 | 13,16,17
Consulta |13 ,17,18 | 15, 18 | 13,16
Login |13,14,15,17 |13,14,15,17 | 13,14,15,17 
Menú |13 ,17,18 | 15, 18 | 13,16
PantallaCitas |13 ,17,18 | 15, 18 | 13,16
PantallaInicio | N/A | N/A | N/A
PrimerControlDeUsuario |13 ,17,18 | 15, 18 | 13,16
Receta Medicamentos |13 ,17,18 | 15, 18 | 13,16
Registro Compra |13 ,17,18 | 15, 18 | 13,16
RegistroDoctores |13 ,17,18 | 15, 18 | 13,16
RegistroDueño | 13 ,17,18 | 15, 18 | 13,16
RegistroPaciente |13 ,17,18 | 15, 18 | 13,16
RegistroProveedor |13 ,17,18 | 15, 18 | 13,16
RegistroVenta | 13 ,17,18 | 15, 18 | 13,16
VentanaCompra |13,14 ,17,18 | 14,15, 18 | 13,14,16
VentanaVenta |13,14 ,17,18 | 14,15, 18 | 13,14,16

## Eficiencia
Conjunto de atributos relacionados en el nivel de desempeño del software y la cantidad de recursos necesarios.

- **Comportamiento en el tiempo:** Se relaciona con los tiempos de respuesta, procesamiento y el rendimiento en desempeñar su función.
- **Comportamiento de recursos:** Usar los controladores y tipos de recursos adecuados cuando el software lleva a cabo su función.

### **Criterios para la evaluación del sistema**

# | Criterio
-|----------
19 | El usuario debe de saber para qué es cada interfaz
20 | Tiempo justificado 
21 | Ejecución rápida 
22 | Utilización de pocos recursos del sistema
23 | Visualización rápida de interfaces

#### **Módulo Busca Pacientes**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
button1_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
BuscaPacientes_Load | 20, 21, 22, 23 | 20, 21, 22, 23
button2_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23

#### **Módulo Consulta**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
llenacombobox | 20, 21, 22, 23 |  20, 21, 22, 23
button3_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
button4_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
openConnection | 20, 21, 22, 23 |  20, 21, 22, 23
closeConnection | 20, 21, 22, 23 |  20, 21, 22, 23
executeMyQuery | 20, 21, 22, 23 |  20, 21, 22, 23
btRegistro_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btLimpiar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23

#### **Módulo Login** 
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
button1_Click | 20, 21, 22, 23 |  20, 21, 22, 23
btncerrar_Click | 20, 21, 22, 23 |  20, 21, 22, 23
txtUsuario_Click | 20, 21, 22, 23 |  20, 21, 22, 23

#### **Módulo Menú**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
ocultaBotones | 20, 21, 22, 23 |  20, 21, 22, 23
muestraBotones | 20, 21, 22, 23 |  20, 21, 22, 23
button1_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
button2_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btRU_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btRD_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btRP_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btRDueño_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btConsulta_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btVentas_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btCompra_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
bloquear | 20, 21, 22, 23 |  20, 21, 22, 23

#### **Módulo PantallaCitas**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
dataGridView1_MouseClick | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
llenacombobox | 20, 21, 22, 23 |  20, 21, 22, 23
llenacombobox2 | 20, 21, 22, 23 |  20, 21, 22, 23
PantallaCita_Load | 20, 21, 22, 23 |  20, 21, 22, 23
openConnection | 20, 21, 22, 23 |  20, 21, 22, 23
executeMyQuery | 20, 21, 22, 23 |  20, 21, 22, 23
MuestraTabla | 20, 21, 22, 23 |  20, 21, 22, 23
btRegistro_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btEliminar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btActualiza_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btLimpiar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23

#### **Módulo PantallaInicio**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
PantallaDeRegistros_Load | 20, 21, 22, 23 |  20, 21, 22, 23
btUsuarios_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23

#### **Módulo PrimerControlDeUsuario**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
dataGridView1_MouseClick | 20, 21, 22, 23 |  20, 21, 22, 23
PrimerControlDeUsuario_Load | 20, 21, 22, 23 |  20, 21, 22, 23
openConnection | 20, 21, 22, 23 |  20, 21, 22, 23
closeConnection | 20, 21, 22, 23 |  20, 21, 22, 23
executeMyQuery | 20, 21, 22, 23 |  20, 21, 22, 23
btRegistro_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
button2_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
button1_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btLimpiar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23

#### **Módulo RecetaMedicamentos**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
llenacombobox | 20, 21, 22, 23 |  20, 21, 22, 23
llenacombobox2 | 20, 21, 22, 23 |  20, 21, 22, 23
openConnection | 20, 21, 22, 23 |  20, 21, 22, 23
executeMyQuery | 20, 21, 22, 23 |  20, 21, 22, 23
button1_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23

#### **Módulo RegistroCompra**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
dataGridView1_MouseClick | 20, 21, 22, 23 |  20, 21, 22, 23
llenacombobox | 20, 21, 22, 23 |  20, 21, 22, 23
RegistroCompra_Load | 20, 21, 22, 23 |  20, 21, 22, 23
openConnection | 20, 21, 22, 23 |  20, 21, 22, 23
closeConnection | 20, 21, 22, 23 |  20, 21, 22, 23
executeMyQuery | 20, 21, 22, 23 |  20, 21, 22, 23
MuestraTabla | 20, 21, 22, 23 |  20, 21, 22, 23
btRegistro_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btActualiza_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btEliminar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btLimpiar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23

#### **Módulo RegistroDoctores**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
dataGridView1_MouseClick | 20, 21, 22, 23 |  20, 21, 22, 23
RegistroDoctores_Load | 20, 21, 22, 23 |  20, 21, 22, 23
openConnection | 20, 21, 22, 23 |  20, 21, 22, 23
closeConnection | 20, 21, 22, 23 |  20, 21, 22, 23
executeMyQuery | 20, 21, 22, 23 |  20, 21, 22, 23
MuestraTabla | 20, 21, 22, 23 |  20, 21, 22, 23
btRegistro_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btActualiza_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btEliminar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btLimpiar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23

#### **Módulo RegistroDueño**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
dataGridView1_MouseClick | 20, 21, 22, 23 |  20, 21, 22, 23
RegistroDueño_Load | 20, 21, 22, 23 |  20, 21, 22, 23
openConnection | 20, 21, 22, 23 |  20, 21, 22, 23
closeConnection | 20, 21, 22, 23 |  20, 21, 22, 23
executeMyQuery | 20, 21, 22, 23 |  20, 21, 22, 23
MuestraTabla | 20, 21, 22, 23 |  20, 21, 22, 23
btRegistro_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btActualiza_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btEliminar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btLimpiar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23

#### **Módulo RegistroPaciente**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
dataGridView1_MouseClick | 20, 21, 22, 23 |  20, 21, 22, 23
RegistroPaciente_Load | 20, 21, 22, 23 |  20, 21, 22, 23
openConnection | 20, 21, 22, 23 |  20, 21, 22, 23
closeConnection | 20, 21, 22, 23 |  20, 21, 22, 23
executeMyQuery | 20, 21, 22, 23 |  20, 21, 22, 23
MuestraTabla | 20, 21, 22, 23 |  20, 21, 22, 23
btRegistro_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btActualiza_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btEliminar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btLimpiar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23

#### **Módulo RegistroProveedor**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
dataGridView1_MouseClick | 20, 21, 22, 23 |  20, 21, 22, 23
RegistroProveedor_Load | 20, 21, 22, 23 |  20, 21, 22, 23
openConnection | 20, 21, 22, 23 |  20, 21, 22, 23
closeConnection | 20, 21, 22, 23 |  20, 21, 22, 23
executeMyQuery | 20, 21, 22, 23 |  20, 21, 22, 23
MuestraTabla | 20, 21, 22, 23 |  20, 21, 22, 23
btRegistro_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btActualiza_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btEliminar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btLimpiar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23

#### **Módulo RegistroVenta**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
dataGridView1_MouseClick | 20, 21, 22, 23 |  20, 21, 22, 23
RegistroVenta_Load | 20, 21, 22, 23 |  20, 21, 22, 23
openConnection | 20, 21, 22, 23 |  20, 21, 22, 23
closeConnection | 20, 21, 22, 23 |  20, 21, 22, 23
executeMyQuery | 20, 21, 22, 23 |  20, 21, 22, 23
MuestraTabla | 20, 21, 22, 23 |  20, 21, 22, 23
btRegistro_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btActualiza_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btEliminar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
btLimpiar_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
 
#### **Módulo VentanaCompra**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
button2_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
button3_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
button1_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
VentanaCompra_Load | 20, 21, 22, 23 |  20, 21, 22, 23
button4_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23

#### **Módulo VentanaVenta**
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------
button2_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
button3_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
button1_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23
VentanaVentas_Load | 20, 21, 22, 23 |  20, 21, 22, 23
button4_Click | 19, 20, 21, 22, 23 | 19, 20, 21, 22, 23

## Mantenibilidad
Atributos relacionados con la facilidad de extender, modificar, corregir errores en un sistema de software.

- **Estabilidad:** Atributos relacionados con el riesgo de efectos inesperados por modificaciones.
- **Facilidad de análisis:** Atributos relacionados con el esfuerzo necesario para el diagnostico de deficiencias a causa de fallo o identificadores de partes a modificar.
- **Facilidad de cambio:** Atributos del software relacionados con el esfuerzo necesario para la modificación, corrección de falla o cambio de ambiente.
- **Facilidad de pruebas:** Atributos del software relacionados con el esfuerzo necesario para validar el software modificado.

### **Criterios para la evaluación del sistema**

# | Criterio
-|----------
24 | Sencillo de probar una aplicación 
25 | Nombres de variables comprensibles 
26 | Documentación de funciones
27 | Sin redundancia de código
28 | Nombre de métodos de acuerdo a su función 
29 | Cuenta con manual del programador 
30 | Cuenta con documentación del sistema 
31 | Corrección sencilla de errores


#### **Módulo Busca Pacientes**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
button1_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
BuscaPacientes_Load | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
button2_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28


#### **Módulo Consulta**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
llenacombobox | 24, 25, 26, 27, 28 |  24, 25, 26, 27, 28 | 24, 25, 26, 27, 28 | 24, 25, 26, 27, 28, 31
button3_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
button4_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
openConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
closeConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
executeMyQuery | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
btRegistro_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btLimpiar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

#### **Módulo Login** 
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
button1_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btncerrar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
txtUsuario_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

#### **Módulo Menú**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
ocultaBotones | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 26, 27, 28
muestraBotones | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 26, 27, 28
button1_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
button2_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btRU_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btRD_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btRP_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btRDueño_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btConsulta_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btVentas_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btCompra_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
bloquear | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 26, 27, 28

#### **Módulo PantallaCitas**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
dataGridView1_MouseClick | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
llenacombobox | 24, 25, 26, 28 |  24, 25, 26, 28 | 24, 25, 26, 28 | 24, 25, 26, 28, 31
llenacombobox2 | 24, 25, 26, 28 |  24, 25, 26, 28 | 24, 25, 26, 28 | 24, 25, 26, 28, 31
PantallaCita_Load | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
openConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
executeMyQuery | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
MuestraTabla | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
btRegistro_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btEliminar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btActualiza_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btLimpiar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

#### **Módulo PantallaInicio**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
PantallaDeRegistros_Load | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
btUsuarios_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

#### **Módulo PrimerControlDeUsuario**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
dataGridView1_MouseClick | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
PrimerControlDeUsuario_Load | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
openConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
closeConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
executeMyQuery | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
btRegistro_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
button2_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
button1_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btLimpiar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

#### **Módulo Receta Medicamentos**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
llenacombobox | 24, 25, 26, 28 |  24, 25, 26, 28 | 24, 25, 26, 28 | 24, 25, 26, 28, 31
llenacombobox2 | 24, 25, 26, 28 |  24, 25, 26, 28 | 24, 25, 26, 28 | 24, 25, 26, 28, 31
openConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
executeMyQuery | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
button1_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

#### **Módulo RegistroCompra**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
dataGridView1_MouseClick | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
llenacombobox | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 26, 27, 28
RegistroCompra_Load | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
openConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
closeConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
executeMyQuery | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
MuestraTabla | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
btRegistro_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btActualiza_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btEliminar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btLimpiar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

#### **Módulo RegistroDoctores**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
dataGridView1_MouseClick | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
RegistroDoctores_Load | 24, 26, 28 | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 25, 26, 28
openConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
closeConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
executeMyQuery | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
MuestraTabla | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
btRegistro_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btActualiza_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btEliminar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btLimpiar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

#### **Módulo RegistroDueño**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
dataGridView1_MouseClick | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
RegistroDueño_Load | 24, 26, 28 | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 25, 26, 28
openConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
closeConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
executeMyQuery | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
MuestraTabla | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
btRegistro_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btActualiza_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btEliminar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btLimpiar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

#### **Módulo RegistroPaciente**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
dataGridView1_MouseClick | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
RegistroPaciente_Load | 24, 26, 28 | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 25, 26, 28
openConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
closeConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
executeMyQuery | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
MuestraTabla | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
btRegistro_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btActualiza_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btEliminar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btLimpiar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

#### **Módulo RegistroProveedor**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
dataGridView1_MouseClick | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
RegistroProveedor_Load | 24, 26, 28 | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 25, 26, 28
openConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
closeConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
executeMyQuery | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
MuestraTabla | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
btRegistro_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btActualiza_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btEliminar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btLimpiar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

#### **Módulo RegistroVenta**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
dataGridView1_MouseClick | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
RegistroVenta_Load | 24, 26, 28 | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 25, 26, 28
openConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
closeConnection | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
executeMyQuery | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28
MuestraTabla | 24, 25, 26, 28 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 27, 28, 31 | 24, 25, 26, 28
btRegistro_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btActualiza_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btEliminar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
btLimpiar_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

#### **Módulo VentanaCompra**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
button2_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
button3_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
button1_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
VentanaCompra_Load | 24, 26, 28 | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 25, 26, 28
button4_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

#### **Módulo VentanaVenta**
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|
button2_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
button3_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
button1_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28
VentanaVentas_Load | 24, 26, 28 | 24, 26, 27, 28, 31 | 24, 26, 27, 28, 31 | 24, 25, 26, 28
button4_Click | 24, 26, 31, 28 | 24, 26, 28, 31 | 24, 26, 28, 31 | 24, 26, 28

## Portabilidad
Atributos relacionados con la capacidad de un sistema de software para ser transferido desde una plataforma a otra.

- **Capacidad de instalación:** Esfuerzo necesario para instalar el software en un ambiente especificado.
- **Capacidad de reemplazo:** Atributos del software relacionados con la oportunidad y esfuerzo de usar el software en lugar de otro software en un ambiente de dicho software.
- **Adaptabilidad:** Adaptación a # de ambientes.
- **Co-existencia:** Coexistir con otro software independiente, en un entorno común compartiendo recursos comúnes.

### **Criterios para la evaluación del sistema**

'#' | Criterio
----| --------
32 | Es fácil de instalar
33 | El software se puede mover a través de una amplia gama de sistemas
34 | El programa trabaja con otras aplicaciones en sistemas locales y remotos
35 | Cuenta con documentación de administrador del sistema 

#### Software VetZoo
Capacidad de instalación | Capacidad de re-emplazamiento | Adaptabilidad | Co-existencia
-------------------------|-------------------------------|------------ --|---------------
33, 34 | 32, 33, 34 | 32 | 32, 33, 34 

#### Tipo de defectos
Tipo| 10 | 20 | 30 | 40 | 50 | 60 |70 |80 |90 |100
--------|----------|----------------------------------|------------|---------|--------------|-------|---------|---------|---|---|
Defecto | Defectos| Sintaxis | Construcción de Paquete de Datos | Asignación | Interfaz| Comprobación | Datos | Función | Sistema | Entorno


#### Tabla de decfetos
Numero | Tipo | Introducción| Eliminado | Tiempo de corrección | Defecto corregido
-------|------|-----------------------|-----------|----------------------|-----------------|
1 | 30|No se valida que los campos sean llenados antes de enviar|NO|45 min|NO
2 | 70|En caso de no generar la consulta no se notifica que no se encontro |NO|5 min |SI
3 | 40|Validación de tipo de dato acorde al campo |NO|15 min|NO
4 | 60|Validación al eliminar un registro |NO|10 min|NO


## Conclusiones 
El proceso de calidad de software es muy importante para un correcto desarrollo de software, el hecho de que un proyecto de software cuente con un certificado internacional de calidad habla del interés por lograr cumplir los objetivos que este tiene asignados.

Durante el desarrollo de la evaluación logramos evaluar la calidad de un proyecto de software aprendiendo los principios básicos del estándar ISO 9126 no se trata de alcanzar una calidad perfecta, sino la necesario para cada contexto de uso y del uso del software por parte de los usuarios.

También una de las cosas aprendidas fue a evaluar nuestros proyectos de software durante el desarrollo, de está forma podemos alcanzar la calidad en una fase temprana de software y no cuando este ya es entregado al cliente.

## Referencias
1. lecasabe CAPACITACIÓN PRÁCTICA. 2019. ¿Qué es la norma ISO 9126?. Recuperado de http://lecasabe.com/que-es-la-norma-iso-9126/
