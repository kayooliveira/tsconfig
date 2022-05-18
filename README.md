# <p align="center"> My tsconfig.json
>## Node
>I know, I'm a psychopath for putting this in alphabetical order. :smile:
```json
{
  "env": {
    "es2021": true,
    "node": true,
    "jest": true
  },
  "extends": [
    "standard",
    "plugin:@typescript-eslint/recommended",
    "prettier"
  ],
  "globals": {
    "Atomics": "readonly",
    "SharedArrayBuffer": "readonly"
  },
  "parser": "@typescript-eslint/parser",
  "parserOptions": {
    "ecmaVersion": "latest",
    "sourceType": "module"
  },
  "plugins": [
    "@typescript-eslint",
    "prettier",
    "eslint-plugin-import-helpers"
  ],
  "rules": {
    "no-new": "off",
    "no-prototype-builtins": "off",
    "no-restricted-syntax": "off",
    "max-classes-per-file": 1,
    "@typescript-eslint/no-explicit-any": "off",
    "no-console": "off",
    "import/prefer-default-export": "off",
    "@typescript-eslint/explicit-function-return-type": ["off"],
    "@typescript-eslint/no-unused-vars": [
      "error",
      {
        "argsIgnorePattern": "_"
      }
    ],
    "no-useless-constructor": "off",
    "@typescript-eslint/naming-convention": [ 
      "error", 
      { 
        "selector": "interface", 
        "format": ["PascalCase"], 
        "custom": { 
          "regex": "^I[A-Z]", 
          "match": true 
        } 
      } 
    ],
    "@typescript-eslint/explicit-module-boundary-types": ["warn", {
      "allowArgumentsExplicitlyTypedAsAny": true
    }],
    "no-underscore-dangle": "off",
    "@typescript-eslint/camelcase": "off",
    "prettier/prettier": "error",
    "class-methods-use-this": "off",
    "import/extensions": [
      "error",
      "ignorePackages",
      {
        "ts": "never"
      }
    ],
    "import-helpers/order-imports": [
      "warn",
      {
        "newlinesBetween": "always", // new line between groups
        "groups": [
          "module",
          "/^@/",
          ["parent", "sibling", "index"]
        ],
        "alphabetize": { "order": "asc", "ignoreCase": true }
      }
    ]
  },
  "settings": {
    "import/resolver": {
      "typescript": {
        "project": "./tsconfig.json"
      }
    }
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
