<div align="justify">

<div style="background: white; padding: 2vw;">
    <img src="img/Atlassian_Bitbucket_Logo.png">
</div>

## Índice de contenidos

- [¿Qué es Bitbucket](https://github.com/javigh193/Bitbucket/tree/main#qu%C3%A9-es-bitbucket)

<ul>
<li><a href="#title1">¿Qué es Bitbucket?</a></li>
<li><a href="#title2">¿Qué son las herramientas CI/CD?</a></li>
<li><a href="#title3">¿Qué es, y dentro de que grupò de las herramientas CI/CD esta?</a></li>
<li><a href="#title4">Plan de precios</a></li>
<li><a href="#title5">Ejemplo de integración de código</a></li>
<li><a href="#title6">Ejemplo de documentación de proyectos</a></li>
<li><a href="#title7">Otras herramientas con las que se integra</a></li>
<li><a href="#title8">Comparativa con otras herramientas</a></li>
<li><a href="#title9">¿Por qué escoger esta herramienta frente a otras?</a></li>

</ul>

## <div id="title1">¿Qué es Bitbucket?</div>

Bitbucket Cloud es un servicio de 'hosting' basado en Git y una herramienta de colaboración para facilitar la coordinación de equipos de trabajo. Provee una solución completa para implementar un 'Desarrollo Continuo de Software' ( CI + CD ). 

Uno de sus puntos fuertes es su integración con Jira y Trello, ambas herramientas del mismo desarrollador que Bitbucker: Atlassian. La combinación de estas tres herramientas busca cubrir todas las necesidades de un equipo de desarrolladores en su día a día. 

## ¿Qué son las herramientas CI/CD?

CI y CD son las siglas correspondientes a Continous Integraition y Continuous Deployment.

El concepto de Continous Integretaion se basa en la automatización de la integración de nuestro código a un repositorio central, donde 
cada commit que se realiza ejecuta un conjunto de tareas o tests encargados de verificar que el código es apto para hacer un merge sobre
la rama main o master.

Por otro lado el Contious Deployment, donde todo código que se encuentra testeado se despliega automáticamente bien en un servidor de testing o en un servidor de producción.

<div align="center">

<img src="img/CI_CD.png">

</div>

<br>

Existen diversas herramientas de terceros para CI/CD como puede ser Circleci, TC, Buddy, Concourse, entre otras. Pero sin embargo, la más popular de las herramientas de integración conitnua es Jenkins.

<div align="center">

<img src="img/Jenkins_logo.svg" width="50%">

</div>

<br>

Por otro lado cada herramienta de gestión de proyectos puede tener la suya propia. En nuestro caso Atlassian (propietario de Bitbucket) cuenta con la herramienta de integración y despliegue Bamboo. Además en el caso de que el hosting se realice con Bitbucket Cloud, existe una herramienta CI/CD integrada llamada Pipelines.

<br>

<div align="center">

<img src="img/Bamboo_logo.png" width="50%">

</div>

<br>

Hay que tener en cuenta, además, que el uso de la herramienta de integración y despliegue es independiente de la herramienta de gestión de proyectos que se esté utilizando. Esto quiere decir que Bitbucket podria utilizarse junto con CI/CD Gitlab por ejemplo, sin ningún problema.

En resumen las herramientas CI/CD simplifican el trabajo del desarollador, permitiendole definir una serie de reglas que automaticen en gran medida el flujo de trabajo posterior a la elaboración del código.

## Plan de precios

Los precios varían en función del tipo de plan, la cantidad de usuarios y el tipo de hosting. Atlassian nos da una calculadora para poder indicar nuestras necesidades aproximadas y obtener una estimación instantánea de lo que nos costaría.

### Bitbucket Cloud

Tenemos tres categorías de plan: gratuito, estándar y premium.

<div style="text-align: center;">
    <img src="img/servicios_plan.png">
</div>

Si suponemos un equipo de 5 usuarios, la cantidad máxima permitida dentro de la modalidad gratuita, los saltos de precio son los siguientes.

<div style="text-align: center;">
    <img src="img/precios.png">
</div>

Un ejemplo que Atlassian nos da como referencia sería:

<div style="text-align: center;">
    <img src="img/ejemplo_tarifa.png">
</div>

En el ejemplo de factura se puede ver como se han ido contratando capacidad de usuarios a medida que se fue necesitando. Esta flexibilidad es interesante de cara a poder absorber imprevistos que surjan en el día a día del proyecto o empresa.

### Bitbucket Server

Esta opción parece ser un producto que ha dejado de tener sentido dentro de los planes de Atlassian.

<div style="text-align: center;">
    <img src="img/server.png">
</div>

Ya no venden licencias y además avisan de que dejarán de dar servicio en febrero de 2024.

### Bitbucket Data Center

Una opción en la que Atlassian esta centrando sus esfuerzos. Pensado ya para coordinar equipos de mayor  tamaño. Se pierde flexibilidad a la hora de contratar usuarios. Las primeras opciones de usuarios/precio(USD) son: 

<ul>
    <li>25 usuarios, 2.300$</li>
    <li>50 usuarios, 4.200$</li>
    <li>100 usuarios, 7.600$</li>
    <li>250 usuarios, 15.200$</li>
    <li>500 usuarios, 20.200$</li>
    <li>1000 usuarios, 30.400$</li>
</ul>

Por referencias, la cantidad máxima seleccionable es 30.000 usuarios con un coste de 910.800$.

A partir de 250 usuarios contratados se dispone de servicio de atención prioritario. 

<div style="text-align: center;">
    <img src="img/data_center.png">
</div>

### Comparativa Data Center y Cloud

Atlassian dedica una sección a dicha comparativa, ofreciendo incluso distintos niveles de detalle para diferentes tipos de usuario. Una primera comparativa a un nivel muy básico sería la siguiente:

<div style="text-align: center;">
    <img src="img/comparativa.png">
</div>

## Ejemplo integración de código

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

Una vez definido el fichero yml a utilizar, podrá ser accedido por pipelines a travéz de la plataforma. 

Para poder habilitar Pipelines se deberá habilitar primero la verificación en dos pasos.

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

<br>

Por defecto el proceso CI/CD se ejecutará tras realizar un pull request 

## Ejemplo documentación de proyecto

### Editor de documentos

Se pueden editar los documentos online. Permite obtener una previsualización de cómo se vería el documento, trabajar con diferentes sintaxis y visualizar solamente los cambios respecto al documento de partida. 

<div style="text-align: center;">
    <img src="img/menu_edicion.png">
</div>

### Wikis

Diferentes niveles de acceso
Independencia entre repositorio y wiki

<img src="img/wiki_page.PNG">

## Otras herramientas con las que se integran 

https://www.youtube.com/watch?v=slU60fbyj70
    
</div>
