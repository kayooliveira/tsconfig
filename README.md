# <p align="center"> My tsconfig.json
>## Node
>I know, I'm a psychopath for putting this in alphabetical order. :smile:
```json
{ 
  "compilerOptions": {
    "allowJs": true,
    "emitDecoratorMetadata": true,
    "esModuleInterop": true,
    "experimentalDecorators": true,
    "forceConsistentCasingInFileNames": true,
    "lib": ["es6"],
    "module": "commonjs",
    "outDir": "./dist",
    "paths": {
      "@/*": ["./src/*"],
      "@database/*": ["./src/database/*"]
      "@entities/*": ["./src/entities/*"],
      "@providers/*": ["./src/providers/*"],
      "@repositories/*": ["./src/repositories/*"],
      "@useCases/*": ["./src/useCases/*"],
    }
    "removeComments": true,
    "resolveJsonModule": false,
    "rootDir": "./src",
    "skipLibCheck": true,
    "strict": false,
    "target": "es2020",
    "typeRoots": ["./node_modules/@types", "./src/@types"],
  }
}

```
>## React
```json
{
  "compilerOptions": {
    "allowJs": false,
    "allowSyntheticDefaultImports": true,
    "esModuleInterop": false,
    "forceConsistentCasingInFileNames": true,
    "isolatedModules": true,
    "jsx": "react-jsx",
    "lib": ["DOM", "DOM.Iterable", "ESNext"],
    "module": "ESNext",
    "moduleResolution": "Node",
    "noEmit": true,
    "resolveJsonModule": true,
    "skipLibCheck": false,
    "strict": true,
    "target": "ESNext",
    "useDefineForClassFields": true
  },
  "include": ["./src"]
}
```
--- 

<p align="center">made with :two_hearts: by Kayo Oliveira
