# Yarn 

## Índice
   
* [Instalación global](#instalación-global)
* [Inicialización de un proyecto](#inicialización-de-un-proyecto)
* [Añadir dependencias](#añadir-dependencias)
* [Eliminar dependencias](#eliminar-dependencias)
* [<em>Updgrade</em> o <em>donwgrade</em> dependencias](#updgrade-o-donwgrade-dependencias)
* [Encontrar dependencias <em>outdated</em>](#encontrar-dependencias-outdated)
* [Dependencias en modo plano](#dependencias-en-modo-plano)
* [Instalar dependencias](#instalar-dependencias)
* [Limpiar caché local](#limpiar-caché-local)
* [Ejecutar scripts](#ejecutar-scripts)
* [Instalar <em>packages</em> globalmente](#instalar-packages-globalmente)
* [Información adicional](#información-adicional) 

## Instalación global

```
npm i -g yarn
```

## Inicialización de un proyecto

```
yarn init -y
```

- `-y` Responde `yes` a todas las preguntas.

## Añadir dependencias

`add` guarda las dependencias en `dependencies` por defecto.

```
yarn add package-name
yarn add package-name@1.2.3 --> versión específica
yarn add package-name --dev --> devDependency
```

## Eliminar dependencias

`remove` elimina las dependencias del package.json, node_modules y del archivo yarn.lock.

```
yarn remove package-name
```

## _Updgrade_ o _donwgrade_ dependencias

```
yarn upgrade package-name --> actualiza a la última versión
yarn upgrade package-name@0.1.1
```

## Encontrar dependencias _outdated_

```
yarn outdated
```

## Dependencias en modo plano

package.json
```json
{
  "flat": true
}
```

## Instalar dependencias 

Instalar por primera vez en un proyecto o limpiar node_modules después de eliminar dependencias manualmente en el package.json

```
yarn install
```

## Limpiar caché local

```
yarn cache clean
```

## Ejecutar scripts

package.json
```json
{
  "scripts": {
    "serve": "node server",
    "test": "node test"
  }
}
```

¡`run` es opcional!

```
yarn run serve
yarn serve
```

## Instalar _packages_ globalmente

```
yarn global add package-name
```

------



## Información adicional

- [Yarn](https://yarnpkg.com/)
- [Yarn in 30 minutes (Vídeo)](http://www.mead.io/yarn/)