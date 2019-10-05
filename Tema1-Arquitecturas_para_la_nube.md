# Ejercicios del tema Arquitecturas software para la nube .
### Ejercicio 1: 

__Buscar una aplicación de ejemplo, preferiblemente propia, y deducir qué patrón es el que usa. ¿Qué habría que hacer para evolucionar a un patrón tipo microservicios?__

Como trabajo TFG se realizo un servicio web para almacenar información genealógica de individuos y, a partir de esta, crear de manera gráfica el árbol genealógico de los mismos. El servicio tambien incluia la posibilidad de editar de manera interactiva en el árbol la información, descargar fotos del árbol a partir del gráfico y crear un fichero GEDCOM en base a los datos. 
El servicio usaba una arquitectura cliente-servidor claramente estructurada por capas ya que el servidor contenia toda la aplicación.

Para tranformar este sistema en uno basado en microservicios podríamos haber separado: el almacenamiento de información, La aplicación para edición de árboles, la funcionalidad de descargar la imagen del árbol a partir de HTML y la creación del fichero GEDCOM a partir de los datos en distintos microservicios interconectados, más escalables y fáciles de mantener.

### Ejercicio 2: 

__En la aplicación que se ha usado como ejemplo en el ejercicio anterior, ¿podría usar diferentes lenguajes? ¿Qué almacenes de datos serían los más convenientes?__

Claramente se podrian usar muchos lenguajes. Por ejemplo: JavaScript para la aplicación web de visualización de árboles, una API en Rust usando Rocket para procesar el intercambio de información, la librería imgkit de python para crear las imágenes a partir del HTML de la web o un servicio en PHP o en cualquiera de los lenguajes anteriores para generar el fichero GEDCOM. 

Como almacén para la información, dada la naturaleza de los datos, que representan información genealógica de relaciones entre personas, en mi opinion lo más adecuado sería un almacén de datos con estructura relacional como MySQL o PostgreSQL. No obstante, cualquier base de datos NoSQL podría adaptarse a esa tarea.