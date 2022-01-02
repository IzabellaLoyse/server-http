# Módulos do NodeJS

- Os módulos conjuntos de códigos

  ## 3 Tipos de Módulos

- Todos os arquivos JavaScript são módulos
- Nativos
- npm (Node Package Manager)


  ## Exportação de Módulo

  ```js
  function printName(name) {
    console.log(name);
  }

  const lastName = 'Candido';

  module.exports = { printName, lastName };
  ```

  ou

  ```js
  exports.printName = (name) => {
    console.log(name);
  };

  exports.lastName = 'Candido';
  ```

  ## Importação de Módulo

  ```js
  const { printName, lastName } = require(./service.js);

  printName(`Izabella ${lastName}`);

  ```

  ## Importação de Módulos Nativos

  ```js
  const os = require('os');

  console.log(os.type());
  ```
