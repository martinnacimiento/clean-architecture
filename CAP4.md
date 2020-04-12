# Programación estructurada

- Dijkstra nació en 1930 en Rotterdam 1930. Sobreviviente a los bombardeos de Rotterdam durante la segunda guerra mundial, junto con la ocupación Alemana en Países Bajos, y en 1948 graduado de la secundaria con las notas más altas posibles en matemáticas, física, química y biología. En 1952 (edad 21) tomo un trabajo en el Centro de matemático como el primer programador en Países Bajos.
- En 1955, con 3 años siendo programador, y mientras era estudiante, concluyo que el desafío intelectual de la programación era mayor que el de la física teórica. Entonces eligió la programación como carrera a largo plazo.
- En 1957 Dijkstra se casa, y como es común en los ritos holandeses, tenía que declarar su profesión. Las autoridades no aceptarían "programador" como su profesión, por lo que Dijkstra declaró ser físico teórico.
- Dijkstra esta preocupado que nadie descubriera un disciplina o ciencia de programación, y por eso a él no lo tomaran en serio. Su jefe decía que Dijkstra podría ser una de las personas que descubriera tal disciplina, y así evolucionar el software a una ciencia.
- Dijkstra comenzó su carrera en la era de los tubos de vacíos, cuando las computadoras eran grandes, frágiles, lentas, poco confiables (para los estándares actuales) y extremadamente escasas. En estos primeros años, los programas eran escritos en binario o en un lenguaje ensamblador muy crudo. Las entrada tomó la forma física de cintas de papel o tarjetas perforadas. El ciclo de edición/compilación/pruebas duraba horas, sino días, en este entorno primitivo Dijkstra hizo su gran descubrimiento.

## Proof
- Dijkstra reconoció que programar era duro, y los programadores no lo hacían bien. Un programa de cualquier complejidad tenía demasiados detalles para un cerebro humano manejar sin ayuda. Pasar por alto un pequeño detalle resultaba en programas que parecía funcionar, pero fallaban de formas sorprendentes.
- La solución fue aplicar la disciplina matemática de **prueba**. Su visión fue la construcción de una jerarquía euclidiana de postulados, teoremas, corolarios y lemas. Dijkstra pensó que los programadores podrían usar esa jerarquía como lo hacen los matemáticos. En otras palabras, los programadores usarían estructuras comprobadas y las vincularían con un código que luego probarían que eran correctos.
- Por su puesto se dío cuenta que tenía que demostrar la técnica para escribir pruebas básicas de algoritmos simples.
- En esto, descubrió que ciertos uso de declaraciones *goto* evitan que los módulos se dividan recursivamente en unidades más pequeñas, evitando así el enfoque de divide y vencerás necesario para obtener pruebas razonables.
- Sin embargo otros usos de *goto* no tenían problemas. Por lo que se dió cuenta que estos buenos usos corresponden a simples estructuras de control de selección e iteración tales como *if/then/else* y *do/while*. Los módulos que usaban este tipo de estructuras de control podían ser recursivamente divididos dentro de unidades probables.
- Él sabía que la combinación de ejecución secuencial con estas estructuras eran especiales. Habían sido identificados dos años antes por Böhm y Jacopini, quienes probaron que todos los programas pueden construirse a partir de solo tres estructuras: secuencia, selección e iteración.

# La ciencia en la pruebas
- La ciencia no funciona probando declaraciones verdaderas, sino probando declaraciones falsas. Esas declaraciones que no podemos probar falsas, después de mucho esfuerzo, consideramos que son lo suficientemente verdaderas para nuestros propósitos.
- Dijkstra once said, “Testing shows the presence, not the absence, of bugs.”. In other words, a program can be proven incorrect by a test, but it cannot be proven correct. All that tests can do, after sufficient testing effort, is allow us to deem a program to be correct enough for our purposes.


# Conclusión
- La habilidad de crear unidades falseables hace al a programación estructurada valiosa.
- A nivel arquitectónico es considerado buena practica la **descomposición funcional**.
- En cada nivel, desde la función más pequeña hasta el componente más grande, es software es como una ciencia, por lo tanto, es manejado por la falsificables. **Los arquitectos se esfuerzan en definir módulos, componentes y servicios que son fácilmente falsificables(testeables)**.