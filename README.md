<h1 align="center"> <em>¿ Que es Angular ?</em></h1>

### Descripción
Angular es uno de los frameworks más populares en el mercado de desarrollo front-end.se utiliza para construir 
aplicaciones `web,mobile o desktop`.utilizando tecnologias conocidas como:`TypeScript,HTML Y CSS`.

Utilizado para crear Single Page Applications(SPA´s) con un enfoque modular,componentes y servicios .`Angular` facilita el mantenimiento de layouts complejos y permite el aislamiento de responsabilidades de cada recurso de la aplicación.

![imagen 1](./img/img1.webp) 

Si bien el mundo del desarrollo web es dinámico y siempre evoluciona, a continuación enumeramos algunas de las buenas  prácticas que han demostrado ser valiosas para mantener proyectos robustos y faciles de mantener.

En la pagina oficial de `Angular` existe una guia de estilos, que nos puede ayudar para tener en cuenta cierto aspectos a la hora de crear nuestra aplicaciones. 

Teniendo en cuenta los conceptos básicos,la guia de estilos de Angular nos da una pauta para convenciones, nombramientos,buenas prácticas y patrones que es importante  conocer y seguir las recomendaciones que la guia nos enseña,para crear buenas  aplicaciones.

Podemos encontrar la guía en el siguiente enlace [Guía de estilos]( https://angular.io/guide/styleguide)

<h2 align="center"> <em>Buenas Prácticas</em></h2>

[1.Organización del Proyecto.](#módulos-funcionales)

[2.Estructura de Archivos.](#convenio-de-nombres)

[3.Gestión de Dependencias.](#inyección-de-dependencias)

[4.Rendimiento.](#aot-compilation)

[5.Manejo de Errores.](#logging-eficiente)

<h1 align="center"> <em>1. Organización del Proyecto:</em></h1>

  **Módulos Funcionales:**
  
   Divide tu aplicación en modulos funcionales, agrupando componentes ,servicios y artefactos relacionados.Aquí hay algunos puntos clave para entender mejor esta práctica:  

  1. **División lógica de la aplicación:** Los módulos funcionales agrupan componentes, servicios y otros artefactos relacionados que tienen un propósito común dentro de la aplicación. Por ejemplo, podrías tener un módulo para la autenticación, otro para la gestión de usuarios, otro para las funcionalidades principales de la aplicación, etc.  
  2. **Beneficios de la división:**  Al dividir la aplicación en módulos funcionales, se mejora la escalabilidad y la mantenibilidad del código. Cada módulo puede ser desarrollado, probado y mantenido de manera independiente, lo que facilita la colaboración en equipos grandes y la identificación de responsabilidades claras.  
  3. **Reutilización:** Los módulos funcionales permiten la reutilización de componentes y servicios en diferentes partes de la aplicación o en otras aplicaciones Angular. Esto promueve la consistencia en el diseño y la funcionalidad de la interfaz de usuario.    
  4. **Estructura típica de un módulo funcional:** Un módulo funcional en **Angular** generalmente incluye:  
    - `Componentes:` Para la presentación de la interfaz de usuario y la lógica relacionada.  
    - `Servicios:` Para la lógica de negocio, comunicación con APIs externas, etc.  
    - `Directivas y Pipes:` Funcionalidades adicionales para manipular la presentación de datos.  
    - `Rutas:` Si el módulo necesita gestionar sus propias rutas dentro de la aplicación.  
  5. **Importación y exportación de módulos:** En Angular, los módulos pueden importar y exportar funcionalidades, lo que permite la comunicación entre diferentes partes de la aplicación y facilita la modularidad.
  6. **Ejemplo práctico:**  Por ejemplo, en una aplicación de comercio electrónico, podrías tener un módulo funcional para la gestión de productos, otro para el carrito de compras y otro para el proceso de pago. Cada uno de estos módulos agrupa los componentes, servicios y funcionalidades relacionadas con su respectiva área.
   
   **Lazy Loading:** 
  
  Utiliza la carga diferida para módulos que no se cargan de inmediato, mejorando así el rendimiento inicial de la aplicación.

  `Lazy Loading`, o carga diferida, es un patrón de diseño que retarda la carga o inicialización de recursos en una aplicación hasta el momento en que son realmente necesarios. En el contexto de Angular, esto significa que los módulos o componentes no se cargan al iniciar la aplicación, sino que se cargan de manera asíncrona a medida que el usuario navega en la aplicación. Esto se logra utilizando el sistema de rutas de Angular.

  <h1 align="center"> <em>2.Estructura de Archivos.</em></h1>

  **Convenio de Nombres:**

  Adhiérete a un convenio de nombres consistente para archivos y carpetas.Esto simplifica la navegación y facilita la colaboración con otros desarrolladores.

  usar mayúsculas para iniciar los nombres, minúsculas, Camelcase, separar los nombres por guiones y puntos, nombrar los archivos seguidos del tipo de archivo, entre otras. 

  **Barrel Files:**

  Utilizar archivos barrel para exportar módulos, facilitando la importación de multiples elementos con una sola sentencia.

  <h2 align="center"> <em>3.Gestión de Dependencias</em></h2>

  **Inyección de Dependencias:**

 Usar la `inyección de dependencias` de Angular para facilitar la prueba unitaria y reducir el acoplamiento.

 La  inyección de dependencia está conectado al framework de Angular y se usa en todas partes para proporcionar nuevos componentes con los servicios u otras cosas que necesitan.Los componentes consumen servicios;es decir , es decir ,puede inyectar un servicio en un componente ,dándole acceso al componente en ese servicio.

 ![imagen 2](./img/injector-injects.png)

 **Lazy-Load de Librerías Externas:** 
 
 Aprovechar las capacidades de lazy-load para integrar bibliotecas de terceros solo cuando sea necesario, reduciendo así el tamaño inicial de la aplicación.

  <h1 align="center"> <em>4.Rendimiento</em></h1>

   **AOT Compilation:** 
  
  Habilitar Ahead-of-Time (AOT) Compilation para mejorar el rendimiento de la aplicación en tiempo de ejecución.

  **Change Detection OnPush:** 
  
  Aplica la estrategia OnPush para la detección de cambios en los componentes, reduciendo el número de evaluaciones innecesarias.


 <h1 align="center"> <em>5.Manejo de Errores.</em></h1>

 **Interceptor de Errores:** 
 
 Implementa un interceptor de errores para centralizar y gestionar de manera consistente los errores en toda la aplicación.

 **Logging Eficiente:** 
 
 Utiliza técnicas de logging efectivas para registrar información significativa sin afectar el rendimiento.