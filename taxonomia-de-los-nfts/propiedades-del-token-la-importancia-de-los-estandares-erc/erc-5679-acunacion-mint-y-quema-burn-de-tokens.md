# ERC-5679: Acuñación(Mint) y Quema(Burn) de Tokens

El ERC-5679 es una propuesta de mejora para Ethereum que busca estandarizar las funciones de acuñación (minting) y quema (burning) para los tokens basados en los estándares EIP-20, EIP-721 y EIP-1155. Este estándar propone una manera consistente de manejar estas acciones, completando así el ciclo de vida básico de los tokens.

### ERC-5679: Acuñación y Quema de Tokens

**Resumen**

* **Objetivo**: Proporcionar una manera estandarizada de acuñar y quemar tokens, aplicable a varios estándares de tokens.
* **Aplicación**: Adecuado para todos los tokens que siguen los estándares EIP-20 (tokens fungibles), EIP-721 (NFTs) y EIP-1155 (tokens híbridos).

**Especificaciones**

* **Funciones para EIP-20**: `mint` para crear tokens y `burn` para destruirlos.
* **Funciones para EIP-721**: `safeMint` para acuñar de forma segura NFTs y `burn` para destruirlos.
* **Funciones para EIP-1155**: `safeMint`, `safeMintBatch` para acuñar uno o varios tokens de forma segura, y `burn`, `burnBatch` para destruir uno o varios tokens.

**Motivación**

* **Necesidad de Estandarización**: Algunas implementaciones de EIP-721 y EIP-1155 utilizan métodos de transferencia para acuñar y quemar tokens, pero carecen de consistencia en sus interfaces.
* **Simplificación y Seguridad**: Crear métodos separados para la acuñación y la quema simplifica las implementaciones y reduce los errores de seguridad.

**Racional**

* **Consistencia con Estándares Existentes**: Cada token sigue su propia forma estándar de representar la cantidad de token, manteniendo la consistencia con sus estándares originales.
* **Uso de Eventos de Transferencia Existentes**: Se recomienda utilizar eventos de transferencia existentes para la máxima compatibilidad.

**Compatibilidad**

* **Con EIP-20, EIP-721 y EIP-1155**: Diseñado para ser compatible con estos estándares respectivamente.
* **No se Aplica a EIP-777**: El EIP-777 ya maneja la acuñación y la quema por sí mismo.

**Consideraciones de Seguridad**

* **Control de Acceso para Acuñación**: Debe diseñarse cuidadosamente para evitar emisiones fraudulentas y un aumento indebido del suministro total.
* **Control de Acceso para Quema**: Generalmente, solo el poseedor actual del token o un rol con privilegios especiales debería tener permiso para quemar tokens.

El ERC-5679 ofrece un marco coherente para agregar funcionalidades de acuñación y quema a los tokens, abordando una necesidad crucial en el espacio de los tokens digitales y aumentando la eficiencia y seguridad en su manejo.
