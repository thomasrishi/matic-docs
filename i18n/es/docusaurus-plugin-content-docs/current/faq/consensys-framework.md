---
id: consensys-framework
title: Consensys Marco de escalamiento
sidebar_label: Consensys Scaling Framework
description: Desarrolla tu próxima app de cadena de bloques en Polygon.
keywords:
  - docs
  - matic
image: https://matic.network/banners/matic-network-16x9.png
---
import useBaseUrl from '@docusaurus/useBaseUrl';

Este marco se deriva de las cuatro preguntas de Consensys [Para juzgar cualquier solución de escalabilidad](https://consensys.net/?p=19015&preview=true&_thumbnail_id=19017)

## ¿Quién lo opera? {#who-operates-it}
Los nodos de la red principal de Ethereum mueven o “operan” la red hacia adelante mediante la resolución de pruebas de trabajo y la creación de nuevos bloques. La solución L2 requiere un rol de “operador” similar en su red, que es el equivalente minero de la red principal de Ethereum que puede mover la red L2 hacia delante. Sin embargo, hay algunas diferencias. Por ejemplo, junto con el procesamiento y autorización de transacciones igual que un minero, un operador de L2 también puede facilitar a los usuarios entrar y salir de la propia capa de L2.

### - ¿Quién o qué es necesario para operar la red de prueba de participación de Polygon? {#who-or-what-is-required-to-operate-the-polygon-proof-of-stake-network}

La cadena de compromiso PoS de Polygon depende de un conjunto de validadores para asegurar la red. El papel de los validadores es ejecutar un nodo completo; producir bloques, validar y participar en el consenso y comprometer puntos de verificación en la cadena principal de Ethereum. Para convertirse en validador, hay que participar con sus tokens MATIC contratos de gestión de apilamiento que residen en la cadena principal de Ethereum.

Para más detalles, consulta https://docs.polygon.technology/docs/validate/validator/introduction#overview

### - ¿Cómo se convierten en operadores en la red PoS de Polygon? ¿Qué reglas cumplen? {#how-do-they-become-operators-in-the-polygon-pos-network-what-rules-do-they-abide-by}

Para convertirse en validador, hay que participar con sus tokens MATIC con apilamiento contratos de gestión que residen en la cadena principal de Ethereum.

Las recompensas se distribuyen a todos los participantes en forma proporcional a su apuesta en cada punto de control, con la excepción de que el proponente obtiene una bonificación adicional. El saldo de recompensas de los usuarios se actualiza en el contrato que se refiere mientras que reclama recompensas.

Las participaciones están en riesgo de ser reducidas en caso de que el nodo validador cometa un acto malicioso como doble firma y tiempo de inactividad de los validadores que también afecta a los vinculados delegados en ese punto de verificación.

Para más detalles, consulta https://docs.polygon.technology/docs/validate/validator/introduction#end-to-end-flow-for-a-matic-validator y https://docs.polygon.technology/docs/validate/validator/introduction#end-to-end-flow-for-a-matic-validator


### - ¿Qué suposiciones de confianza deben tener los usuarios de PoS de Polygon en relación con el operador? {#what-trust-assumptions-must-the-polygon-pos-users-make-about-the-operator}

La cadena de compromiso PoS de Polygon depende de un conjunto de validadores para asegurar la red. El papel de los validadores es ejecutar un nodo completo; producir bloques, validar y participar en el consenso y comprometer puntos de verificación en la cadena principal. Para convertirse en validador, hay que participar con sus tokens MATIC contratos de gestión de apilamiento que residen en la cadena principal. Siempre que ⅔ de la apuesta ponderada de los validadores sea honesta, la cadena progresará con precisión.

### - ¿De qué son responsables los operadores? ¿Qué poder tienen? {#what-are-the-operators-responsible-for-what-power-do-they-have}

El papel de los validadores es ejecutar un nodo completo; producir bloques, validar y participar en el consenso y comprometer puntos de verificación en la cadena principal.

Los validadores tienen la facultad de detener el progreso de la cadena, reordenar los bloques, etc. suponiendo que las ⅔ de los validadores de participaciones ponderadas no son honestas. No tienen la capacidad de cambiar el estado, los saldos de activos de los usuarios, etc.

### - ¿Cuáles son las motivaciones para convertirse en un operador de los PoS de Polygon? {#what-are-the-motivations-to-become-an-operator-of-the-polygon-pos}

Los validadores participan con sus tokens MATIC como garantía para trabajar en la seguridad de la red y a cambio de su servicio, ganar recompensas.

Para más detalles, consulta https://docs.polygon.technology/docs/validate/economics#what-is-the-incentive (en inglés).

## ¿Cómo están los datos? {#how-s-the-data}
Por definición, una tecnología de capa 2 debe crear puntos de verificación de datos incrementales en la capa 1 de una red principal (Ethereum). Entonces, nuestra preocupación es el tiempo intersticial entre esas comprobaciones de registros periódicos de la capa 1. Específicamente, ¿cómo se generan, almacenan y administran los datos de la capa 2 mientras no hay un puerto seguro de la capa 1? Estamos más preocupados por esto, porque es cuando el usuario está más alejado de la seguridad confiable de una red principal pública.

### - ¿Cuáles son las condiciones de bloqueo de PoS de Polygon? {#what-are-the-lock-up-conditions-for-polygon-pos}

En la mayoría de los patrones de diseño de tokens, el token se acuñó en Ethereum y se puede enviar a PoS de Polygon. Para mover un token de Ethereum a PoS de Polygon, el usuario tiene que bloquear fondos en un contrato en Ethereum, y los tokens correspondientes entonces se acuñan en PoS de Polygon.

Este mecanismo de relé de puente es administrado por los validadores de PoS de Polygon que necesitan que ⅔ estén de acuerdo en el evento de token bloqueado en Ethereum para acuñar la cantidad de token correspondiente en PoS de Polygon.

El retiro de activos a Ethereum es un proceso de 2 pasos en el que los tokens de activos tienen que ser primero quemados en la cadena de compromiso PoS de Polygon y luego la prueba de esta transacción de quemado tiene que ser presentada en la cadena de Ethereum.


Para más detalles, consulta https://docs.polygon.technology/docs/develop/ethereum-polygon/pos/getting-started#steps-to-use-the-pos-bridge

### - ¿Qué tan pronto están disponibles esos fondos en el PoS de Polygon? {#how-soon-are-those-funds-available-on-the-polygon-pos}

Alrededor de 7-8 minutos. Esto se realiza a través de un mecanismo de paso de mensajes que se denomina`state sync`. Más detalles aquí: https://docs.polygon.technology/docs/pos/state-sync/state-sync/

¿El PoS de Polygon proporciona soporte para los usuarios que entran sin un bloqueo de L1 (es decir, en el caso de que un usuario ingrese directamente en Polygon, entonces el usuario desea salir a la red principal de Ethereum)?

Sí, un mecanismo de puente especial se utiliza para lograr esto. Cuando el usuario desea salir a Ethereum, en lugar del método usual de desbloquear los tokens de un contrato especial, se acuña.

Puedes leer sobre ellos aquí: https://docs.polygon.technology/docs/develop/ethereum-polygon/pos/mintable-assets

### - ¿Cómo disputaría un usuario una transacción PoS de Polygon no válida? ¿Demuestra una transacción PoS de Polygon? {#how-would-a-user-dispute-an-invalid-polygon-pos-transaction-prove-a-valid-polygon-pos-transaction}

Actualmente, no hay manera de disputar en la cadena una transacción PoS de Polygon inválida. No obstante, los validadores de la cadena PoS de Polygon envían los puntos periódicos de verificación a Ethereum: puedes ver más detalles aquí: https://docs.polygon.technology/docs/pos/heimdall/modules/checkpoint/ Es posible verificar una transacción en la cadena PoS de Polygon en Ethereum mediante la construcción de una prueba de árbol de Merkle y la verificación contra los puntos de verificación periódicos que ocurren en Ethereum de la transacción PoS de Polygon y recibir raíces de los árboles de Merkle.

Una vez que un usuario de Polygon desee salir, ¿qué tan pronto estarán disponibles los fondos de la capa 1 (más o menos las ganancias o pérdidas de la capa 2) en la L1?

Aproximadamente entre 1-3 horas dependiendo de la frecuencia de los puntos de verificación (https://docs.polygon.technology/docs/pos/heimdall/modules/checkpoint/). La frecuencia es en gran medida una función del costo que los validadores están dispuestos a gastar en tarifas de gas de ETH para enviar puntos de verificación.

### - ¿Anticipas que hay proveedores de liquidez en la capa 1 dispuestos a proporcionar inmediatamente fondos canjeables L1 a los usuarios actuales de PoS de Polygon? {#do-you-anticipate-there-being-liquidity-providers-on-layer-1-willing-to-provide-immediately-redeemable-l1-funds-to-existing-polygon-pos-users}

Ya hay algunos jugadores como https://connext.network/ (ya en directo) y https://connext.network/ que están o estarán prestando este servicio. Hay varios de otros jugadores que también irán en vivo muy pronto.

## ¿Cómo está la pila? {#how-s-the-stack}
La comparación de la pila es importante para destacar lo que una capa 2 tiene o lo que no ha cambiado de la red principal de Ethereum.

### - ¿Cuánto comparte la pila PoS de Polygon con la pila de la red principal de Ethereum? {#how-much-does-the-polygon-pos-stack-share-with-the-ethereum-mainnet-stack}

Si eres un desarrollador de Ethereum, ya eres un desarrollador de PoS de Polygon. Todas las herramientas con las que estás familiarizado son compatibles con PoS de Polygon desde la caja: Truffle, Remix, Web3js y muchas, muchas más.

No hay cambios importantes en la interfaz de EVM para PoS de Polygon en relación con Ethereum.

### - ¿Dónde difiere el PoS de Polygon de la red principal de Ethereum y qué riesgos / recompensas introducen eso? {#where-does-the-polygon-pos-differ-from-ethereum-mainnet-stack-and-what-risks-rewards-does-that-introduce}

No hay cambios importantes.

## Preparandote para lo peor {#preparing-for-the-worst}
¿Cómo se preparan en el sistema PoS de Polygon para:

### - ¿Una salida masiva de los usuarios? {#a-mass-exit-of-users}

Siempre que ⅔ de los validadores sean honestos, los fondos de la cadena son seguros. En caso de que esta suposición no sea válida, en tal escenario puede suceder que la cadena pueda detener o volver a ordenar. El consenso social será necesario para reiniciar la cadena desde un estado anterior, incluyendo instantáneas del estado PoS de Polygon que se envían a través de puntos de verificación que pueden ser utilizados para hacerlo.

### - Los participantes de Polygon que intentan jugar el consenso de Polygon. Por ejemplo, ¿formando un cartel? {#polygon-participants-attempting-to-game-the-polygon-consensus-for-example-by-forming-a-cartel}

El consenso social será necesario para reiniciar la cadena de un estado anterior eliminando esos validadores y reiniciar con un nuevo conjunto de validadores, incluidas instantáneas del estado PoS de Polygon que se envían a través de puntos de verificación que pueden ser utilizados para hacerlo.


### - ¿Un error o explosión descubierto en una parte crítica de su sistema? {#a-bug-or-exploit-discovered-in-a-critical-part-of-its-system}

Se han tenido cuidado de reutilizar los componentes probados en la batalla en la construcción del sistema. Sin embargo, si hay un error o explosión en una parte crítica del sistema, restaurar la cadena a un estado anterior a través de consenso social es la ruta de solución principal.

