---
id: general-faq
title: Preguntas frecuentes
description: Preguntas frecuentes en la red de Polygon
keywords:
  - docs
  - matic
  - polygon
  - faq
image: https://matic.network/banners/matic-network-16x9.png
---

## ¿Qué es la red de Polygon  {#what-is-polygon-network}

La red de Polygon es una solución de escalabilidad de capa 2 que logra escalar utilizando cadenas laterales para los cálculos fuera de la cadena, mientras asegura seguridad de activos y descentraliza a través de los validadores de prueba de participación PoS.

Ver también [Que es Polygon](/docs/home/polygon-basics/what-is-polygon).

## ¿Qué es una prueba de participación (PoS)? {#what-is-proof-of-stake-pos}

La prueba de participación es un sistema en el que la red de cadena de bloques tiene como objetivo lograr distribuir consenso. Cualquier persona con suficiente cantidad de tokens puede bloquear sus criptomonedas y el incentivo económico radica en el valor compartido de descentralizado de la red descentralizada. Los apilamientos individuales de sus criptomonedas validan las transacciones votando en la misma el consenso es logrado cuando una transacción o un conjunto de transacciones en bloque o un conjunto de bloques en punto de verificación recibe votos suficientes. El umbral utiliza el peso en términos de participación que viene con cada voto. Por ejemplo, en Polygon consenso se consigue al comprometer los puntos Polygon de verificación de los bloques de Polygon a la red Ethereum cuando ⅔ +1 del total apilan votos de poder para esto.

Ver también [Qué es la prueba de participación](/docs/home/polygon-basics/what-is-proof-of-stake).

## ¿Qué papel juega Polygon en la prueba de participación de la arquitectura de Polygon? {#what-role-does-proof-of-stake-play-in-the-polygon-architecture}

La capa de prueba de participación en la arquitectura de Polygon tiene los 2 propósitos siguientes:

* Actúa como capa de incentivación para mantener vivacidad de la cadena de plasma y mitigar principalmente el espinoso problema de la indisponibilidad de datos.
* Implementar las garantías de seguridad de la prueba de participación para las transiciones no cubiertas por plasma.

## ¿Cómo PoS de Polygon es diferente de otros sistemas similares? {#how-is-polygon-pos-different-from-other-similar-systems}

Es diferente en el sentido de que sirve un doble propósito: proporcionando garantías de disponibilidad de datos para la cadena de plasma que cubre las transiciones de estado a través de los predicados de plasma y la validación de la prueba de participación para los contratos inteligentes genéricos en el EVM.

La arquitectura Polygon también separa el proceso de producción de bloque y la validación en 2 capas distintas. Los validadores como productores de bloque crean bloques como el nombre sugiere en la cadena de Polygon para confirmaciones parciales más rápidas (< 2 segundos) mientras que la confirmación final se logra una vez que el punto de verificación se compromete en la cadena principal de Polygon con un cierto intervalo, periodo en el que puede variar dependiendo de múltiples factores como la congestión en Ethereum o el número de transacciones de Polygon. En condiciones ideales, será de entre 15 minutos a 1 hora.

Un punto de verificación es básicamente la raíz de Merkle de todos los bloques producidos entre intervalos. Los validadores múltiple desempeñan roles, creando bloques en el productor de bloques de capa, participando en consenso firmando todos los puntos de verificación y comprometiendo el punto de verificación cuando actúa como proponentes de bloques. La probabilidad de que un validador se convierta en productor o en proponente de bloques se basa en su relación de participación en el pool general.

## Animar al proponente de bloques a incluir todas las firmas {#encouraging-the-proposer-to-include-all-signatures}

Avalar al bono del proponente completamente, el proponente de bloques tendría que incluir todas las firmas en el punto de verificación. Debido a que el protocolo desea 2/3+1 de peso de la participación total, el punto de verificación será aceptado incluso con un 80% de votos. Sin embargo, en este caso, el proponente de bloques solo obtiene el 80% del bono calculado.

## ¿Cómo puedo generar un ticket de soporte o contribuir a la documentación de Polygon? {#how-can-i-raise-a-support-ticket-or-contribute-to-polygon-documentation}
Si cree que es necesario corregir algo en nuestra documentación o incluso desea agregar nueva información aquí, puede [plantear un asunto al repositorio de Github](https://github.com/maticnetwork/matic.js/issues). El [archivo Readme](https://github.com/maticnetwork/matic-docs/blob/master/README.md) en el repositorio también le da algunas sugerencias de como contribuir con nuestra documentación.

Si necesitas ayuda puedes siempre contactar **con nuestro equipo de soporte**.
