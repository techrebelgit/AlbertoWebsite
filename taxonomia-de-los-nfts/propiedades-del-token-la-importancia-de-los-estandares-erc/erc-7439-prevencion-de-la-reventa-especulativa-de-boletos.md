# ERC-7439: Prevención de la Reventa Especulativa de Boletos

El ERC-7439 es una propuesta de mejora para Ethereum que extiende el estándar ERC-721, definiendo funciones estándar para la reventa de boletos a través de revendedores autorizados. Este estándar tiene como objetivo abordar el problema de la reventa especulativa de boletos, comúnmente conocida como "scalping", y proteger a los consumidores de ser explotados en el mercado secundario de boletos.



### ERC-7439: Prevención de la Reventa Especulativa de Boletos

**Concepto Básico**

* **Objetivo**: Implementar un marco que permita a los agentes de venta de boletos o a los organizadores de eventos tomar acciones preventivas contra la reventa especulativa de boletos.
* **Aplicación**: Habilitar a los clientes para revender sus boletos a través de revendedores autorizados, manteniendo un control sobre la transferencia y el estado de los boletos.

**Funcionalidad y Especificación**

* **TokenInfo y TokenStatus**: Estructuras que definen el estado y la información adicional de los boletos, como el estado de venta, reventa, anulación o canje.
* **Restricción de Transferencias**: Prohibir las transferencias de boletos, excepto por cuentas específicas autorizadas (como agentes de boletos, gerentes, promotores o plataformas de reventa autorizadas).
* **Control de Revendedores Autorizados**: Solo cuentas específicas con un rol asignado pueden cambiar el estado del boleto o realizar transferencias.

**Motivación**

* **Problema de Reventa Especulativa**: Abordar los problemas asociados con la reventa especulativa de boletos, incluido el fraude y la explotación de los consumidores.
* **Transparencia en la Venta de Boletos**: Establecer un canal de ventas primarias abierto y transparente y un mecanismo de reventa secundaria justo.

**Implementación de Referencia y Casos de Prueba**

* La implementación de referencia se basa en contratos inteligentes de Solidity que extienden el estándar ERC-721.
* Se incluyen casos de prueba para verificar la funcionalidad de la transferencia y el cambio de estado de los boletos.

**Racionalidad**

* **Establecer un Ecosistema de Venta de Boletos Saludable**: Crear reglas claras y un sistema de precios abierto para equilibrar la oferta y la demanda, y proteger a los consumidores.
* **Proceso de Venta de Boletos Fluida**: Facilitar la compra, reembolso y canje de boletos, asegurando una experiencia sin problemas para los consumidores.

**Compatibilidad con Versiones Anteriores**

* Compatible con ERC-721 para aprovechar las herramientas y la infraestructura existentes.

Al implementar el estándar ERC-7439, los organizadores de eventos y los agentes de venta de boletos pueden ofrecer una forma más segura y justa de manejar la venta y reventa de boletos, protegiendo a los consumidores y mejorando la experiencia general de compra de boletos.
