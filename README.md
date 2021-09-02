# Introducción

Este repositorio contiene los recursos necesarios para la formación de AKS impartido en Sogeti durante la última parte del año 2021. Con estos recursos más el contenido de la formación en sí, son suficientes para hacer lo siguiente:

1. desarrollar dos microservicios con arquitectura DDD en C# y .Net 5, 
2. a partir de ellos crear los contenedores Docker, 
3. publicarlos en ACR (creando un ACR si es necesario),
4. configurar el despliegue a partir de un archivo YAML y
5. desplegar el cluster en AKS.

Los microservicios de ejemplo se comunicarán y uno de ellos le servirá una colección de DTOs al otro. Los tipos DTO se obtendrán de nuget.org/packages/Denczh.Literature.Dtos/.

# Contenido del repositorio

## aks-deployment.yaml

Archivo de configuración en YAML que describe el cluster Kubernetes del ejemplo.

## Denczh.Template.vsix

Plantilla para crear automáticamente la solución y los proyectos de los microservicios de ejemplo. Es un archivo ejecutable VSIX que instala la plantilla en Visual Studio. Tras la instalación, solo hay que crear un nuevo proyecto y buscar la plantilla por Denczh.

## how to deploy AKS in commands.txt

Archivo de ayuda con todos los comandos (y alguno más) correspondientes a la formación de AKS. Estos comandos son el día a día de un desarrollador de microservicios desplegados en AKS.