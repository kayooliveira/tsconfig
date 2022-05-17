# <p align="center"> My tsconfig.json

```json
{
  "compilerOptions": {
    "target": "es2020",
    "lib": ["es6"],
    "typeRoots": ["./node_modules/@types", "./src/@types"],
    "allowJs": true,
    "resolveJsonModule": false,
    "module": "commonjs",
    "rootDir": "./src",
    "outDir": "./dist",
    "esModuleInterop": true,
    "removeComments": true,
    "forceConsistentCasingInFileNames": true,
    "strict": false,
    "experimentalDecorators": true,
    "emitDecoratorMetadata": true,
    "skipLibCheck": true,
    "paths": {
      "@repositories/*": ["./src/repositories/*"],
      "@providers/*": ["./src/providers/*"],
      "@useCases/*": ["./src/useCases/*"],
      "@entities/*": ["./src/entities/*"],
      "@database/*": ["./src/database/*"]
    }
  }
}

```

--- 

<p align="center">made with :two_hearts: by Kayo Oliveira
