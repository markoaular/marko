
1. Creando VM con Vagrant
1.1.
Vagrant es una herramienta para crear y administrar entornos de máquinas virtuales en un solo flujo de trabajo. Con un flujo de trabajo fácil de usar y enfocado en la automatización, Vagrant reduce el tiempo de configuración del entorno de desarrollo y aumenta la paridad de producción.
Un proyecto se define por el fichero de configuración Vagrantfile. Este fichero define:
    • Dónde se encuentra el directorio base del proyecto.
    • Describe el tipo de máquina y recursos que necesitamos para ejecutar nuestro proyecto, así como el software que necesitamos instalar y cómo queremos acceder a él.

Para crear este fichero en el directorio donde nos encontremos podemos ejecutar el comando:

$ vagrant init centos/7

Despues de que se crea el archivo Vagrantfile, debemos ejecutar el comando:

$ vagrant up

Vagrant usa una imagen de base, que puede clonar rápidamente a estas imágenes que se utilizan como base es a lo que se denominan boxes.

Veremos como en pocos minutos se descarga el box de Internet. Esta descarga se hace una sola vez, ya que
que estas imágenes se comparten entre todos los proyectos. Es decir cada proyecto hace referencia a un box por su nombre, en nuestro caso centos/7.
  
  
