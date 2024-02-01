# Smart Contracts

Tras haber explorado qué son los NFTs y cómo pueden enriquecer tus productos digitales, es hora de adentrarnos en el corazón de estos activos únicos: los Smart Contracts (Contratos Inteligentes). Estos no son solo el motor que impulsa los NFTs, sino que definen su verdadera naturaleza y posibilidades.

## Smart Contracts: La Máquina Expendedora de la Blockchain

Imagina que estás frente a una máquina expendedora. Introduces tu dinero, seleccionas el producto y, automáticamente, la máquina valida tu selección, procesa tu pago y entrega el artículo. No hay interacción humana, todo se realiza según un conjunto predefinido de reglas programadas en la máquina.

Los Smart Contracts funcionan de manera similar en el mundo de los NFTs y la blockchain. Son contratos autoejecutables con los términos del acuerdo entre comprador y vendedor escritos directamente en líneas de código. Estos contratos viven y operan en la blockchain, que es una red descentralizada y segura que actúa como un libro mayor inmutable.

<figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

### Elementos de un Smart Contract

#### Estándares: ERC-721 y Más

Para los NFTs, el estándar más común es el ERC-721, que permite la creación de tokens únicos. Este estándar es crucial porque define las normas que todos los Smart Contracts ERC-721 deben seguir para funcionar correctamente dentro del ecosistema Ethereum.

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption><p>El Contrato inteligente define las funcionalidades que se pueden realizar con un token específico. </p></figcaption></figure>

#### Funciones Esenciales

* **Función de Acuñación (Mint Function)**: Es como seleccionar tu bebida en la máquina expendedora. Esta función permite crear un nuevo NFT, único y rastreable.
* **Función de Transferencia (Transfer Function)**: Al igual que la máquina dispensa el producto, esta función permite al dueño del NFT enviarlo a otro usuario.
* **Funciones de Aprobación (Approve Function)**: Decides quién puede manejar o transferir tu NFT, proporcionando una capa extra de seguridad y control. Esta función permite que el propietario actual de un NFT autorice a otra dirección (un usuario o un contrato inteligente) para transferir el token específico en su nombre. así funcionan los marketplaces como Opensea.&#x20;
* **Funciones de Propiedad (Ownership Functions)**: Estas funciones establecen y verifican quién es el dueño actual del NFT.

#### Datos y Metadatos

* **URL de Metadatos (Metadata URL)**: Cada NFT tiene información asociada, como el arte digital, características o términos de uso, almacenada a menudo fuera de la cadena y accesible a través de una URL.
* **Funciones de Saldo (Balance Functions)**: Estas funciones permiten consultar cuántos tokens posee una dirección específica.
* **Controles de Acceso (Access Controls)** y **Eventos (Events)**: Permiten gestionar permisos y registrar actividades significativas que ocurren con el NFT, como ventas o transferencias.



### El Smart Contract en Acción

Al igual que una máquina expendedora, el Smart Contract es implacablemente lógico. Si se cumplen las condiciones establecidas, ejecutará la acción correspondiente. No hay lugar para errores o malinterpretaciones; todo es transparente y automático.



En resumen, los Smart Contracts son el motor que da vida a los NFTs, proporcionando la infraestructura necesaria para que estos activos digitales funcionen de manera autónoma y segura. Con cada función y atributo cuidadosamente codificado, estos contratos inteligentes nos permiten imaginar y construir una economía digital más libre y justa. Sin embargo, para que un NFT o cualquier token tenga un impacto real, debe ser parte de un ecosistema tecnológico más amplio.&#x20;

En sección de [Arquitectura](../arquitectura-de-un-producto-web3-que-utiliza-tokens.md), exploraremos[^1] la arquitectura general de un producto Web3 que utiliza tokens, detallando cómo cada componente juega un papel esencial en la creación de una experiencia digital descentralizada. Pero antes exploremos un poco más en las funciones básicas de un contrato 721.&#x20;

[^1]: test
