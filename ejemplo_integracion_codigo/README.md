<div align="center">

 <img src="../CI_CD/img/Bitbucket_logo.webp" width="30%"> 

# <p style="color:#2684FF"> Bitbucket </p>

</div>

<div align="justify">

## Creación de un repositorio y añadido de contenido

<br>

<p>Una vez nos hemos registrado en Bitbucket (bien sea con una cuenta de google o incluso con una cuenta de Github), el siguiente paso es crear nuestro workspace, el cual tendrá un nombre y una url única.</p>

<p>Un workspace es un espacio donde podremos agrupar todos nuestros repositorios dedicados a un tema en concreto. Es posible tener más de un workspace, lo que nos permite una mejor organización.</p>

<br>

<div align="center">

<img src="img/1.PNG">

<br><br>

<img src="img/2.PNG">

<br><br>

<img src="img/3.PNG">

</div>

<br>

<p>Una vez dentro de nuestro Workspace tendremos la opción de crear nuestro repositorio. En este apartado podremos darle un nombre al projecto para así agrupar diferentes repositorios en uno mismo. Además también tendremos la opción de proporcionar un nombre de repositorio, el tipo de acceso que tendrá el mismo, la inclusión de un README con plantilla, el nombre de la branch principal y la inclusión o no de un .gitignore.</p>

<br>

<div align="center">

<img src="img/4.PNG">

<br><br>

<img src="img/5.PNG">

</div>

<br>

<p>Una vez creado el repositorio este podrá ser clonado en remoto por medio de HTTPS o SSH.</p>

<br>

<div align="center">

<img src="img/6.PNG">

</div>

<br>

<p>Para la creación de una nueva rama en el desplegable de la izquierda se encuentra la opción de "Branches" donde podremos administrar las mismas.
Dentro de esta opción podremos especificar el tipo de rama que vamos a crear, de que otra rama hereda el contenido así como el nombre que le queremos dar.</p>

<br>

<div align="center">

<img src="img/8.PNG">

<br><br>

<img src="img/9.PNG">

</div>

<br>

<p>La siguiente característica a ver son los pull request. Una vez se haya realizado un cambio en la nueva rama y este se haya subido al repositorio remoto, se podrá hacer un pull request a otros colaboradores para revisar los cambios y aceptarlos para realizar el merge con la rama main o master.</p>

<br>

<div align="center">

<img src="img/10.PNG">

</div>

<br>

<p>En este apartado se puede poner un título al pull request, especificar que ramas se quieren mezclar, una descripción de lo que se ha hecho para que los colaboradores tengan más información, qué colaboradores deben hacer la review así como también si la rama en cuestión ha de borrarse una vez hecho el merge.</p>

<br>

<div align="center">

<img src="img/11.PNG">

</div>

<br>

<p>Una vez aprobado se puede proceder a realizar el merge. En esta parte del proceso se podrá poner un commit así como la estrategia de merge que se quiere seguir y si se ha de cerrar o no la branch.</P>

<br>

<div align="center">

<img src="img/13.PNG">

<br><br>

<img src="img/14.PNG">

</div>

<br>

## Pipelines

Como se ha mencionado en apartados anteriores, Bitbucket Cloud cuenta con una herramienta CI/CD integrada, Pipelines. Esta nos permite, a travéz de un fichero yml la automatización de procesos de integración y despliegue.

Para acceder a la creación de nuestro pipeline existen dos opciones. Se puede crear de forma manual, simplemente añadiendo un fichero yml desde cero o bien puede utilizarse las plantillas que proporciona la propia herramienta.

<br>

<div align="center">

<img src="img/15.PNG">

<br><br>

<img src="img/16.PNG">

</div>

<br>

A continuación se muestran algunas de las plantillas disponibles

<br>

<div align=="center">

<img src="img/17.PNG">

</div>

<br>

El fichero yml que se creará cuenta con una serie de apartados. En primer lugar encontramos la imágen que se va a utilizar, en este caso se trata de una máquina ubuntu, por lo que los scripts que se lanzarán serán en bash. Seguido de esto se encuentran una serie de pasos con sus propios nombres cada uno así como con el script deseado.

La última parte de este fichero corresponde a los pasos de despliegue, los cuales al igual que los anteriores tendrán un nombre, un script asociado así como triggers.

Además de todo esto, la interfaz de creación cuenta con un apartado de plantillas, opciones para añadir nuevos steps así como una amplia variedad integraciones.

<br>

<div align="center">

<img src="img/18.PNG">

</div>