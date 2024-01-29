# ERC-5007: Extensión de Tiempo en ERC-721

El ERC-5007 es una propuesta de mejora para Ethereum que introduce una extensión al estándar ERC-721 para agregar gestión de tiempo en cadena a los tokens no fungibles (NFTs). Esta extensión permite asignar un período de tiempo durante el cual un NFT es válido o utilizable.

### ERC-5007: Extensión de Tiempo en ERC-721

**Concepto Básico**

* **Objetivo**: Extender los NFTs estándar ERC-721 con funciones adicionales para manejar el tiempo, específicamente las fechas de inicio y fin de validez del NFT.
* **Aplicación**: Ideal para NFTs que tienen un período de uso definido, como entradas para eventos, suscripciones, o licencias temporales.

**Funcionalidad y Especificación**

* **Funciones de Tiempo**: Incluye `startTime` y `endTime`, que devuelven el inicio y el fin del período de validez del NFT como una marca de tiempo UNIX.
* **Compatibilidad con Composición**: Opcionalmente, los NFTs pueden ser compuestos a partir de NFTs existentes o combinar dos NFTs en uno.

**Motivación**

* **Manejo Eficiente del Tiempo**: Resolver el problema de los NFTs que requieren activación o desactivación en momentos específicos sin necesidad de transacciones adicionales.
* **Consistencia en la Interfaz**: Unificar las interfaces para NFTs con funciones de tiempo, facilitando el desarrollo de plataformas de terceros.

**Datos de Tiempo**

* **Tipo de Dato**: Se utiliza `uint64` para las marcas de tiempo, que es suficientemente amplio para abarcar fechas futuras y es compatible con la mayoría de los lenguajes de programación.

**Compatibilidad con Versiones Anteriores**

* Totalmente compatible con ERC-721, lo que permite el uso de herramientas y estructuras existentes.

**Implementación de Referencia y Casos de Prueba**

* Se proporcionan detalles de implementación y casos de prueba para verificar la funcionalidad del manejo del tiempo y la composición de NFTs.



Al implementar ERC-5007, los creadores de NFT pueden diseñar tokens que tienen una relevancia temporal, como boletos para eventos o licencias que solo son válidas durante un período específico. Esto abre nuevas posibilidades para el uso de NFTs en diversas aplicaciones donde el tiempo es un factor crítico.
