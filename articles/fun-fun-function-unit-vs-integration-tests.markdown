# FunFunFunction: Unit vs Integration tests

[Mattias](https://twitter.com/mpjme) habla en esta ocasión de los tests,
de por qué tu aplicación debe tener tests (automáticos) y las diferencias
que hay entre tests unitarios y de integración.

[Unit vs Integration tests](https://www.youtube.com/watch?v=vqAaMVoKz1c)

## Notas

Automatizar la ejecución de los tests es **crítico**. ¿Por qué? Según tu
aplicación va creciendo, necesitas probar funcionalidades anteriores
(regression tests), y cada vez vas a necesitar más y más de estos tests.
Hasta que llega un momento en la que ya no se pueden hacer de forma
manual: muchos tests, múltiples entornos y dispositivos, cubrir las
infinitas posibilidades,...

¿Solución? Automatizarlos.

**Si no tienes tests automáticos, casi seguro que tu producto software
NO es muy bueno, casi seguro que NO tiene mucha calidad**

La diferencia básica entre tests unitarios y de integración es el aislamiento
que existe en los unitarios frente al uso de sistemas reales en los de
integración

¿Qué tienen de malo los unitarios?

1. No prueban el contrato entre componentes aislados, mientras que los de
integración sirven precisamente para esto, para comprobar que distintos
componentes funcionan juntos correctamente
2. Así que los debes de crear tú, mientras que a los de integración no les
importa lo más mínimo. Esta creación de contrato nos lleva a la Inversión
de Control y la Inyección de Dependencias.

Así pues, alguien podría decir: "Si los unitarios son tan costosos de
escribir, y no me prueban algo real, voy a probar toda mi aplicación
sólo con los de integración"

¿Qué tienen de malo los de integración?

1. Son costosos: lentos de ejecutar, muy inestables (tienen muchos puntos
de fallo) y en realidad son mucho más difíciles de escribir que los
unitarios
2. No pueden simular situaciones de fallo, cosa que los unitarios lo
hacen a la perfección
3. No te dicen dónde está el fallo cuando un test falla
4. Se suelen producir fallos intermitentes

## Conclusión

**Necesitas ambos tipos de tests**

## Notas a mano

![Notas tomadas a mano](../images/unit-vs-integration-tests-funfunfunction-taken-notes.jpg)
