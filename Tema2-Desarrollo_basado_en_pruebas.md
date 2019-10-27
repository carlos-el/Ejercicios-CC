# Ejercicios del tema Desarrollo basado en pruebas.
### Ejercicio 1: 
__Instalar alguno de los entornos virtuales de node.js (o de cualquier otro lenguaje con el que se esté familiarizado) y, con ellos, instalar la última versión existente, la versión minor más actual de la 4.x y lo mismo para la 0.11 o alguna impar (de desarrollo).__

En mi caso instalé un entorno para node.js llamado [nodeenv](https://github.com/ekalinin/nodeenv). Como indica su documentación se puede instalar facilmente con la orde 'pip3 install nodeenv'. es incluso posible instalarlo en un entorno virtual de python.
Para crear un entorno virtual con la última versión de node.js se haria con la siguiente orden: 'nodeenv nombre__de_nuestro_entorno'.
Todas las versiones de node.js disponible en el paquete se pueden listar con 'nodeenv --list'.
En este caso la versión minor más actual de la 4.x y de la 0.11 se instalarian en un entorno con las ordenes siguientes: 'nodeenv --node=4.9.1 env-4.9', 'nodeenv --node=11.15.0 env-11.15'.

### Ejercicio 2: 
__Crear una descripción del módulo usando package.json. En caso de que se trate de otro lenguaje, usar el método correspondiente.__

Para esta tarea hemos hecho uso de la orden 'npm init' y tras rellenar una serie de campos necesarios el archivo package.json se ha creado con exito. Para que la dependencia de sqlite aparezca solo es necesario instalar el paequete correspondiente con npm, aunque sqlite ya este instalado se agrega su dependencia.

### Ejercicio 3: 
__Descargar el repositorio de ejemplo anterior, instalar las herramientas necesarias (principalmente Scala y sbt) y ejecutar el ejemplo desde sbt. Alternativamente, buscar otros marcos para REST en Scala tales como Finatra o Scalatra y probar los ejemplos que se incluyan en el repositorio.__


### Ejercicio 4: 
__Para la aplicación que se está haciendo, escribir una serie de aserciones y probar que efectivamente no fallan. Añadir tests para una nueva funcionalidad, probar que falla y escribir el código para que no lo haga. A continuación, ejecutarlos desde mocha (u otro módulo de test de alto nivel), usando descripciones del test y del grupo de test de forma correcta. Si hasta ahora no has subido el código que has venido realizando a GitHub, es el momento de hacerlo, porque lo vamos a necesitar un poco más adelante.__


### Ejercicio 5: 
__Ejercicio: Haced los dos primeros pasos antes de pasar al tercero.__