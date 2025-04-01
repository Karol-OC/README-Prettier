# README-Prettier
PRETTIER

¿QUÉ ES PRETTIER?
- Prettier es un formateador de código que mantiene un estilo consistente en tu proyecto. Formatea automáticamente tu código siguiendo reglas de estilo predefinidas, evitando discusiones innecesarias sobre el formato y mejorando la legibilidad del código.

¿CÓMO INSTALARLO?
1. Inicializar un proyecto Node.js (npm init -y)
2. Instalar Prettier como dependencia de desarrollo (npm i prettier)

REGLAS Y CONFIGURACIÓN
- Crear un archivo .prettierrc
Para personalizar el formato, crea un archivo .prettierrc en la raíz del proyecto con configuraciones como:
    {
        "singleQuote": true,
        "semi": false,
        "tabWidth": 2,
        "trailingComma": "es5"
    }
"singleQuote": true → Usa comillas simples en lugar de dobles.
"semi": false → Elimina los puntos y coma al final de las líneas.
"tabWidth": 2 → Usa 2 espacios para la indentación.
"trailingComma": "es5" → Agrega comas finales solo en objetos y arrays compatibles con ES5.

¿CÓMO SE USA?
1. Formatea archivos manualmente
Ejecuta el siguiente comando para formatear todos los archivos del proyecto:
    npx prettier --write .

2. Agregar script para formatear en package.json
Abre el archivo package.json y agrega:
    "scripts": {
        "format": "prettier --write ."
    }
Para formatear el proyecto ahora puedes ejecutar:
npm run format

EJEMPLO BÁSICO
Archivo app.js antes de Prettier:
    const helloWorld = () => {
        console.log("Hello, World!");
    };
    helloWorld();

Archivo app.js después de Prettier
    const helloWorld = () => {
        console.log('Hello, World!')
    }
    helloWorld()
