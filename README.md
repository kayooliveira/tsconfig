# <p align="center"> My tsconfig.json
>## Node
>I know, I'm a psychopath for putting this in alphabetical order. :smile:
```json
{
    "env": {
        "es2021": true,
        "jest": true,
        "node": true
    },
    "extends": [
        "plugin:@typescript-eslint/recommended",
        "prettier",
        "standard"
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
        "eslint-plugin-import-helpers",
        "prettier"
    ],
    "rules": {
        "@typescript-eslint/camelcase": "off",
        "@typescript-eslint/explicit-function-return-type": [
            "off"
        ],
        "@typescript-eslint/explicit-module-boundary-types": [
            "warn",
            {
                "allowArgumentsExplicitlyTypedAsAny": true
            }
        ],
        "@typescript-eslint/naming-convention": [
            "error",
            {
                "custom": {
                    "match": true,
                    "regex": "^I[A-Z]"
                },
                "format": [
                    "PascalCase"
                ],
                "selector": "interface"
            }
        ],
        "@typescript-eslint/no-explicit-any": "off",
        "@typescript-eslint/no-unused-vars": [
            "error",
            {
                "argsIgnorePattern": "_"
            }
        ],
        "class-methods-use-this": "off",
        "import-helpers/order-imports": [
            "warn",
            {
                "alphabetize": {
                    "ignoreCase": true,
                    "order": "asc"
                },
                "groups": [
                    "/^@/",
                    "module",
                    [
                        "index",
                        "parent",
                        "sibling"
                    ]
                ],
                "newlinesBetween": "always"
            }
        ],
        "import/extensions": [
            "error",
            "ignorePackages",
            {
                "ts": "never"
            }
        ],
        "import/prefer-default-export": "off",
        "max-classes-per-file": 1,
        "no-console": "off",
        "no-new": "off",
        "no-prototype-builtins": "off",
        "no-restricted-syntax": "off",
        "no-underscore-dangle": "off",
        "no-useless-constructor": "off",
        "prettier/prettier": "error"
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
