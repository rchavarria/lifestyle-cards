#[Complexity is out of code], by [Dan North] & [Jessica Kerr], at [Craft Conf 2015]

- El límite de lo que podemos refactorizar es lo que podamos mantener fresco en nuestra memoria. Jessica y Dan hablan que podemos mantener unos 47 conceptos.
- La arquitectura de un sistema representa la estructura en la comuncación del equipo que trabaja en el sistema.
- **Aprender** debe ser una tarea de primer nivel.
- Construye -> Mide -> Aprende (-> Construye) y así un ciclo. Es como describe la metodología *lean*. Hay que cerrar círculos de feedback.
- Dibujar en la misma gráfica el número de funcionalidades implementadas y el número de funcionalidades funcionando. Se puede observar como las implementadas se van incrementando en el tiempo, al principio muy deprisa, y que poco a poco el ritmo de nuevas funcionalidades va decayendo. En cuanto a las que funcionan, al principio siguen el paso de las nuevas, pero según avanza el tiempo, si no se desarrolla bien, llega un punto en el que parece que se llega a un máximo de funcionalidades que funcionan. Y no solo eso, sino que para lograr que todas las funcionalidades implementadas funcionen, hay que hacer un gran esfuerzo (parando de desarrollar nuevas funcionalidades), y esas que se arreglan tardan poco tiempo en dejar de funcionar.
- Metáfora del globo aerostático, que está *formado* por aire y piedras. Cada funcionalidad nueva es aire + piedras. Aprender sobre el sistema aporta solamente aire. Y hacer las cosas mal (deuda técnica,...) aportan solo piedras, lo que haría que el globo acabara cayendo al suelo.
- Gráfica con los distintos números de tecnologías a usar. En una fase de *exploración* está muy bien contar con un gran número de tecnologías. Este número se reducirá un poco en una nueva fase de *evaluación*, tendremos aún menos en la fase de *familiarización* (esta sería la fase en la que podríamos usar esas tecnologías en nuestro producto). En la fase de *entendimiento* existen muy pocas, y en la fase de *validación* quizá ya solo quede una, y tendremos que decidir si seguimos adelante con ella o la dejamos atrás.
- A la hora de estimar, no se pueden dar fechas concretas, solamente rangos. Dependiendo de la información con la que contemos, estos rangos podrán ser muy grandes. Lo que se puede hacer es investigar un poco sobre ciertos aspectos para poder hacer estos rangos más estrechos, y disminuir así las posibilidades de fallo.
- Trabaja en equipo.

[Complexity is out of code]: http://www.ustream.tv/recorded/61439914
[Dan North]: http://dannorth.net/blog
[Jessica Kerr]: http://blog.jessitron.com
[Craft Conf 2015]: http://craft-conf.com/2015
