# Aplicación GUA2S

## Prototipo de la aplicación para el proyecto final de la asignatura de Gestión del Conocimiento en las Organizaciones (GCO) 

Este es el repositorio del prototipo del proyecto final de la asignatura de Gestión del Conocimiento en las Organizaciones, del Grado de Ingeniería Informática de la Universidad de La Laguna.

Es una aplicación colaborativa para la venta de productos típicos de Tenerife, especialmente productos con denominación de origen protegida como por ejemplo: la miel, el mojo, los quesos, piedras del Teide (dulces), etc, a los turistas/autóctonos usando las rutas principales ya existentes de autobuses para el transporte de dichas mercancías, además, permitiría el envío de mercancías entre dos paradas de la red de autobuses previo pago de un pequeño coste.

![Imagen generada con Stable Diffusion](./img/guagua.jpg)
<font size="1"> Imagen generada con Stable Diffusion</font>

## Implementación

La arquitectura que usaremos para implementar la aplicación será de stack MEAN con patrón de
diseño MVVM, interfaz REST, integración continua con Github Actions+Coveralls y desarrollo ágil con Lean Startup+SCRUM.

**MEAN**:
- MongoDB como base de datos.
- Express.js como web framework.
- Angular como frontend.
- Node.js como backend.

**MVVM**:
- Modelo Vista Vista Modelo
- Útil cuando estás trabajando con datos dinámicos y quieres actualizar solo partes de la
página web.
- La impementación elegida para dicho patrón de diseño es Flux, y ya que no existe de forma
nativa en Angular usaremos la librería NgRx.
- Se intentará implementar la programación orientada a eventos (programación reactiva) a través del uso de la librería RxJS.

**REST**:
- Arquitectura de intercomunicación que sigue el protocolo HTTP.
- Se intentará desarrollar la aplicación compatible RESTful nivel 3, si no, se usará el 2.

**JWT**:
- Para la gestión de la sesión se usarán tokens JWT.

**CI/CD y calidad del código**:
- Para la integración continua y la calidad del código se usará Github Actions con Codecov.

**Marco de trabajo**:  
Usaremos la filosofía Lean Startup como canvas y SCRUM como sistema de desarrollo ágil de software para las pinceladas, todo ello gestionado a través de Pivotal Tracker. Las ventajas ofrecidas por este modelo serán:
- Capacidad de extraer hipótesis y validarlas rápidamente.
- Facilidad para el cambio de requisitos on the fly.
- Posibilidad de ir cambiando prioridades de desarrollo de producto en función de rápidas validaciones de negocio.
- Ir creando a partir de validaciones muy rápidas.
- Conocer el ritmo y velocidad de desarrollo y cuantificar fechas de forma muy aproximada.
- Ser capaces de realizar mejoras continuas basadas en aprendizajes anteriores.