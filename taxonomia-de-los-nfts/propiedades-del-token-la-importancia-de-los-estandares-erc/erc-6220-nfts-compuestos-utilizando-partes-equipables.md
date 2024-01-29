# ERC-6220: NFTs Compuestos Utilizando Partes Equipables

El ERC-6220 es una propuesta de mejora para Ethereum que introduce un nuevo concepto en el mundo de los tokens no fungibles (NFTs): los NFTs compuestos utilizando partes equipables. Esta propuesta extiende el estándar ERC-721 permitiendo que los NFTs añadan selectivamente partes a sí mismos a través de un proceso de equipamiento.

### ERC-6220: NFTs Compuestos Utilizando Partes Equipables

**Concepto Básico**

* **Objetivo**: Permitir la composición de NFTs a través de la adición de partes fijas y partes de ranura (slots).
* **Aplicación**: Los NFTs pueden ser compuestos seleccionando partes de un Catálogo para cada instancia de NFT y equipar otros NFTs en ranuras, que también están definidas en el Catálogo.

**Tipos de Partes**

* **Partes Fijas**: Componentes completos con sus propios metadatos que no cambian durante la vida del NFT.
* **Partes de Ranura**: Permiten equipar colecciones de NFTs en ellas.

**Funcionalidad**

* **Equipamiento de Partes**: Al equipar una parte en un NFT, se agrega un componente adicional que se renderiza al recuperar el token.
* **Composición de NFTs**: Permite una personalización prácticamente ilimitada del NFT base.

**Motivación**

* **Progreso del Token**: A medida que un NFT progresa, puede obtener o ser premiado con diversas partes.
* **Seguimiento de Méritos**: Utilizar NFTs equipables para rastrear logros o méritos.
* **Escasez Digital Comprobable**: Asegura que, si una parte está equipada en un avatar, no pueda ser equipada en otro al mismo tiempo.

**Especificación**

* **Tokens Equipables**: Se define una interfaz para el contrato inteligente central de los tokens equipables.
* **Catálogo**: Colección de partes equipables fijas y de ranura que pueden apoyar cualquier número de colecciones de NFTs.

**Razón de Ser**

* **Uso de Catálogo**: Permite la verificación previa de las partes para asegurar que el compuesto resultante funcione como se espera.
* **Dos Tipos de Partes**: Para soportar numerosos casos de uso y configuraciones.

**Compatibilidad con Versiones Anteriores**

* Compatible con ERC-721 para aprovechar las herramientas robustas disponibles y asegurar la compatibilidad con la infraestructura existente de ERC-721.

**Implementación de Referencia y Casos de Prueba**

* Incluye pruebas en `equippableFixedParts.ts` y `equippableSlotParts.ts`.
* Implementación de referencia en `EquippableToken.sol`.

**Consideraciones de Seguridad**

* Se aplican las mismas consideraciones de seguridad que con el ERC-721: precaución con contratos no auditados y posibles lógicas ocultas en las funciones.

Este estándar representa un avance significativo en la funcionalidad y versatilidad de los NFTs, permitiendo una mayor personalización y composición de activos digitales.
