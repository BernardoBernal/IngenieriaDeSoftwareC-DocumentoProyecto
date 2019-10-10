# Proyecto Ingeniería de Software C

## Introducción
> VetZoo es un sistema de información enfocado a pequeñas veterinarias que buscan optimizar sus procesos administrativos. 
> 
> Es natural que dentro del desarrollo de software se busque la calidad total, por lo que es necesaria de implementación de un modelo de calidad que ayude a obtenerla. 
> 

## Objetivos

### Objetivo General

> Herramienta digital que permite automatizar y administrar el proceso que tienen las veterinarias facilitando al usuario su actividad laboral.

### Objetivos Específicos

## Módulos del proyecto

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

## Descripción de Módulos
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
btRegistro_Click | Se crea una consulta guardandola en la base de datos
btLimpiar_Click | Limpia la pantalla 


### **Modulo login**
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
btRU_Click | Evento que muetra la pantalla de registro de Usuarios
btRD_Click | Evento que muestra la pantalla de registro de Doctores
btRP_Click | Evento que muestra la pantalla de registro de Pacientes
btRDueño_Click | Evento que muestra la pantalla de registro de los dueños
btCitas_Click | Se muestra la pantalla para generar citas
btConsulta_Click | Evento que muestra la pantalla con todo lo referente a una consulta
btVentas_Click | Evento que muestra la pantalla con todo lo referente a una Venta
btCompra_Click | Evento que muestra la pantalla con todo lo referente a una Compra
bloquear | Evento que interactua con los botones para activarlos o desactivarlos


### **Modulo PantallaCitas**
Función | Descripción
--------|------------
dataGridView1_MouseClick | Evento que muestra en el cuadro de texto la celda seleccionada de la tabla 
llenacombobox | Evento que llena un combobox segun la tabla de Pacientes
llenacombobox2 | Evento que llena un combobox segun la tabla de Doctores
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
openConnection | Se genera la conexion con la base de datos
closeConnection | Se finaliza la conexion con la base de datos 
executeMyQuery| Se realiza la validación de la consulta de la base de datos
button1_Click | Se captura el evento para crear recetas


### **Modulo RegistroCompra**

Función | Descripción
--------|------------
dataGridView1_MouseClick | Evento que muestra en un cuadro de texto la celda seleccionada 
llenacombobox | Enlista los Doctores disponibles en la base de datos
RegistroCompra_Load | Evento que carga la información de la ventana
openConnection | Se genera la conexion con la base de datos
closeConnection | Se finaliza la conexion con la base de datos 
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
closeConnection | Se finaliza la conexion con la base de datos 
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
closeConnection | Se finaliza la conexion con la base de datos 
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
closeConnection | Se finaliza la conexion con la base de datos 
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
closeConnection | Se finaliza la conexion con la base de datos 
executeMyQuery| Se realiza la validación de la consulta de la base de datos
MuestraTabla | Se muestra la tabla con los datos
btRegistro_Click | Se inserta un registro en la tabla proovedor
btActualiza_Click | Se actualiza el registro de la tabla proovedor
btEliminar_Click | Se elimina el registro de la tabla paciente
btLimpiar_Click | Evento que limpia todos los cuadros de texto de la ventana

### **Modulo RegistroVenta**

Función | Descripción
--------|------------
dataGridView1_MouseClick | Evento que muestra en un cuadro de texto la celda seleccionada 
RegistroVenta_Load | Evento que carga la información al entrar a la ventana
openConnection | Se establece la conexión con la base de datos
closeConnection | Se finaliza la conexion con la base de datos 
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
--------|------------
button2_Click | Evento que muestra la ventana de proveedores
button3_Click | Evento que muestra la ventana de registro de venta
button1_Click | Evento que realiza una consulta en la tabla venta
VentanaVentas_Load | Carga de información de la ventana
button4_Click | Evento que limpia los cuadros de texto de la pantalla




## Tabla 2 Validación de Módulos
Módulo | Funciones | Validaciones
-------|-----------|-------------

## Tabla 3 Funcionalidad 
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------

## Tabla 4 Fiabilidad 
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------

## Tabla 5 Usabilidad 
Funciones | Aprendizaje | Comprensión | Operatividad
----------|-------------|-------------|-------------

## Tabla 6 Eficiencia
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------

## Tabla 7 Mantenibilidad 
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|

## Tabla 8 Portabilidad 
Funciones | Capacidad de instalación | Capacidad de re-emplazamiento | Adaptabilidad | Co-existencia
----------|--------------------------|-------------------------------|---------------|--------------