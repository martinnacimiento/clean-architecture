# A Tale of two values
- Cada sistema de software tiene 2 valores diferentes para las partes interesadas: **comportamiento** y **estructura**. Los desarrolladores son responsables de ambos.
- El trabajo de un programador no es hacer que las maquinas implementen los requerimientos y arreglar cualquier bug. Es un triste equivocación.
- La estructura tiene que ver con la palabra "**software**". El software fue inventando para ser "suave". Tiene la intención de ser una forma fácil de cambiar el comportamiento de una maquina, sino lo hubiesen llamado hardware.
- La dificultad de hacer cambios debe ser proporcional solamente al **alcance del cambio**, y no a la **forma del cambio**.
- Desde el punto de vista de los stakeholders, ellos proporcionan flujos de cambios alcance aproximadamente similar. Desde el los desarrolladores, cada nueva solicitud es mas dura que la anterior, porque la forma del sistema no encaja con la forma de la solicitud. Es como intentar meter una pieza cuadrada en un agujero redondo.
- La **forma** es una metáfora. El problema por su puesto es la **arquitectura**. Donde la arquitectura mas prefiera una forma, mas duro sera encajar una nueva característica en esa estructura. Por eso **la arquitectura debe ser independiente**.
- La gran pregunta es si es mas importante que el software funcione o que sea fácil de cambiar.La mala actitud es elegir la primera, por mas que funcione al mas mínimo cambio que se requiera, no se podrá hacer y el software se vuele inútil.
- Los administrativos siempre van a preferir la funcionalidad ante la facilidad al cambio. Pero se enojan cuando solicitan cambios y los costos son altísimos para hacerlos.
- Las cosas de gran urgencia raramente son importantes, y las cosas importantes raramente son urgentes. El **comportamiento** es urgente, pero no siempre importante. La **arquitectura** es importante pero nunca urgente. Por supuesto, hay cosas que son ambas y otras que no, por lo que tenemos las siguientes prioridades:
  1. Urgente e importante.
  2. No urgente, pero importante.
  3. Urgente, pero no importante.
  4. Ni urgente ni importante.
- Note que la arquitectura del código (la cosa importante) ocupa las 2 primeras posiciones. Mientras que el comportamiento del código la primera y tercera.
- A menudo los administrativos y desarrolladores elevan los ítems en la posición 3 a la 1. Esta falla lleva a ignorar la arquitectura importante del sistema a favor de funcionalidades sin importancias del sistema.
- **La responsabilidad del desarrollador de software es asegurar la importancia de la arquitectura sobre la urgencia de funcionalidades**.
- El equipo de desarrollo de software tiene que luchar con los demás stakeholders (no olvidar que somos un stakeholder también) para asegurar la arquitectura.
- Si eres arquitecto de software, usted crea la estructura que permiten que las funcionalidades sean mas fáciles de desarrollar, modificar y extender.