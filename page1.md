# Qué es TypeScript.

JavaScript es uno de los lenguajes más populares, en parte porque ha evolucionado y mejorado a pasos agigantados en los últimos años.  

Sin embargo, Javascript en algún punto fue un lenguaje que presentaba muchos problemas para bases de código grandes, aplicaciones de gran escala y proyectos con muchos años de desarrollo.  

En 2012 en Javascript no habían clases, ni módulos, el ecosistema carecía de herramientas que optimizaran el flujo de desarrollo, derivado precisamente por las carencias del lenguaje mismo.  

2012 fue el año en que Typescript apareció (luego de 2 años de desarrollo), una solución de Microsoft para el desarrollo de aplicaciones con Javascript a gran escala, para ellos y para sus clientes. Steve Lucco y un equipo de más de 50 personas que incluía a Anders Hejlsberg, Lead Architect de C# y creador de Delphi y Turbo Pascal desarrollaron Typescript en Microsoft, un proyecto que originalmente se conoció como Strada.  

Originalmente, productos como Bing y Office 365 despertaron en Microsoft la necesidad de una mejora a JavaScript que permitiera construir productos escalables.  

Typescript es la solución a muchos de los problemas de JavaScript, está pensado para el desarrollo de aplicaciones robustas, implementando características en el lenguaje que nos permitan desarrollar herramientas más avanzadas para el desarrollo de aplicaciones. 



# Superset de JavaScript
Typescript es un superset de JavaScript. Decimos que una tecnología es un superset de un lenguaje de programación, cuando puede ejecutar programas de la tecnología, Typescript en este caso, y del lenguaje del que es el superset, JavaScript en este mismo ejemplo. En resumen, esto significa que los programas de JavaScript son programas válidos de TypeScript, a pesar de que TypeScript sea otro lenguaje de programación.  

Esta decisión fue tomada en Microsoft bajo la promesa de que las futuras versiones de Ecmascript traerían adiciones y mejoras interesantes a Javascript, esto significa que Typescript se mantiene a la vanguardia con las mejoras de JavaScript.  

Además, esto permite que uno pueda integrar Typescript en proyectos existentes de JavaScript sin tener que reimplementar todo el código del proyecto en Typescript, de hecho, es común que existan proyectos que introduzcan tanto Typescript como JavaScript.  

Por si fuera poco, uno de los beneficios adicionales de esta característica del lenguaje, es que pone a disposición el enorme ecosistema de librerías y frameworks que existen para JavaScript. Con Typescript podemos desarrollas aplicaciones con React, Vue, Angular, etc.  

# Tipado estático
La principal característica de Typescript es el tipado estático. Decimos que un lenguaje es de tipado estático cuando cumple con estas características principales:

- Las variables tienen un tipo de dato.
- Los valores sólo se pueden asignar a variables del tipo correspondiente.
  
  ```
  let edad : number; //Asignamos el tipo number para la variable edad
  edad = 20; // La variable ahora sólo puede asignar valores del tipo number

  ```
A partir de estas dos cararcteristicas principales, se derivan algunas otras como por ejemplo:

- Interfaces
- Genéricos
- Casting de datos (conversión de tipos)
- Argumentos con tipo
- Tipo de retorno para las funciones
- Mucho más
  
El contraste de estos lenguajes son los de tipado dinámico, como JavaScript, estos lenguajes suelen ser mucho más flexibles, lo que nos permite escribir código menos verboso.  

Por otro lado, los lenguajes de tipado estático se prestan a la implementación de herramientas de desarrollo más avanzadas, como:  

- Autocompletado de código  
- Recomendación de qué argumentos recibe una función  
- Recomendación de qué tipo retorna una función  
- Auto documentación del código  
- Mejor análisis para detectar errores  