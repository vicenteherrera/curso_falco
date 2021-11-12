---
layout: frontpage
title: Curso Falco
description: Runtime Security en Containers y Kubernetes con Falco
---

# Runtime Security en Containers y Kubernetes con Falco

Autor: **Vicente Herrera** - [@vicen_herrera](https://twitter.com/vicen_herrera)  
Nivel: **Intermedio**  
Requisitos: Conocimientos básicos de containers y Kubernetes  
Conocimientos: <span class="badge rounded-pill bg-danger white" style="color:white">Falco</span> 
<span class="badge rounded-pill bg-danger white" style="color:white">MITRE</span>
<span class="badge rounded-pill bg-danger white" style="color:white">Kubernetes runtime security</span> 
<span class="badge rounded-pill bg-danger white" style="color:white">Cloud runtime security</span>  

## Introducción

[Falco](https://falco.org) es un sistema open source coordinado por la [Cloud Native Computing Foundation (CNCF)](https://www.cncf.io) (la misma que coordina Kubernetes) para implementar _runtime security_ a nivel de operaciones de kernel en hosts y containers, a nivel de audit log en Kubernetes, y a nivel de comandos de proveedores cloud como AWS. Se basa en un sistema de reglas que son evaluadas contra un buffer circular que almacena todas las operaciones o entradas de log conforme van llegando, en caso de una coincidencia se emite una alerta de salida que puede ser procesada. De esta forma, las reglas escritas en lenguaje también llamado _Falco_ definen las situaciones a detectar, y estas no requieren almacenar permanentemente un log sobre el que hacer consultas, sino que son procesadas al vuelo, y solo las detecciones tendrías que ser almacenadas.

Grabé este curso a principios de 2021 en colaboración con [Quantika 14](https://quantika14.com/) para ser utilizado por estudiantes en cyberseguridad, cuando trabajaba en [Sysdig](https://sysdig.com), la empresa que originalmente creó Falco y lo donó a la CNCF. En el mundo de los containers y Kubernetes el tiempo pasa muy rápido, y para finales de 2021 (fecha en la que publico en abierto este contenido), ya hay muchas cosas que han cambiado. Los contenidos de la sección 8.1 y 8.2 en especial son ahora totalmente diferentes, con el nuevo modelo de plugins de Falco que permiten detecciones de comandos cloud usando el proyecto open source. Los conceptos fundamentales y teóricos permanecen y serán de utilidad a cualquiera que quiera conocer más en general sobre seguridad runtime en containers, Kubernetes y cloud.

El contenido está formado por videos, acompañados de la presentación utilizada en cada uno en formato PDF para poder consultar con detalle las referencias. Algunos videos son demostraciones prácticas, por lo que los PDFs tan solo incluiran una breve introducción en esos casos.

## Contenidos

[**Curso Falco**](./falco/0.md){:class="solid-btn lesson"}  
[0. Metodología y requisitos](./falco/0.md){:class="solid-btn lesson"}  
[1. Runtime security e introducción a Falco](./falco/1.md){:class="solid-btn lesson"}  
[2.1. Falco para segurida en kernel](./falco/2.1.md){:class="solid-btn lesson"}  
[2.2. Instalación práctica de Falco](./falco/2.2.md){:class="solid-btn lesson"}  
[3.1. Sintaxis de reglas de Falco](./falco/3.1.md){:class="solid-btn lesson"}  
[3.2. Creando una nueva regla](./falco/3.2.md){:class="solid-btn lesson"}  
[4. MITRE ATT&CK matrix y reglas](./falco/4.md){:class="solid-btn lesson"}  
[5. Servicios gestionados de Falco](./falco/5.md){:class="solid-btn lesson"}  
[6.1. Falco para Kubernetes](./falco/6.1.md){:class="solid-btn lesson"}  
[6.2. Despliegue de Falco en Kubernetes](./falco/6.2.md){:class="solid-btn lesson"}  
[7. Utilidades adicionales](./falco/7.md){:class="solid-btn lesson"}  
[8.1. Falco en Cloud Connector](./falco/8.1.md){:class="solid-btn lesson"}  
[8.2. Instalación y uso Cloud Connector](./falco/8.2.md){:class="solid-btn lesson"}  

[Playlist todos los videos](https://www.youtube.com/watch?v=draEC1iXiRA&list=PLf_Lmegw9Mexm47vHtlAC8OSyTjjWx_LO){:class="solid-btn video"}{:target="_blank"}