# Prueba técnica

> Tiempo para resolver la prueba es de 2 días

A continuación, se presentan una serie de requerimientos que debes cumplir en un ejercicio práctico.

La prueba general se divide en pequeños ejercicios para evaluar, en la práctica, habilidades como:

- Pensamiento lógico.
- Resolución de problemas.
- Tiempo de desarrollo.
- Calidad del código
- Dominio de las herramientas de código

Se debe manejar migraciones, rutas, modelos, controladores, queues, commands.

> Recomendación: No es necesario terminar todos los ejercicios; lo más importante es que el o los ejercicios resueltos sean funcionales

Finalizada la prueba recuerda enviar link del proyecto o tu repositorio a [adrian.galicia@koltin.com.mx](adrian.galicia@koltin.com.mx) con tu información de contacto, un listado de los ejercicios resueltos y en el asunto colocar: FULLSTACK-INTERVIEW

![](https://i.imgur.com/YHIhHVW.png)

Imaginemos lo siguiente: Tenemos un sitio web llamado **servicios-online.demo** en el cual cualquier usuario registado puede publicar un servicio ejemplo "Aprende a hacer muebles" el cual tiene un descripción, entre otras características.

Las vistas la debes realizar en VueJS, puedes utilizar Laravel Jetstream

# Ejercicios

### 1. Chat entre usuario y anfitrión basado en un publicación.

**HABILIDADES:**

```
PHP, MYSQL, VueJS
```

**PROBLEMA:**

> Usuario **NICOLA4561** publica un servicio de **"Aprende a hacer muebles"**, Usuario **MARIA_4567** pregunta `Hola Daniel se puede mejorar un precio por 10 horas?`

**REQUERIMIENTO:**
El objetivo principal generar los recursos necesarios para recibir las peticiones necesarias para enviar el mensaje, donde se guarde los datos del usuario que emite el mensaje y el usuario que recibe el mensaje, además de fecha, hora, entre otros.

![](https://i.imgur.com/lqJOU2X.png)

### 2. Multiples Chats

**HABILIDADES:**

```
PHP, MYSQL, VueJS
```

**PROBLEMA:**

> El mismo Usuario **NICOLA4561** del problema anterior, publica otro servicio llamado **"Aprende a tocarAprende a hacer muebles"**, donde el mismo Usuario **MARIA_4567** pregunta `Hola Daniel veo que tambien enseñas Guitarra me puedes dar un descuento 10 horas de guitarra y 10 horas de carpintería`.
> ¿Por otro lado tenemos un nuevo Usuario **ROBERTO_DIAZ** el cual realiza una pregunta, `Hola Daniel tengo que llevar mi propia Guitarra?`

**REQUERIMIENTO:**
Se necesita desarrollar la lógica correspondiente en las rutas y el controlador, para que un usuario tenga la capacidad de tener varios hilos de conversación, también conocidos como "chats", relacionados con una publicación y vinculados a su perfil.

![](https://i.imgur.com/DkstVS0.png)

### 3. Paginacion y Orden.

**HABILIDADES:**

```
PHP, MYSQL
```

**PROBLEMA:**

> Tener en cuenta de que el historial del chat puede llegar a tener cientos de mensajes, por lo cual se necesita paginar en lotes de 15 mensajes. También es necesario basado en la fecha del mensaje ordenarlos desde el más reciente.

**REQUERIMIENTO:**
Es necesario desarrollar la lógica adecuada en el controlador para poder paginar los mensajes, mostrar la cantidad de mensajes en cada página y ordenarlos por fecha de manera ascendente o descendente.

### 4. Archivos adjuntos.

**HABILIDADES:**

```
PHP, MYSQL, VUEJS
```

**PROBLEMA:**

> En muchos casos los usuarios necesitaran adjuntar algún tipo de archivo “Foto, Audio” en el hilo de conversación.

**REQUERIMIENTO:**
Se requiere realizar el endpoint y lógica necesaria para utilizar la funcion [Storage](https://laravel.com/docs/8/filesystem) de laravel y poder almacenar los archivos adjuntos, relacionados al mensaje.

### 5. Comandos y colas.

**HABILIDADES:**

```
PHP, MYSQL, VUEJS
```

**PROBLEMA:**

> Los usuarios quisieran un resumen de los chats tenidos al final del día en su corre

**REQUERIMIENTO:**
Se requiere un comando que se ejecute una vez al final del día, dicho comando deberá enviar un correcto electrónico con los chats del día, el envío de correos deberá ser encolado en la cola **correos**

### Entregables:

- Un repositorio de GitHub que contenga todo el código de la aplicación.
- Un archivo README.md que explique cómo instalar y ejecutar la aplicación.
- Una lista de características adicionales que agregaría a la aplicación si tuviera más tiempo.

### Extra.

Si has llegado hasta este punto, y consideras que tienes tiempo se valora el hecho de que puedas desplegar tu proyecto en [Heroku](https://www.heroku.com/) o en cualquier servidor de tu gusto.

¡Gracias por participar!
