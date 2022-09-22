---
id: wallet-bridge-faq
title: Billetera <>Puente Preguntas frecuentes
description: Desarrolla tu próxima app de cadena de bloques en Polygon.
keywords:
  - docs
  - matic
  - wallet
image: https://matic.network/banners/matic-network-16x9.png
---
import useBaseUrl from '@docusaurus/useBaseUrl';

## ¿Dónde puedo utilizar billetera web Matic? {#where-can-i-use-the-matic-web-wallet}
[https://wallet.polygon.technology/](https://wallet.polygon.technology/)

## ¿Cómo encuentro el contrato de token? {#how-do-i-find-the-token-contract}

Por favor comprueba [Añadir un Token Personalizado](../faq/adding-a-custom-token) articulo

## ¿Qué billeteras son compatibles actualmente? {#which-wallets-are-currently-supported}

- Metamask
- Billetera de Coinbase
- Conectar Billetera

Pronto vamos a agregar más Billeteras.

## ¿Cómo es plasma diferente de PoS? (prueba de participación) {#how-is-plasma-different-from-pos}

Plasma viene con una seguridad adicional.  Revisar: [https://docs.polygon.technology/docs/develop/ethereum-polygon/getting-started](https://docs.polygon.technology/docs/develop/ethereum-polygon/getting-started)

## ¿Qué tokens solo están disponibles en Plasma? {#what-tokens-are-only-available-on-plasma}

Tokens Polygon

## ¿Cómo depositar a una billetera de Polygon y retirar también? {#how-do-i-deposit-to-polygon-wallet-and-also-withdraw}

Estos blogs y videos son una perfecta guía para iniciar depositando y retirando: 

Documentación: [https://docs.polygon.technology/docs/develop/wallets/matic-web-wallet/web-wallet-v2-guide/#depositing-funds-from-ethereum-to-matic](https://docs.polygon.technology/docs/develop/wallets/matic-web-wallet/web-wallet-v2-guide/#depositing-funds-from-ethereum-to-matic)

Videos: [https://www.youtube.com/playlist?list=PLslsfan1R_z0Epvnqsj29V1LBAh99dzu9](https://www.youtube.com/playlist?list=PLslsfan1R_z0Epvnqsj29V1LBAh99dzu9)

## ¿Cómo cambiar a la red principal de Polygon en MetaMask? {#how-to-switch-to-polygon-mainnet-in-metamask}

Suponiendo que ya has añadido la red personalizada y RPC red principal de Polygon en tu billetera MetaMask es cómo puedes cambiar:

1. Abrir billetera MetaMask hacer clic en red desplegable para expandirlos como se muestra en la figura:

<img src={useBaseUrl("img/wallet-bridge/wallet-faq-1.png")} width="30%" height="30%" />

1. Una vez que la ventana se expande, puedes seleccionar red principal de Polygon para cambiar:

<img src={useBaseUrl("img/wallet-bridge/wallet-faq-2.png")} width="357" height="600" />

Ahora has cambiado a la red principal de Polygon.

Puede consultar este enlace si está buscando instrucciones sobre cómo agregar la red a Metamask: [https://docs.polygon.technology/docs/develop/metamask/config-polygon-on-metamask/](https://docs.polygon.technology/docs/develop/metamask/config-polygon-on-metamask/)

## ¿Cómo elegir la red principal de Polygon en Walletlink? {#how-to-choose-polygon-mainnet-in-walletlink}

Seguir la guía proporcionada [aquí](https://docs.polygon.technology/docs/develop/metamask/config-polygon-on-wallets#configure-polygon-on-walletlink)

## He depositado en WETH, pero no lo veo en MetaMask. ¿Qué hago? {#i-have-deposited-weth-but-i-don-t-see-it-on-metamask-what-do-i-do}

Necesitas agregar manualmente el token personalizado de la dirección de WETH a MetaMask.

Abrir MetaMask y desplazarse hacia abajo para hacer clic en **Importar tokens**.

<img src={useBaseUrl("img/wallet-bridge/wallet-faq-3.png")} width="357" height="600" />


Luego, agregar la dirección del contrato pertinente, el símbolo y la precisión decimal. Las direcciones de contrato (PoS-WETH en este caso) se pueden encontrar en este enlace [https://docs.polygon.technology/docs/develop/network-details/mapped-tokens/](https://docs.polygon.technology/docs/develop/network-details/mapped-tokens/). Tendrás que agregar la dirección secundaria del token para ver los saldos en la red principal de Polygon. El Decimal de precisión es de 18 para WETH (en general, para la mayoría de los tokens decimales de precisión es 18).

Una vez que rellenes todos los campos, puedes hacer clic en **Añadir Token personalizado** y tu token será agregado.

<img src={useBaseUrl("img/wallet-bridge/wallet-faq-4.png")} width="357" height="600" />


## ¿Puedo enviar mis tokens desde Polygon a cualquier otra billetera / intercambio? {#can-i-send-my-tokens-from-polygon-to-any-other-wallet-exchange}

No puedes enviar tokens directamente desde la interfaz de Polygon a las billeteras. Tienes primero que retirar desde Polygon a Ethereum y entonces enviar a la dirección de cambio (a menos que tu billetera sea explícitamente compatible con la red de la cadena).

## Cometí un error al enviar fondos a una billetera/intercambio directamente. ¿Me puedes ayudar? {#i-made-a-mistake-of-sending-funds-to-an-exchange-wallet-directly-can-you-help}

Desafortunadamente, no podemos asistir en tales casos. No enviar fondos directamente a los intercambios que soporta solo Ethereum, primero tienes que retirar desde Polygon a Ethereum y entonces enviar a tu dirección de intercambio.

## Mi transacción está pendiente por mucho tiempo, ¿qué puedo hacer? {#my-transaction-is-pending-for-too-long-what-can-i-do}

Las transacciones en la cadena de bloques pueden ser abandonadas debido a un precio de gas bajo se establece al enviar la transacción También pueden ser abandonadas cuando hay una subida repentina en el precio del gas debido a la congestión en Etherum. Otra posibilidad es que puedes haber cancelado la transacción desde tu billetera o haber reemplazado la transacción. En todos estos casos, la billetera web te mostrará la transacción en un mensaje de progreso y esto te hará esperar más tiempo.

Si tu transacción está atrapada por más de una hora, mostrará un botón "Intentar otra vez". Esto es bueno, significa que puedes pedir red para volver a intentar la transacción para ti. Lo que puedes hacer a continuación es darle clic en el botón de "Intentar otra vez" para volver a intentar la misma transacción. Si tu transacción de depósito se encuentra atascada, tu proceso de depositar será reiniciado y si tu retiro se encontraba atascado, podrás continuar con tu retiro desde donde completaste con éxito el paso anterior.

En caso de enfrentar problemas en seguir adelante con el botón de "Intentar otra vez" y estás utilizando la billetera MetaMask puedes tener que revisar si hay muchas transacciones en cola que obstruyen la sección de actividad de tu MetaMask En este caso, puede ser útil volver a instalar la billetera MetaMask y continuar con tu transacción Alternativamente, puedes intentar iniciar la transacción desde un navegador separado.

Ver el video abajo puede dar más claridad sobre cómo utilizar la función (o característica) "Trata de nuevo".

[https://youtu.be/0b4yjR_naEQ](https://youtu.be/0b4yjR_naEQ)

## ¿Cuál es la lista de intercambios admitidos en Polygon? {#what-are-the-list-of-supported-exchanges-on-polygon}

Abajo hay una lista de intercambios centralizados que soporta actualmente Polygon y también los tokens que estos intercambios soportan

AscendEX - USDC, EASY MATIC

MXC MATIC - MATIC, PlotX, Dfyn

Okcoin - ETH, USDT, LINK, MKR, USDK, DAI, USDK, COMP, YFI, SNX, YFII, UNI. (Los tokens solo pueden ser movidos de Okcoin a la cadena de Polygon). (La transferencia de tokens desde Polygon a Okcoin no es compatible actualmente)

Okex - BAL, BAT, CEL, COMP, CRV, DAI, ETH, GHST, GUSD, LINK, MKR, PAX, SNX, SUSHI, TUSD, UNI, USDC-ERC20, USDT-ERC20, USDK, wBTC, YFI, YFII, ZRX Los tokens solo pueden ser movidos de Okex a la cadena de Polygon. La transferencia de tokens desde Polygon a Okex no es compatible actualmente.

Bitforex MATIC

Enviar tokens a cualquier otro intercambio que no esté mencionado explícitamente en la lista anterior puede conducir a una pérdida de fondos. Si quieres retirar fondos a cualquier intercambio que no soporte Polygon, tendrás primero que retirar el token a Ethereum y entonces enviarlo al intercambio usando tu billetera Ethereum. Este video demuestra como retirar fondos desde Polygon a Ethereum - [https://www.youtube.com/watch?v=DgpHY95qrbQ&list=PLslsfan1R_z0Epvnqsj29V1LBAh99dzu9&index=5](https://www.youtube.com/watch?v=DgpHY95qrbQ&list=PLslsfan1R_z0Epvnqsj29V1LBAh99dzu9&index=5)

Alternativamente, puedes seguir esta guía [aquí](https://docs.matic.today/docs/develop/wallets/matic-web-wallet/web-wallet-v2-guide/).

## No puedo iniciar sesión, ¿qué hago? {#i-am-not-able-to-login-what-do-i-do}

[https://docs.polygon.technology/docs/validate/delegator-faq/#my-metamask-is-stuck-at-confirming-after-login-what-do-i-do-or-nothing-happens-when-i-try-to-login](https://docs.polygon.technology/docs/validate/delegator-faq/#my-metamask-is-stuck-at-confirming-after-login-what-do-i-do-or-nothing-happens-when-i-try-to-login)

## ¿Es soportada por Polygon la billetera de hardware? {#does-polygon-support-hardware-wallets}
Sí, las billeteras de hardware. son soportadas

## ¿Qué puedo hacer con mi billetera de Polygon? {#what-can-i-do-with-my-polygon-wallet}

- Enviar fondos a cualquier cuenta en Polygon.
- Depositar fondos desde Ethereum a Polygon (usando el puente).
- Retirar fondos de regreso de Ethereum desde Polygon (también usando puente).

## Mi token no es visible en la lista. ¿A quién debo contactar?  {#my-token-is-not-visible-in-the-list-who-should-i-contact}

Contactar al equipo de Polygon en Discord o Telegram y conseguir que tu token este listado. Antes de eso, asegúrate que tu token está mapeado. Si no está mapeado levanta una solicitud [https://mapper.polygon.technology/](https://mapper.polygon.technology/)

## ¿Cuáles son algunas de las mejores prácticas a seguir? {#what-are-some-best-practices-to-follow}

- Cuando quieras enviar fondos desde Polygon a Ethereum, utiliza la funcionalidad de retirar. No utilices la funcionalidad de enviar. Esto conducirá a la pérdida de fondos.
- No deposites en la red principal de Polygon si deseas participar solo en apilamiento.
- No cambiar el límite de gas desde MetaMask.

## ¿Qué hago si el depósito está confirmado pero el saldo no está actualizado?  {#what-do-i-do-if-the-deposit-is-confirmed-but-the-balance-is-not-getting-updated}

Se tarda entre 7 y 8 minutos para depositar la transacción en completar. Espere por un tiempo y de clic en "refrescar saldo"

## ¿Qué debo hacer si el punto de verificación no está sucediendo? {#what-should-i-do-if-the-checkpoint-is-not-happening}

Los puntos de verificación algunas veces toman de 45 minutos a 1 hora basados en la congestión en Ethereum, te sugerimos esperar un momento antes de subir un ticket.

## ¿Es posible cancelar una transacción de retiro? {#is-it-possible-to-cancel-a-withdraw-transaction}

No, tienes que completar los siguientes pasos. Si el precio actual de gas es demasiado alto, entonces espere y pruebe más adelante cuando el precio de gas baje.

## ¿Por qué el token MATIC no es compatible con PoS? (prueba de participación) {#why-is-the-matic-token-is-not-supported-on-pos}

MATIC es el token nativo de Polygon y tiene una dirección de contrato 0x0000000000000000000000000000000000001010 en la cadena de Polygon. También se utiliza para pagar gas. Mapear el token MATIC en el puente PoS dará lugar a que MATIC tenga una dirección de contrato adicional en la cadena de Polygon. Esto colisionará con la existente dirección del contrato, ya que esta nueva dirección de token no puede utilizarse para pagar gas y tendrá que permanecer como un token ERC-20 normal en la cadena de Polygon. Por lo tanto, para evitar esta confusión, se decidió conservar MATIC solo en plasma

## ¿Cómo mapeo los tokens? {#how-do-i-map-tokens}

Por favor, envíe una solicitud de mapeo a [https://mapper.polygon.technology/](https://mapper.polygon.technology/)

## ¿Qué hago si la transacción está demorando demasiado o si el precio del gas es demasiado alto?  {#what-do-i-do-if-the-transaction-is-taking-too-long-or-if-the-gas-price-is-too-high}

El tiempo de una transacción y el precio de gas varían según la red se congestione. Si se paga un alto, precio del gas entonces la transacción se confirma más rápido.

## ¿Puedo cambiar el límite del gas o el precio del gas? {#can-i-change-the-gas-limit-or-the-gas-price}

El límite del gas se estima y establece por la aplicación de acuerdo con ciertos requisitos de la función que se llama en contrato. Esto no debe ser editado. El precio de gas solo puede ser cambiado para aumentar o disminuir los gastos de la transacción.

## ¿Qué debo hacer si la transacción fue cancelada pero la billetera web muestra que la transacción está completa? {#what-should-i-do-if-the-transaction-was-cancelled-but-the-web-wallet-shows-transaction-is-completed}

Contacta a nuestro equipo de soporte.

## ¿Dónde elevo un ticket de soporte? {#where-do-i-raise-a-support-ticket}
https://support.polygon.technology/support/home

## El precio del gas es mayor que la cantidad que busco retirar.  {#the-gas-price-is-more-than-the-amount-i-seek-to-withdraw}

Una operación de retiro con el puente de plasma se divide en 3 pasos, uno que ocurre en la red principal de Polygon y dos pasos que se completarán en la red principal de Ethereum. En el puente del puente de PoS (prueba de participación) la transacción de retiro ocurre en dos pasos: la quema de token en la red de Polygon y la prueba de presentación en la red de Ethereum. En la red principal de Polygon los cargos son mínimos, y la participación de Lion del costo de la transacción que ves es del precio del gas en la red de Ethereum gobernada por mineros de Ethereum. Como es de esperarse, este cargo está fuera de nuestro control, y no tenemos mucha influencia sobre el punto de precio. Una última cosa, si tus tokens están quemados, puedes tener proceder con tu retiro independientemente de que no hay nada que podamos hacer para invertir el proceso.


## ¿Puedo cancelar mi transacción de retiro? {#can-i-cancel-my-withdrawal-transaction}

Desafortunadamente, Polygon no puede cancelar un retiro una vez que el proceso es inicializado y los tokens se queman correctamente. Se crea un hash de quemado y la próxima fase de la transacción viene inmediatamente. Si la transacción de quemado sigue pendiente, puedes ser capaz de facilitar una cancelación mediante las siguientes guías

[Metamask](https://metamask.zendesk.com/hc/en-us/articles/360015489251-How-to-Speed-Up-or-Cancel-a-Pending-Transaction) <br />
 [Walletlink](https://www.techdreams.org/crypto-currency/how-to-cancel-a-pending-ethereum-transaction-on-coinbase-wallet/10159-20210412)


## Mi transacción está atascada.  {#my-transaction-is-stuck}

Hemos enumerado algunos errores comunes que los usuarios pueden enfrentar. Puedes encontrar la solución abajo de la imagen del error. En caso de que te muestren un error diferente [eleva un ticket de soporte](https://support.polygon.technology/support/home) de nuestro equipo para solucionar problemas.

  - ### Errores comunes {#common-errors}
a. retiro atascado en la fase inicializada.

    <img src={useBaseUrl("img/wallet-bridge/plasma-progress-stuck.png")} width="357" height="800"/>

    Esto ocurre normalmente cuando la transacción se remplaza y la aplicación de la billetera web no es capaz de detectar el hash de la transacción remplazada. Seguir las instrucciones de [https://withdraw.polygon.technology/](https://withdraw.polygon.technology/) y completar tu retiro
b. Error de RPC

    <img src={useBaseUrl("img/wallet-bridge/checkpoint-rpc-error.png")} width="357" height="600"/>

    El error actual de RPC que enfrentas puede ser debido a una sobrecarga de RPC.

     Intenta cambiar tu RPC y proceder con la transacción. Puedes seguir este enlace [here](https://docs.polygon.technology/docs/develop/network-details/network#matic-mainnet) para más información.
c.

  <img src={useBaseUrl("img/wallet-bridge/checkpoint-stumbled-error.png")} width="357" height="600"/>

Este es generalmente un error de apagado y encendido que se resuelve automáticamente. En caso de que siga recibiendo el mismo error al reiniciar el paso, haga [la elevación de un ticket de soporte](https://support.polygon.technology/) con toda la información relevante para solucionar este problema aún más.

## Cometí el error de enviar fondos a una billetera de intercambio directamente desde la billetera de Polygon. ¿Me puedes ayudar? {#i-made-the-mistake-of-sending-funds-to-an-exchange-wallet-directly-from-polygon-wallet-can-you-help}

Tristemente lamentamos informarle de que es posible que no podamos ayudarte si has enviado tokens de la red de Polygon a una billetera de intercambio lo que no es compatible.

Esto es lo que necesita en este caso hacer un intercambio (aunque no estamos seguros de cuanta flexibilidad tienen los ejecutivos de soporte para ejecutar esto). Suponiendo que el ejecutivo de soporte de intercambio tiene acceso a las claves privadas pueden transferir los fondos desde su cuenta en Polygon a tu dirección (de usuario) en Polygon.

Es importante notar que no debes enviar fondos directamente a intercambios que solo soporte Ethereum. El procedimiento correcto es que primero tienes que retirar desde Polygon a Ethereum y entonces enviarlo a tu dirección de intercambio.

## Me muestran un error de saldo insuficiente. {#i-m-shown-an-insufficient-balance-error}

Los retiros y los depósitos en la red de Polygon son baratos. Lo que debe entenderse es que el error de saldo insuficiente puede ser aclarado obteniendo saldo ETH en la red principal de Ethereum. Eso generalmente borra el problema de saldo insuficiente.

Si esta es una transacción en la red principal de Polygon te pediremos que tengas suficiente cantidad de tokens MATIC.

## ¿Cómo puenteo los activos a través de las cadenas? {#how-do-i-bridge-assets-across-chains}

[https://wallet.polygon.technology/bridge/](https://wallet.polygon.technology/bridge/) (ETH <-> Polygon) <br/>
 [https://xpollinate.io/](https://xpollinate.io/) (BSC <-> Polygon <-> xDai) <br/>
 [https://exchange.chainswap.com/](https://exchange.chainswap.com/) (ETH <-> Polygon/BSC) <br/>
 [https://anyswap.exchange/bridge](https://anyswap.exchange/bridge) (ETH <-> Polygon <-> BSC/xDai) <br/>
 [https://app.0.exchange/#/home](https://app.0.exchange/#/home)(ETH <-> Polygon <-> Avalanche <-> BSC

Agregar que no respaldamos ningún servicio externo asegúrate de hacer siempre tu propia investigación.

## Hice una transferencia a la dirección equivocada. ¿Cómo recupero los fondos? {#i-made-a-transfer-to-the-wrong-address-how-do-i-retrieve-the-funds}

Desafortunadamente, nada puede hacerse. Solo el propietario de las claves privadas a esa dirección en particular puede mover esos activos.


## Mis transacciones no son visibles en el explorador (o Explorer). ¿Qué debo hacer? {#my-transactions-are-not-visible-on-the-explorer-what-should-i-do}

Este es probablemente un problema de indexación con Polygonscan. Contacta el [Equipo de Soporte](https://support.polygon.technology/support/home) para más clarificaciones.
 También puedes probar este bloque de exploradores

[https://polygon-explorer-mainnet.chainstacklabs.com](https://polygon-explorer-mainnet.chainstacklabs.com/) <br />
[https://explorer-mainnet.maticvigil.com](https://explorer-mainnet.maticvigil.com/) <br />
[https://explorer.matic.network](https://explorer.matic.network/) <br />
[https://backup-explorer.matic.network](https://backup-explorer.matic.network/)


## Inicié un depósito en Ethereum, pero todavía se muestra como pendiente. ¿Qué debo hacer? {#i-initiated-a-deposit-on-ethereum-but-it-still-shows-as-pending-what-should-i-do}

Tu gas suministrado es probablemente demasiado bajo. Debes esperar un tiempo y rehacer la transacción si no se acuña. En caso de ayuda adicional, contacta al [equipo de soporte](https://support.polygon.technology/support/home) con tu dirección de billetera, hashes de transacción (si existe alguno) y capturas de pantalla relevantes.


## Tengo un problema de retiro de token con OpenSea o cualquier otra aplicación que use el puente de Polygon.  {#i-have-a-token-withdrawal-issue-with-opensea-or-any-other-application-which-uses-polygon-bridge}

Si tienes un problema con tu transacción estancada, de retiro, Polygon te ofrece el retiro puente con https://polygon-withdraw.matic.network/ para ayudarte a sacarte del problema si tienes tu hash quemado. Con esta herramienta, estás rápidamente incorporado y el problema será resuelto. Otras preguntas relacionadas con tu transacción con OpenSea y otras dApps tendrán que ser manejadas por el equipo de las aplicaciones.


## ¿Dónde puedo obtener tokens MATIC directamente? {#where-can-i-get-matic-tokens-directly}

Así que los tokens MATIC tokens pueden comprarse en cualquier centralizada de ([Binance](https://www.binance.com/en), [Coinbase](https://www.coinbase.com/), et.al) o descentralizada ([Uniswap](https://uniswap.org/), [QuickSwap](https://quickswap.exchange/#/swap)) de intercambio. También puedes investigar y tratar con algunas on-ramps como [Transak](https://transak.com/), [Ramp](https://ramp.network/).
 El propósito para tu compra de monedas MATIC también debe determinar dónde las comprarás y de que red. Es aconsejable tener MATIC en la red principal de Ethereum si tu intención es de apilamiento o delegación. Si tu intención es una transacción en la red principal de Polygon debes mantener y transaccionar con MATIC en la red principal de Polygon.


## ¿No estoy recibiendo una transacción hash y mis depósitos no están pasando? ¿Qué está pasando? {#i-m-not-getting-a-transaction-hash-and-my-deposits-aren-t-going-through-what-is-happening}

Probablemente tienes transacciones pendientes previas, por favor cancele o primero acelérelas. Las transacciones en Ethereum solo pueden pasar una tras otra.


## Muestra que Polygon no cobra cantidad alguna por un retiro pero que debemos pagar durante la transacción.  {#it-shows-polygon-does-not-charge-any-amount-for-a-withdrawal-but-we-are-to-pay-during-the-transaction}

Una operación de retiro con el puente de plasma se divide en 3 pasos, uno que ocurre en la red principal de Polygon y dos pasos que se completarán en la red principal de Ethereum. En el puente del puente de PoS (prueba de participación) la transacción de retiro ocurre en dos pasos: la quema de token en la red de Polygon y la prueba de presentación en la red de Ethereum. En cada caso, la quema de token que ocurre en red principal de Polygon será con un costo mínimo. Los pasos restantes que sucedan en la red principal de Ethereum deberán pagarse en ETH dependiendo del precio actual de gas lo que se puede verificar [aquí](https://ethgasstation.info/).


## ¿Cómo contacto con las principales aplicaciones desplegadas en la red de Polygon? {#how-do-i-contact-major-applications-deployed-on-the-polygon-network}

Curve [https://discord.gg/JnUFrsDF](https://discord.gg/JnUFrsDF) <br />
SushiSwap [https://discord.gg/ApbE4Eau](https://discord.gg/ApbE4Eau) <br />
CREAM [https://discord.gg/js8JpmFB](https://discord.gg/js8JpmFB) <br />
AAVE [https://discord.gg/YYtp7N5d](https://discord.gg/YYtp7N5d) <br />
FuruCombo [https://discord.gg/wJJ7PXAd](https://discord.gg/wJJ7PXAd) <br />
QuickSwap [http://t.me/QuickSwapDEX](http://t.me/QuickSwapDEX) <br />

Beefy Finance - [https://discord.gg/egkEEAkC](https://discord.gg/egkEEAkC)


## Lista de billeteras compatibles de hardware en la red de Polygon.  {#list-of-hardware-wallets-supported-on-polygon-network}

Así la red de Polygon soportará todas las billeteras hardware compatibles con MetaMask. Siga este [enlace](https://metamask.zendesk.com/hc/en-us/articles/360020394612-How-to-connect-a-Trezor-or-Ledger-Hardware-Wallet) desde Metamask para más información.


## He sido estafado. ¿Cómo recuperaré mis tokens? {#i-have-been-scammed-how-will-i-retrieve-my-tokens}

Desafortunadamente, no hay un proceso de recuperación de las monedas perdidas. Pedimos que antes de hacer una transacción hagas una verificación y cheques doble antes de comenzar y completar. nota que la red de Polygon y nuestros manejos oficiales no participan en ninguna publicación de regalos o de duplicación de tokens y nunca te acercaremos en nombre de la organización. Ignore todos los intentos, ya que lo más probable es que sean estafas. Todas nuestras comunicaciones son a través de nuestro oficial manejos.


## Así que Ethereum tiene Goerli como su prueba de red. ¿Tiene la red de Polygon una prueba de red?  {#so-ethereum-has-goerli-as-its-test-network-does-polygon-network-have-a-test-network}

Así que cómo la red de Ethereum tiene Goerli como una prueba de red, la red principal de Polygon tiene Mumbai. Todas las transacciones en esta prueba de red serán indexadas en el Explorador de Mumbai.


## ¿Cómo puedo acelerar mi transacción en MetaMask?  {#how-can-speed-up-my-transaction-on-metamask}

Para acelerar las transacciones mediante MetaMask entra en este [enlace](https://metamask.zendesk.com/hc/en-us/articles/360015489251-How-to-Speed-Up-or-Cancel-a-Pending-Transaction)


## ¿Qué información debo proporcionar cuando cree un ticket? {#what-all-information-should-i-provide-when-i-create-a-ticket}

- billetera dirección
- hash transacción
- Acción exacta intentada y el resultado, muy descriptivo
- Capturas de pantalla o grabaciones de la pantalla de la acción

## Intentaba hacer un depósito, pero la transacción se detuvo en el paso de Aprobación.  {#i-was-trying-to-make-a-deposit-but-the-transaction-stopped-at-the-approve-step}

Si la transacción sigue en la etapa de **Aprobación** no está aún completada. Para cumplirlo, tienes que pagar la comisión de gas entonces debe pasar.

## la comisión de mi transacción de retiro es demasiado alta.  {#the-gas-fee-for-my-withdrawal-transaction-is-too-high}

Las tarifas de gas en la red de Polygon son siempre muy bajas, pero no podemos decir lo mismo para la red principal de Ethereum. Si has comenzado una transacción es importante no cancelarla. En cambio, puedes esperar por las tarifas de gas para bajar o agregar ETH a tu cuenta.

## Hay algunas transacciones no autorizadas en mi billetera. ¿Está mi billetera hackeada? {#there-are-some-unauthorized-transactions-in-my-wallet-is-my-wallet-hacked}

Desafortunadamente, la red no puede revertir las transacciones no deseadas. Siempre es importante tener cuidado con tus claves privadas y **nunca compartirlas con nadie**.
 Si todavía tienes algunos fondos restantes, transfiérelos inmediatamente a una nueva billetera.

## La billetera de Polygon muestra un mensaje de error de ‘Oops nuestro servidor Tropezó’ {#polygon-wallet-shows-an-oops-our-server-stumbled-error-message}

Ese mensaje puede significar que nuestro servidor está desactivado. Sin embargo, si todo está funcionando bien, te sugerimos que uses otro navegador.  Si estás intentando hacer un retiro también puedes probar el [retiro en la herramienta Polygon](https://polygon-withdraw.matic.network/). Allí, tú puedes conectar tu billetera, pegar tu transacción hash y proceder con la transacción.

## La billetera de Polygon muestra Mensaje de error "Firma de transacción denegada por el usuario".  {#polygon-wallet-shows-user-denied-transaction-signature-error-message}

Esto ocurre generalmente porque el usuario canceló o se negó a firmar una transacción a través de MetaMask. Cuando se le solicite la billetera MetaMask, proceda a firmar la transacción haciendo clic en Aprobar y no en Cancelar.

## No recibí los tokens que transfirieron a un intercambio  {#i-did-not-receive-the-tokens-i-transferred-to-an-exchange}
Has transferido las monedas a Binance (Coinbase, Kucoin cualquier u otro intercambio) pero no las has recibido en la lateral de intercambio. Si ese fue tu caso, es importante saber que actualmente no proporcionamos una conexión directa con los intercambios. La mayoría de las transacciones realmente pasarían por la red principal de Ethereum antes de llegar al intercambio. Contacta al equipo de soporte de intercambio.

## Mi billetera MetaMask no está conectada con la billetera de Polygon {#my-metamask-wallet-is-not-connecting-with-polygon-wallet}

Hay muchas razones por las que esto puede estar sucediendo. Te sugerimos **que intentes en otro momento**, **uses otro navegador** o, si nada de esto te ayuda, **contacta a nuestro equipo de soporte**.

## ¿Cómo puedo obtener tokens MATIC para pagar tarifas de gas? {#how-can-i-get-matic-tokens-to-pay-for-gas-fees}

Te proporcionamos un [Intercambio de Gas](https://wallet.polygon.technology/gas-swap/) este servicio que te ayudara con eso. Tú eliges una cantidad de MATIC que necesitas para completar tu transacción y puedes intercambiar por otros tokens como Ether o USDT. Vale la pena señalar que esta es una **transacción sin gas**.

## Intercambiar tokens es demasiado lento. {#token-swap-is-too-slow}

Si estás intentando intercambiar tokens y está tomando demasiado tiempo, puedes intentar la misma transacción en un navegador diferente. Si eso no funciona y te enfrentas a un error envía una captura de pantalla a nuestro equipo de soporte
