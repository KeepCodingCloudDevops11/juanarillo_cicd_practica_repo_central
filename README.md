# PRÁCTICA CICLO DE VIDA DE UN DESARROLLO - CICD - JUAN ARILLO

Práctica de Juan Arillo para el módulo de **Ciclo de vida de un desarrollo - CICD**.

## TABLA DE CONTENIDOS

[Descripción](#descripción)  
[Recursos](#recursos)  
[Desarrollo de la práctica](#desarrollo-de-la-práctica)  

## DESCRIPCIÓN

Este es el repositorio central para la práctica del **Ciclo de vida de un desarrollo - CICD**, en el cual se despliega una aplicación *Flask* conectada a una base de datos *Redis*, usando manifiestos de *Kubernetes* en una infraestructura local con *Kind* usando *ArgoCD*.  

La aplicación *Flask* muestra un texto con el número de veces que se ha cargado la página principal de la aplicación. La imagen de la aplicación *Flask* está en un repositorio personal de docker hub ([*Docker hub*](https://hub.docker.com/repository/docker/juanarillo/cicd_practica/general)).

El servicio de la base de datos *Redis*, sirve como persistencia del número de veces que se visita la página principal
de la aplicación.

A través de *Kind* creamos un cluster local de Kubernetes, que nos permitirá desplegar de manera automática la herramienta *ArgoCD* para la entrega continua de despliegues de *Kubernetes*, y la aplicación *Flask* ya desplegada, a través de un fichero *bash* `install.sh`.

## RECURSOS

La práctica está compuesta de los siguientes repositorios y proyectos:

- Repositorio del código de la aplicación -> <https://github.com/juarru/juanarillo_cicd_practica>  
- Repositorio de los artefactos de la release -> <https://github.com/juarru/juanarillo_cicd_practica/releases>  
- Repositorio de las imágenes generadas -> <https://hub.docker.com/repository/docker/juanarillo/cicd_practica/general>
- Proyecto de CircleCI -> <https://app.circleci.com/pipelines/github/juarru/juanarillo_cicd_practica>
- Proyecto de Sonarqube -> <https://sonarcloud.io/summary/overall?id=juarru_juanarillo_cicd_practica&branch=main>
- Repositorio de la infraestructura de despliegue -> <https://github.com/juarru/juanarillo_cicd_practica_argo>  

> **Nota:** En el `README.md` del repositorio de código y del repositorio de infraestructura, se encontrarán las instrucciones para su uso.

## DESARROLLO DE LA PRÁCTICA
