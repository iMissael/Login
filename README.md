# Login
Ejemplo de un login.

Formulario de Login con Validación


Este proyecto implementa un sistema básico de inicio de sesión web donde el usuario ingresa su correo y contraseña. El formulario valida ambos campos utilizando expresiones regulares y muestra mensajes de error personalizados si los datos no cumplen con los requisitos. Si los datos son correctos, redirige a una nueva página.


1. HTML (index.html)
Contiene los campos de entrada para el correo electrónico y contraseña.

Utiliza etiquetas <label>, <input>, <small> y <button> para crear un formulario accesible y estructurado.

Incluye íconos mediante Font Awesome.

Llama al método validarFormulario() desde el botón de autenticación.

2. CSS (estilos.css)
Define la apariencia visual del formulario:

body: fondo azul oscuro, centrado vertical y horizontal.

.contenedor: tarjeta blanca con sombra, bordes redondeados y padding.

input: diseño limpio y uniforme para los campos.

.btn: botón estilizado con colores vivos y animación al pasar el mouse.

.alerta y small.error: muestran mensajes de validación con estilos de advertencia.

.ventana-flotante: lista para usar si se quiere mostrar mensajes flotantes tipo tooltip o advertencia extra.

.oculto: clase reutilizable para esconder elementos.

3. JavaScript (validaciones.js)
Contiene la lógica principal del formulario:

➤ validarFormulario(email, contraseña)
Ejecuta todas las validaciones al hacer clic en el botón.

Si ambas validaciones son correctas, redirige al usuario a Secundaria.html.

Si alguna falla, muestra el mensaje de alerta general.

➤ validarEmail(email)
Usa una expresión regular para validar formato de correo.

Si no es válido, muestra mensaje debajo del campo.

➤ validarContraseña(contraseña)
Valida que la contraseña tenga:

Al menos 8 caracteres.

Letras.

Números.

Símbolos especiales.

Si no cumple, muestra un mensaje de advertencia.

➤ mostrarError(id, mensaje)
Muestra el mensaje de error debajo del campo correspondiente.

➤ limpiarErrores()
Borra todos los mensajes de error antes de una nueva validación.



Ventana inicial del login.

![image](https://github.com/user-attachments/assets/53ad8ad4-74f0-4fa0-9fdc-a6e41b86b3be)


Ventana a la que nos redirige.

![image](https://github.com/user-attachments/assets/5895664b-c059-44d2-8cfa-19ec5e456bf5)
