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

## Plan de precios



<br>

Hay que tener en cuenta, además, que el uso de la herramienta de integración y despliegue es independiente de la herramienta de gestión de proyectos que se esté utilizando. Esto quiere decir que Bitbucket podria utilizarse junto con CI/CD Gitlab por ejemplo, sin ningún problema.

En resumen las herramientas CI/CD simplifican el trabajo del desarollador, permitiendole definir una serie de reglas que automaticen en gran medida el flujo de trabajo posterior a la elaboración del código.

</div>
