# Integradora II

## Módulo Cliente-Servidor
<details>
  <summary>Tabla contenidos</summary>
  <ol>
    <li>
      <a href="#acerca-del-módulo">Acerca del Módulo</a>
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
      </ul>
    </li>      
    <li>
      <a href="#pruebas">Pruebas</a>
      <ul>
        <li><a href="#casos-de-prueba">Casos de prueba</a></li>
        <li><a href="#ejecución">Ejecución</a></li>
      </ul>
    </li>       
    <li><a href="#participantes">Participantes</a></li>
  </ol>
</details>

<!-- Acerca del proyecto -->
## Acerca del módulo.
Elaboración de las siguientes funcionalidades:
  * Vista de los clientes que solicitan servicios que se encuetren en el mismo pool de aplicaciones.
  * Vista de los detalles de cada cliente mostrando sus aplicaciones y la ubicacion de su base o bases de datos.
  * Funcionalidad para generar reportes con formato EXCEL aplicando filtros a estos.

<!-- Descripción -->
#### Descripción.
El tiempo de desarrollo del proyecto abarcó un total de 2 meses y una semana.
La calidad del entregable final se califica con un 90% del 100 que se esperaba por parte de la empresa.
Tecnologías empleadas:
      * FortiClient(VPN para conexión al servidor remoto)
      * Tortoise SVN (Control de versiones y descarga del proyecto)
      * Visual Studio 2022 ( ASP.NET , C# , JQuery , JavaScript)
      * SQL Server 
      * SQL Management Studio 2019
Departamento al que afecta el módulo:
 Diseñado para el departamento de TIC's de la empresa NAD Global.
<!-- Objetivos -->
#### Objetivos.

Eficiencia en la Gestión de Clientes:

Diseñar e implementar  una interfaz que contenga una tabla con los detalles de los sistemas que se encuentran agregados a cada cliente para eficientar la administración de los datos recabados por la empresa y tener mejor accesibilidad y a su vez poder generar informes en format EXCEL.

<!-- Organigrama -->
#### Organigrama.
![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/52ae8221-27b1-480e-a9dc-40924f68bd2c)


<!-- Diagrama Gantt -->
#### Diagrama Gantt.
![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/fe1f687f-36e9-4c5b-907c-699eba13a20e)

<!-- Casos de prueba -->
#### Historias de usuario
 ##### Link a documento de historias: 
[Historias de usuario](https://docs.google.com/document/d/1HnNU9vYmhkJfOg0PqX9jHz_kT6WJYFrTD8UR35uGSiI/edit?usp=sharing)

<!-- Análisis del proyecto -->
## Análisis de la Solución.


<!-- Requerimientos -->
#### Requerimientos.
## Requerimientos Módulo Cliente-Servidor

### Requisitos Funcionales

| No. | Requisito                     | Descripción                                                                                              |
|-----|-------------------------------|----------------------------------------------------------------------------------------------------------|
| 1   | Visualización de Sistemas    | Permitir al administrador tener una vista general de los sistemas asociados a cada cliente en la matriz.  |
| 2   | Visualización de Clientes     | Mostrar de manera clara y ordenada la tabla de los clientes, con opciones de filtrado y búsqueda.       |
| 3   | Reportes de sistemas por cliente | Generar reportes de la matriz de sistemas de los clientes en formato descargable (Excel).             |

### Requisitos No Funcionales

| No. | Requisito                     | Descripción                                                                                              |
|-----|-------------------------------|----------------------------------------------------------------------------------------------------------|
| 1   | Seguridad                     | Implementar medidas de seguridad como autenticación de dos factores, encriptación de datos, etc.        |
| 2   | Rendimiento                   | Garantizar tiempos de respuesta rápidos incluso con grandes cantidades de datos en la matriz.           |
| 3   | Interfaz apegada a los estándares marcados por la empresa            | Desarrollar una interfaz de usuario amigable y fácil de usar para facilitar la navegación y la interacción. |
| 4   | Compatibilidad                | Asegurar que la aplicación sea compatible con los principales navegadores web (Chrome, Firefox, Safari, etc.). |

<!-- Diagrama de Casos de Uso -->
#### Diagrama Casos de Uso.
### Casos de Uso:

#### 1. Visualizar los sistemas para un Cliente

- **ID Caso de Uso:** CP001
- **Descripción:** Verificar que un administrador pueda visualizar los sistemas para un cliente en la matriz.
- **Precondiciones:** El administrador ha iniciado sesión y está en la sección de "Matriz".
- **Pasos:**
   1. Dar clic sobre algún cliente en la tabla de clientes.
   2. Asociar el sistema a un cliente.
- **Resultado Esperado:** El sistema debería mostrar los sistemas en la matriz asociados al cliente.

#### 2. Generar Reporte de Sistemas por Cliente

- **ID Caso de Uso:** CP002
- **Descripción:** Verificar que un administrador pueda generar un reporte de sistemas por cliente en formato Excel.
- **Precondiciones:** El administrador ha iniciado sesión y está en la sección de "Matriz" con sistemas asociados a clientes.
- **Pasos:**
   1. Seleccionar "Generar Reporte".
   2. Seleccionar el cliente para el cual se generará el reporte.
   3. Solicitar generación del reporte.
- **Resultado Esperado:** El sistema debería descargar un archivo Excel con la lista de sistemas asociados al cliente seleccionado.

#### 3. Ver Detalles de un Cliente y sus Sistemas

- **ID Caso de Uso:** CP003
- **Descripción:** Verificar que un administrador pueda ver los detalles de un cliente y sus sistemas asociados.
- **Precondiciones:** El usuario ha iniciado sesión y está en la sección de "Matriz" con clientes y sistemas existentes.
- **Pasos:**
   1. Seleccionar el cliente del cual se desea ver los detalles.
   2. El sistema muestra la información detallada del cliente y sus sistemas asociados.
- **Resultado Esperado:** El sistema debería mostrar correctamente los detalles del cliente y sus sistemas.

### Diagrama de los Casos de Uso:
#### ![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/0f007df0-8dab-4d0b-b586-44a376e3d097)


<!-- Diseño del proyecto -->
## Diseño de la Solución.
### Tabla Cliente-Servidor.
#
![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/cd13de8b-8276-4e3d-835e-ff3e501d92b4)


### Detalles de sistemas por cliente.
#
![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/2c1aa7df-5f99-4426-902f-3cb96bf03d58)


### Generar Reporte.
# 
![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/c98d9523-a5e4-4bdb-8724-cdf7dd011c3c)




<!-- Modelo Relacional -->
#### Modelo Relacional.
![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/2ef86354-f56e-4cf4-964f-61431ca799cd)

<!-- Diagrama de Clases -->
#### Diagrama de Clases.
 ##### ![image](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/6a3e2efc-cd05-49f6-8221-9e7beffb7833)




<!-- Estándares de Codificación -->
## Estándares de Codificación

[Estándares](https://docs.google.com/document/d/1i8lkzp329RRrHhN9hIkFhgoltLPJIAxOIOccSPy1zXg/edit)




<!-- Arquitectura MVC y Middleware -->
#### Arquitectura.

![mvc](https://github.com/danonino25/Modulo-Cliente-Servidor/assets/116208398/9caf3d89-e62f-4814-b2ec-feb13cb6c855)

<!-- Casos de prueba -->
#### Manual de instalación.
 ##### Link a documento del manual: 
[Manual de instalación](https://docs.google.com/document/d/1lBUvIzTdSSxOawj_YkzYLu9_1JX-7MmERs-OyJlPw4g/edit?usp=sharing)


<!-- Pruebas proyecto -->
## Pruebas.

<!-- Casos de prueba -->
#### Casos de prueba.
 ##### Link a documento de pruebas: 
[Casos de prueba](https://docs.google.com/spreadsheets/d/1HRTT9GVvqO9kPoE8oA3uWiqDFSEFTc3Vn1U7cqJfpkw/edit?usp=sharing)

<!-- Ejecución -->
#### Evidencia.
 ##### Link a documento de pruebas: 
[Casos de prueba](https://docs.google.com/document/d/1T0ipbvW1YWnb8pQBYZTPRFHQaiwXjbksTOqmbJ0Pk3E/edit?usp=sharing)

<!-- Ejecución Casos de prueba -->
#### Ejecución.
Evidencia de Ejecución de Casos de prueba.




## Participantes
* [Juan Diaz Prado]()
* [Miguel Alejandro Espinoza Guzmán]()
* [Emilio Antonio Palacios Arvizu]()
* [Ana María Barrientos Guerrero]()

