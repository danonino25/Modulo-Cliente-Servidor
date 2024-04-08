# Integradora II

## contenido
<details>
  <summary>Tabla contenidos</summary>
  <ol>
    <li>
      <a href="#acerca-del-proyecto">Acerca del Proyecto</a>
      <ul>
        <li><a href="#descripción">Descripción</a></li>
        <li><a href="#objetivos">Objetivos</a></li>
        <li><a href="#organigrama">Organigrama</a></li>
        <li><a href="#diagrama-gantt">Diagrama Gantt</a></li>
      </ul>
    </li>
    <li>
      <a href="#análisis-de-la-solución">Análisis de la Solución</a>
      <ul>
        <li><a href="#requerimientos">Requerimientos</a></li>
        <li><a href="#diagrama-casos-de-uso">Diagrama de Casos de Uso</a></li>
      </ul>
    </li>
    <li>
      <a href="#diseño-de-la-solución">Diseño de la Solución</a>
      <ul>
        <li><a href="#modelo-relacional">Modelo Relacional</a></li>
        <li><a href="#diagrama-de-clases">Diagrama de Clases</a></li>
        <li><a href="#diagrama-de-componentes">Diagrama de Componentes</a></li>
      </ul>
    </li>    
    <li>
      <a href="#implementación">Implementación</a>
      <ul>
        <li><a href="#estándares-codificación">Estándares Codificación</a></li>
        <li><a href="#arquitectura">Arquitectura</a></li>
        <li><a href="#código-fuente">Código Fuente</a></li>
      </ul>
    </li>      
    <li>
      <a href="#pruebas">Pruebas</a>
      <ul>
        <li><a href="#casos-de-prueba">Casos de prueba</a></li>
        <li><a href="#ejecución">Ejecución</a></li>
      </ul>
    </li>       
    <li><a href="#guias">Guias</a></li>
    <li><a href="#contribucion">Contribución</a></li>
    <li><a href="#licencia">licencia</a></li>
    <li><a href="#contacto">Contacto</a></li>
    <li><a href="#participantes">Participantes</a></li>
  </ol>
</details>

<!-- Acerca del proyecto -->
## Acerca del módulo.
Elaboración de las siguientes funcionalidades:
  *Vista de los clientes que solicitan servicios que se encuetren en el mismo pool de aplicaciones.
  *Vista de los detalles de cada cliente mostrando sus aplicaciones y la ubicacion de su base o bases de datos.
  *Funcionalidad para generar reportes con formato ECXEL aplicando filtros a estos.

<!-- Descripción -->
#### Descripción.
El tiempo de desarrollo del proyecto abarcó un total de 2 meses y una semana.
Costo???
La calidad del entregable final se califica con un 90% del 100 que se esperaba por parte de la empresa.

<!-- Objetivos -->
#### Objetivos.

Integración de Sistemas Empresariales:

Establecer la funcionalidad para vincular los sistemas de la empresa con  cada cliente. 
Este objetivo busca lograr una integración perfecta que maximice la eficiencia operativa y la transparencia en las relaciones comerciales.

Eficiencia en la Gestión de Clientes:

Desarrollar una sólida infraestructura de administración de clientes que permita almacenar, 
organizar y gestionar eficientemente la información de cada cliente.
Esto asegura una actualización constante y precisa de los datos, facilitando la toma de decisiones informadas.

Transparencia en la Relación Comercial:

Crear un sistema robusto para definir y administrar contratos y servicios para cada cliente. 
Este objetivo garantiza una transparencia total en las relaciones comerciales, asegurando una 
prestación de servicios alineada con las expectativas del cliente.

Análisis y Optimización de Costos:

Registrar minuciosamente los costos asociados con la gestión y el soporte de sistemas para los clientes.
Este objetivo busca facilitar un análisis detallado de los costos, permitiendo una toma
de decisiones informada y la optimización de recursos.

<!-- Organigrama -->
#### Organigrama.
![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/52ae8221-27b1-480e-a9dc-40924f68bd2c)


<!-- Diagrama Gantt -->
#### Diagrama Gantt.
![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/fe1f687f-36e9-4c5b-907c-699eba13a20e)


<!-- Análisis del proyecto -->
## Análisis de la Solución.
En ésta sección se indicará los artefactos generados en base a la solución.

<!-- Requerimientos -->
#### Requerimientos.


<!-- Diagrama de Casos de Uso -->
#### Diagrama Casos de Uso.
Agregar la imagen de los Casos de Uso.



<!-- Diseño del proyecto -->
## Diseño de la Solución.
### Vista Cliente-Servidor.
#
![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/e030ef84-eaec-4c5d-8f39-020ee2002b84)

### Editar URL de acceso.
#
![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/39b9551f-052d-416e-9a5a-8e481d738fd3)

### Editar URL de servidor.
#
![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/0917e30c-75af-4607-92d0-fa80f852071c)


<!-- Modelo Relacional -->
#### Modelo Relacional.
![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/2ef86354-f56e-4cf4-964f-61431ca799cd)

<!-- Diagrama de Clases -->
#### Diagrama de Clases.
Esquema de las clases empleadas (atributos y sus métodos).



<!-- Implementación del proyecto -->
## Implementación.
En ésta sección se describe  los artefactos generados en base a la solución.

<!-- Estándares de Codificación -->
## Estándares de Codificación

### Especificaciones generales

Todo contenido agregado al sistema debe respetar lo siguiente para mantener el orden del código:
- Se trabajará en el idioma predominante en la aplicación de software.
- Todos los nombres de los objetos de base de datos deben tener coherencia con su uso, contenido o funcionalidad.
- No usar caracteres especiales o la letra 'ñ' en el nombramiento de objetos en las bases de datos.

### Bases de Datos

Los objetos de las bases de datos y ellas mismas deben ser nombrados con prefijos que 
representen el tipo de objeto que se está creando. Para nombrar las bases de datos se seguirán las reglas:
- Utilizar sustantivos.
- Usar todo en mayúsculas.
- Hacer uso del prefijo "BD".
- Usar palabras que identifiquen el objetivo de la base de datos.

Ejemplo:

[Prefijo] + [Identificador aplicativo] + [Cliente]*
BDSGCEMPRESA


### Tablas

Las tablas se deben de categorizar en grupos para su fácil identificación y control. El nombre de la tabla se deberá de conformar por un prefijo en minúsculas, mismo que se utilizará dependiendo del tipo de tabla, seguido del nombre de la tabla, para lo cual es necesario considerar que se deben nombrar utilizando sustantivos y estructura camel case, es decir, iniciando con la primera letra de cada palabra en mayúsculas y el resto en minúscula. Además de usar palabras que identifiquen a los datos que se almacenan en las tablas para identificarlas fácilmente.



Ejemplo:

| Nombre de Tabla                       | Prefijo |
|---------------------------------------|---------|
| Control de Catálogos Estáticos        | ce      |
| Control de Catálogos Parametrizables  | ct      |
| Control de Tablas de Sistema          | ts      |
| Control de Tablas de Log              | tl - tlog |
| Control de Tablas Compuestas          | tr      |
| Control de Históricos                 | th      |

Se debe definir un estándar por proyecto para controlar el agrupamiento de las tablas, estas pueden ser definidas por módulo, por ejemplo:

**SOP**

| Nombre de Tabla                        | Prefijo |
|----------------------------------------|---------|
| Control de Tablas exclusivas para Aéreo       | taer    |
| Control de Tablas exclusivas para Marítimo    | tmar    |
| Control de Tablas exclusivas para Terrestre   | tter    |




<!-- Arquitectura MVC y Middleware -->
#### Arquitectura.
![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/3e2a450e-f581-4219-a0a6-aa25ee3f9016)



<!-- Pruebas proyecto -->
## Pruebas.
En ésta sección se describe  los artefactos generados en base a la solución.

<!-- Casos de prueba -->
#### Casos de prueba.
Caso de prueba "Generar Reporte".
Caso de prueba "Visualizar sistemas por cliente".
Caso de prueba "Visualizar detalles del sistema"

<!-- Ejecución Casos de prueba -->
#### Ejecución.
Evidencia de Ejecución de Casos de prueba.




## Participantes
* [Juan Diaz Prado]()
* [Miguel Alejandro Espinoza Guzmán]()
* [Emilio Antonio Palacios Arvizu]()
* [Ana María Barrientos Guerrero]()

