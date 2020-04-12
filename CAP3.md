# PARTE2 - EMPEZANDO CON LOS LADRILLOS: PARADIGMAS DE PROGRAMACIÓN

- La arquitectura empieza con el código, por veamos sus inicios.
- En 1938, Alan Turing puso las bases de lo que se transformo en programación de computadoras. Él no fue el primero programar, sino en entender que los **programas eran simplemente datos**.
- Por 1945 Turing programaba en binario, usando loops, bifurcaciones, asignamiento, subrutinas, pilas y otras estructuras familiares.
- A fines de los 40, aparecen los **ensambladores**, salva a los programadores de escribir en binario.
- En 1951, Grace Hopper inventó A0, el primer compilador.
- En 1953 nace Fortran.
- Luego fue una incesante marea de lenguajes, COBOL, PL/1. SNOBOL, C, Pascal, C++, Java, etc.
- Otra gran revolución, fue el de los paradigmas de programación, que son formas de programar, relativamente no relacionadas a los lenguajes. Este te dice que estructuras de programación usar, y cuando usarlas. Hay 3 paradigmas (hay más si, pero el prefiere discutir eso más adelante).

# Visión general de paradigma

## Programación Estructurada
El primer paradigma ha ser adoptado (no inventado) fue este, descubierto por E.W. Dijkstra en 1968. Él mostró que el *goto* era perjudicial para la estructura del programa, por lo que lo reemplazo por constructos como *if/then/else* y *do/while/until*.

En resumen: La programación estructurada impone disciplina en la transferencia directa de control.

## Programación orientada a objetos
El segundo paradigma ha ser adoptado fue descubierto en el 1966 por Ole Johan Dahl y Kristen Nygaard. Estos dos programadores notaron que el marco de la pila de llamadas de función en el lenguaje ALGOL podría moverse a un montón, permitiendo así que las variables locales declaradas por una función existan mucho después de que la función regresó. La función se convirtió en un constructor para una clase, la local
las variables se convirtieron en variables de instancia y las funciones anidadas se convirtieron en métodos. Esto condujo inevitablemente al descubrimiento del polimorfismo a través del uso disciplinado de punteros de función.

En resumen: La programación orientada a objetos impone disciplina en la transferencia indirecta de control.

## Programación funcional
El tercer paradigma que recientemente comenzó a utilizarse fue el primero en inventarse. De hecho su invención fue anterior a la programación de computadoras. Fue el resultado directo del trabajo de Alonzo Church que 1936 inventó **1-cálculo** mientras buscaba el mismo problema matemático que motivaba a Alan Turing al mismo tiempo. Su 1-calculus es la base de LISP, inventadó por Jhon McCarthy en 1958. La noción fundamental de 1-calculus es la inmutabilidad, es decir, que los valores de los símbolos no cambian, más efectivamente significa que no ha declaración de asignamiento. De hecho algunos lenguajes funcionales tienen medios para alterar el valor de una variable, pero solo bajo una disciplina muy estricta.

En resumen: La programación funcional impone disciplina a la asignación.

# Comida para el pensamiento

- Cada paradigma elimina capacidades del programador. Ninguno de ellos agrega nuevas capacidades. Cada uno impone algún tipo de disciplina adicional que es negativa en su intención. **Los paradigmas nos dicen qué no hacer, más de lo que nos dicen qué hacer**.
- Otra forma de ver, es reconocer que cada paradigma nos quita algo. Los 3 juntos eliminan la instrucciones *goto*, punteros de función y la asignación.
- Algo más que llevarse? No, por eso dice que estos son los únicos 3 paradigmas. Desde el 1968 no nace otro paradigma.

# Conclusión
- Qué tiene que ver toda esta historia con la arquitectura? TODO.
- Utilizamos polimorfismo como mecanismo para cruzar los límites arquitectónicos
- Utilizamos la programación funcional para imponer disciplina en la ubicación y el acceso a los datos.
- Usamos programación estructurada como la base algorítmica de nuestros módulos.
- Observe qué tan bien se alinean esos tres con las tres grandes preocupaciones de la arquitectura: función, separación de componentes y gestión de datos.
