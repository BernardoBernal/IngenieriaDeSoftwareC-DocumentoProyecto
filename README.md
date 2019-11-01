# **Proyecto Ingeniería de Software C** 

## **Introducción**
> VetZoo es un sistema de información enfocado a pequeñas veterinarias que buscan optimizar sus procesos administrativos. 
> 
> Es natural que dentro del desarrollo de software se busque la calidad total, por lo que es necesaria de implementación de un modelo de calidad que ayude a obtenerla. 
> 

## **Objetivos**

### **Objetivo General**

> Herramienta digital que permite automatizar y administrar el proceso que tienen las veterinarias facilitando al usuario su actividad laboral.

### **Objetivos Específicos**

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
3. Autentificación. Identidad de Usuarios <br>   
4. Autorización. Autentifica los usuarios y aplicaciones que tienen derechos definidos de acceso a los recursos del sistema.
5. Algoritmo implementado de manera correcta.
6. Funciona correctamente.
7. Manejo adecuado de la base de datos. 

## Tabla 3 Funcionalidad 

###Modulo BuscaPacientes
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
dataGridView1_MouseClick | 
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

#### Modulo PrimerControlDeUsuario
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------

#### Modulo RecetaMedicamentos
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------

#### Modulo RegistroCompra
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------

#### Modulo RegistroDoctores
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------

#### Modulo RegistroPaciente
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------

#### Modulo RegistroProveedor
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------

#### Modulo RegistroVenta
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------

#### Modulo VentanaCompra
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------

#### Modulo VentanaVentas
Funciones | Adecuación | Exactitud | Interoperatividad | Seguridad
----------|------------|-----------|-------------------|----------


## Tabla 4 Fiabilidad 
Funciones | Madurez | Recuperabilidad | Tolerancia a Fallos
----------|---------|-----------------|--------------------

## Tabla 5 Usabilidad 
Funciones | Aprendizaje | Comprensión | Operatividad
----------|-------------|-------------|-------------

## Eficiencia
Conjunto de atributos relacionados en el nivel de desempeño del software y la cantidad de recursos necesarios.

- **Comportamiento en el tiempo:** Se relaciona con los tiempos de respuesta, procesamiento y el rendimiento en desempeñar su función.
- **Comportamiento de recursos:** Usar los controladores y tipos de recursos adecuados cuando el software lleva a cabo su función.

## Tabla 6 Eficiencia
Funciones | Comportamiento en el tiempo | Comportamiento de Recursos
----------|-----------------------------|------------------

## Mantenibilidad
Atributos relacionados con la facilidad de extender, modificar, corregir errores en un sistema de software.

- **Estabilidad:** Atributos relacionados con el riesgo de efectos inesperados por modificaciones.
- **Facilidad de análisis:** Atributos relacionados con el esfuerzo necesario para el diagnostico de deficiencias a causa de fallo o identificadores de partes a modificar.
- **Facilidad de cambio:** Atributos del software relacionados con el esfuerzo necesario para la modificación, corrección de falla o cambio de ambiente.
- **Facilidad de pruebas:** Atributos del software relacionados con el esfuerzo necesario para validar el software modificado.

## Tabla 7 Mantenibilidad 
Funciones | Estabilidad | Facilidad de análisis | Facilidad de cambio | Facilidad de prueba
----------|-------------|-----------------------|-------------|-------|

## Portabilidad
Atributos relacionados con la capacidad de un sistema de software para ser transferido desde una plataforma a otra.

- **Capacidad de instalación:** Esfuerzo necesario para instalar el software en un ambiente especificado.
- **Capacidad de reemplazo:** Atributos del software relacionados con la oportunidad y esfuerzo de usar el software en lugar de otro software en un ambiente de dicho software.
- **Adaptabilidad:** Adaptación a # de ambientes.
- **Co-existencia:** Coexistir con otro software independiente, en un entorno común compartiendo recursos comúnes.

## Tabla 8 Portabilidad 
Funciones | Capacidad de instalación | Capacidad de re-emplazamiento | Adaptabilidad | Co-existencia
----------|--------------------------|-------------------------------|---------------|--------------
