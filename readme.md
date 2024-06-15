# Configuracion de Biome
## herramienta de linter y formateado de codigo

- Biome
- Husky


Biome, Husky necesita [Node.js](https://nodejs.org/) v18+

## instalación
instalar Biome
```sh
npm install --save-dev --save-exact @biomejs/biome
```
Crear archivo config de Biome
```sh
npx @biomejs/biome init
```
instalar Husky
```sh
npm install --save-dev husky
```
Crear archivo config de husky
```sh
npx husky init
```

## Agregar scripts en el package.json

| script | valor |
| ------ | ------ |
| "biome:format:check" | "biome format ./src", |
| "biome:format:write" | "biome format --write ./src", |
| "biome:lint:check" | "biome lint ./src" |
| "biome:lint:write" | "biome check --apply", |

## Agregar script en el pre-commit (husky)
```sh
npm run biome:format:write
```
De esta manera cuando se haga un commit primero formateara los archivos del proyecto
