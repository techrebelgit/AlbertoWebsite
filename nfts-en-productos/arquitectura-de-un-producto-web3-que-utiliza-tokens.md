# Arquitectura de un Producto Web3 que Utiliza Tokens

La creación de un producto Web3 es un ejercicio de precisión arquitectónica, donde cada componente tiene un papel definido que contribuye a la autonomía y eficiencia del sistema.

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

### Frontend (FE): La Cara del Producto Web3

El Frontend de un producto Web3 es la interfaz con la que el usuario interactúa. Dado que la interacción con la blockchain es inherente a los productos Web3, el FE no solo debe ser estéticamente agradable sino también funcionalmente robusto. Debe ser capaz de interactuar con billeteras digitales y signers para transacciones y gestionar de manera efectiva la comunicación con los smart contracts.

### Backend (BE): El Cerebro Opcional

El BE en el contexto Web3 puede no ser necesario para aplicaciones que simplemente leen y escriben en la blockchain, utilizando el signer del usuario para interactuar directamente con la red. Sin embargo, para aplicaciones con lógica más compleja o que requieren un signer interno, como las soluciones custodial, se vuelve esencial. En estos casos, el BE interactúa con un sistema de gestión de claves (KMS) para firmar transacciones de manera segura y gestionar los procesos internos.

### Signers: Los Autorizadores de Transacciones

Los signers son entidades o mecanismos que firman las transacciones en la blockchain. Pueden ser externos, como en aplicaciones no custodiales donde los usuarios tienen el control total de sus claves privadas, o internos, en productos custodiales o aquellos que generan transacciones automáticamente.

### Providers: Los Conectores de la Blockchain

Los providers son servicios esenciales que permiten a las aplicaciones Web3 interactuar con la red blockchain. Ejemplos de providers incluyen WalletConnect, librerías como web3.js, extensiones de navegador como MetaMask y servicios de nodo como Infura y Alchemy. Actúan como intermediarios entre el FE, los smart contracts y la blockchain, facilitando la comunicación necesaria para las operaciones.

### Storage: El Almacenamiento de Datos

El almacenamiento en aplicaciones Web3 puede ser on-chain, directamente en la blockchain, o off-chain, en otras estructuras de datos. Soluciones como IPFS (InterPlanetary File System) y Arweave permiten almacenar datos de manera descentralizada y son fundamentales para manejar información que no es práctico o rentable almacenar en la blockchain, como grandes archivos multimedia.

### Oracles

Los oracles son puentes que proporcionan datos del mundo real a la blockchain, lo que permite que los Smart Contracts respondan a eventos externos.

### Red Blockchain: Testnet y Mainnet

Antes de lanzar un producto al mercado, se prueba en una red de prueba o testnet, que simula la blockchain principal (mainnet) sin el riesgo de manejar activos reales.



### Smart Contracts: La Base de la Interacción

Estos no son meros trozos de código; son los constructores de reglas y ejecutores de lógica que manejan tanto tokens fungibles como NFTs dentro de la red blockchain. Los usuarios y aplicaciones interactúan con estos contratos inteligentes para realizar todas las operaciones, desde transferencias hasta la ejecución de funciones complejas.



