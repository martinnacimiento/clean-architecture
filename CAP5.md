# Programación orientada a objetos
- Las bases de una buena arquitectura es el entendimiento y aplicación de los principios del diseño orientado a objetos.
- Qué es? 
- Una respuesta es: la combinación de datos y funciones.
- Otra es: "una forma de modelar el mundo real", que es una afirmación evasiva y poco definida. No nos dice qué es OO.
- Algunas personas recurren a tres palabras mágicas para explicar la naturaleza de la OO: **encapsulación**, **herencia** y **polimorfismo**. La implicación es que OO es la mezcla adecuada de estas tres cosas, o al menos que un lenguaje OO debe soportar estas tres cosas.
- OO ciertamente depende de la idea de que los programadores se comportan lo suficientemente bien como para no circuncidar los datos **encapsulados**. Aun así, los lenguajes que dicen proporcionar OO solo han debilitado la **encapsulación** una vez perfecta que disfrutamos con C.
- La **herencia** como tal existía en C a través de un truco de upcasting que se podía hacer, pero OO nos brinda una mejor manera de hacerlo.
- Y con el polimorfismo pasa lo mismo, se lograba en lenguajes como C, que no es OO, pero se hacía con punteros a funciones, lo cual es muy difícil y peligroso de aplicar, había que seguir al pie de la letra muchas convenciones. Y en lenguajes OO, no facilita y nos salva de ese peligro el aplicar polimorfismo.
- La **arquitectura del complemento** se inventó para soportar la independencia de dispositivos de I/O, a los programadores de la época les costo llevar esta idea a sus programas porque usar punteros a funciones es peligroso. OO permite que la **arquitectura del complemento** se use en cualquier lugar, para cualquier cosa.
- **Inversión de dependencia**: El hecho de que los lenguajes OO proporcionen un polimorfismo seguro y conveniente significa que cualquier dependencia del código fuente, sin importar dónde se encuentre, puede invertirse.
- La idea es que si el código fuente de un componente cambia, solo el componente necesita ser compilado y desplegado, esto es **Desplegalibilidad independiente**.
- Si lo anterior pasa, estos pueden ser **desarrollados independientemente** por diferentes equipos.

## Conclusión
Hay varias respuestas de qué es OO, pero para el arquitecto es claro: es la habilidad, a través de usar polimorfismo, para ganar absoluto control sobre cada dependencia del código fuente en el sistema. Permite al arquitecto crear una arquitectura de complemento, en la cual los módulos que contienen políticas de alto nivel son independientes de módulos contienen detalles de bajo nivel. Los detalles de nivel bajo son relegados a módulos de complemento que pueden ser desplegados y desarrollados independientemente de los módulos que contienen políticas de alto nivel.