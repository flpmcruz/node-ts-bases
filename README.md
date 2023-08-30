# 02 Bases de Node
* En este proyecto se explican como hacer factory functions y adapters.
* Y una buena introducción a los tests con Jest
* Se explica un ejemplo del logger winston con un adapter

# Ver package.json para los scripts y dependencias
Correr en Dev
```
npm run dev
```

## Config Jest
# Pasos para configurar Jest con TypeScript, en Node 

Documentación [oficial sobre Jest](https://jestjs.io/docs/getting-started)

1. Instalaciones de desarrollo (super test es útil para probar Express)
```
npm install -D jest @types/jest ts-jest supertest
```

2. Crear archivo de configuración de Jest
```
npx jest --init
```

3. En el archivo **jest.config.js** configurar
```
preset: 'ts-jest',
testEnvironment: "jest-environment-node",

// Opcional - The paths to modules that run some code to configure or set up the testing environment before each test
// setupFiles: ['dotenv/config'],
```

4. Crear scripts en el **package.json**
```
"test": "jest",
"test:watch": "jest --watch",
"test:coverage": "jest --coverage",
```