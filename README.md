Trabajo integrador modelo y sistemas

Descripción del proyecto

Sistema Épico es una aplicación de escritorio desarrollada en C# con Windows Forms, diseñada para administrar usuarios, políticas de seguridad y proveedores.
El sistema utiliza una base de datos SQL Server llamada Sistema_Usuarios1 para almacenar y gestionar la información.
Su principal objetivo es ofrecer una administración organizada y segura, incorporando un sistema de inicio de sesión con verificación en dos pasos mediante correo electrónico.

Objetivos

Administrar usuarios y sus respectivos roles.
Gestionar políticas de seguridad.
Administrar proveedores.
Proteger el acceso mediante validación de credenciales.
Incorporar verificación en dos pasos.
Organizar el código mediante una arquitectura de cinco capas.

Funcionalidades principales

Inicio de sesión: permite ingresar mediante usuario y contraseña.
Verificación en dos pasos: envía un código de 6 dígitos al correo electrónico registrado.
Gestión de usuarios: permite administrar las cuentas del sistema.
Roles de usuario: diferencia entre administradores y usuarios generales.
Políticas de seguridad: permite gestionar las condiciones de seguridad.
Gestión de proveedores: permite administrar la información de los proveedores.
Recuperación de contraseña: ofrece una opción para recuperar el acceso.
Preguntas de seguridad: se solicitan durante el primer ingreso.

Tecnologías utilizadas

Lenguaje: C#.
Entorno de desarrollo: Visual Studio.
Interfaz gráfica: Windows Forms.
Base de datos: Microsoft SQL Server.
Seguridad: SHA-256.
Arquitectura: programación por capas.

Estructura del proyecto

El sistema está organizado en cinco capas principales:

CapaPresentacion: contiene las ventanas y formularios que utiliza el usuario.
CapaNegocio: contiene las reglas del sistema, validaciones de contraseñas y envío de códigos por correo.
CapaDatos: administra la conexión con SQL Server y los procedimientos almacenados.
CapaEntidades: contiene las clases Usuario, Persona, Proveedor y PoliticaSeguridad.
BaseDeDatos: contiene los scripts SQL, las tablas y los procedimientos almacenados.

Requisitos del sistema

Para utilizar y ejecutar el proyecto se necesita:

Windows.
Visual Studio.
.NET compatible con el proyecto.
Microsoft SQL Server.
Conexión a internet para la verificación por correo electrónico.
Una cuenta de correo configurada para el envío de códigos.

Instalación

Descargar o clonar el repositorio desde GitHub.
Descomprimir los archivos si fueron descargados en formato ZIP.
Abrir la solución del proyecto en Visual Studio.
Verificar que estén instaladas las dependencias necesarias.
Abrir SQL Server y crear o configurar la base de datos Sistema_Usuarios1.
Ejecutar los scripts SQL incluidos en la carpeta BaseDeDatos.
Configurar la cadena de conexión para que apunte al servidor SQL Server correspondiente.
Configurar los datos necesarios para el envío de correos electrónicos.
Compilar el proyecto y ejecutarlo desde Visual Studio.

Uso del sistema

Abrir Sistema Épico
Ingresar el nombre de usuario y la contraseña
Presionar el botón “Ingresar al sistema”
Revisar el correo electrónico y obtener el código de verificación de 6 dígitos
Introducir el código en la ventana de verificación
Presionar aceptar
Si es el primer ingreso, responder las preguntas de seguridad
Acceder a la pantalla principal correspondiente al rol asignado

Seguridad

El sistema incorpora diferentes mecanismos para proteger la información:

Validación de usuario y contraseña
Hash de contraseñas mediante SHA-256
Verificación de identidad en dos pasos
Códigos de seguridad enviados por correo electrónico
Control de usuarios activos
Administración de roles y políticas de seguridad

Posibles errores

Error	Posible solución
Usuario o contraseña incorrectos	Revisar los datos ingresados
Usuario desactivado	Comunicarse con el administrador
Código incorrecto	Verificar los 6 dígitos o reenviar el código
No se pudo enviar el código	Comprobar la conexión a internet y el correo configurado
Error de conexión con SQL Server	Revisar la cadena de conexión y el estado del servidor

Pruebas

Se deben verificar los siguientes aspectos para comprobar el funcionamiento del sistema:

Inicio de sesión con credenciales correctas e incorrectas.
Verificación del código enviado por correo.
Acceso según el rol asignado.
Comportamiento de usuarios desactivados.
Funcionamiento de las preguntas de seguridad.
Conexión y comunicación con la base de datos.

Autor

Valentín Seijas
Institución: EEST N° 2.
Curso: 7mo 2da.
Materia: Modelos y Sistemas.
Profesor: Gian Franco Denaro.







