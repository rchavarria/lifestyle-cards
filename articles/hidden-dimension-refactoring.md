#[Hidden dimension of refactoring], by [Michael Feathers], at [Craft Conf 2015]

- Cómo los métodos/funciones crecen/decrecen (en líneas y complejidad) con el tiempo
- La frecuencia en los cambios nos pueden informar de clases/métodos *peligrosos*, con demasiadas responsabilidades
- Puedes descubrir si varias clases cambian *a la vez* -> relacionado con Single Responsability Principle
- Open/Closed Principle: medir cuanto tiempo se queda una clase sin cambiar, o medir tiempo entre cambios (mucha frecuencia, no muy cerrada a cambios)
- Gráfica de *turbulencia*. Dos ejes: complejidad y commit hecho al repo

complejidad
^
|               ·
|        2      ·       3
|               ·
|  ····························
|               ·
|        1      ·       4
|               ·
|------------------------------>  # of commits of a class
4 zonas:
1. Pocos commits, poca complejidad: perfecto, clases pequeñas que cambian poco
2. Pocos commits, mucha complejidad: un poco malo, pueden ser clases super grandes, un gran copy&paste, complejo, pero cambia poco, por lo que no es malo del todo
3. Muchos commits, mucha complejidad: peligro, clases muy complejas que cambian constantemente (quizá porque tienen bugs y bugs, normal, al ser tan grandes)
4. Muchos commits, poca complejidad: ¿?

- Análisis del estilo de trabajo:

1. inter-commit interval: cuanto tiempo pasa entre dos commits de un programador. Los buenos, hacen muchos commits pero cambiando pocas clases cada vez. Los no tanto, hacen menos commits pero cambian más ficheros de golpe
2. *churn*: crear spagetti code, agitar, arremolinarse

[Hidden dimension of refactoring]: http://www.ustream.tv/recorded/61483799
[Michael Feathers]: https://twitter.com/mfeathers
[Craft Conf 2015]: http://craft-conf.com/2015
