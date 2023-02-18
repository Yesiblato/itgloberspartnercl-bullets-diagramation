# BULLETS DIAGRAMATION COMPONENT

Este es un componente personalizado que permite mostrar los niveles de inferiores de navegación dentro de una lista de bullets con imágenes, y se puede renderizar de diferente maneras según el dispositivo.

En este componente se trabajó con las siguientes tecnologías:

- Vtex.
- React.
- Typescript.
- Css.

## Imágenes del componente.

- Slider en desktop.

![slider bullets](https://user-images.githubusercontent.com/87024446/219830339-88600adb-b00e-4498-b925-964f9564c453.JPG)

- Slider en mobile.

![bullets diagramation mobile](https://user-images.githubusercontent.com/87024446/219830343-e45b24de-b612-4eb9-bf99-fdc5a3e1470d.JPG)

## Configuration 

### Paso 1 - Clonar

Realizar la clonación del siguiente repositorio:
- [Repositorio](https://github.com/Yesiblato/itgloberspartnercl-bullets-diagramation)

### Paso 2 - Editar el Manifest.json 

Ingresar al archivo manifest.json y realizar las siguentes modificaciones en: `vendor`, `name`, `version`, `title` y `description`
como se muestra en el siguiente ejemplo: 

```js
{
  "vendor": "itgloberspartnercl",
  "name": "bullets-diagramation",
  "version": "0.0.1",
  "title": "Bullets Diagramation",
  "description": "Es un contexto de elementos que renderizan los nieveles inferiores de la navegación dentro de una lista de bullets con imagenes.",
}
```
Además, verifique que el archivo cuente con los siguientes builders: 

```js
  "builders": {
    "react": "3.x",
    "messages": "1.x",
    "docs": "0.x",
    "store": "0.x"
  }
```
### Paso 3 - Instalar node-modules

Para realizar esta instalación de node-modules, debe estar ubicado en la carpeta de `react` de la aplicación y ejecutar el comando `yarn`, y tendrá instaladas todas las dependencias necesarias para usar esta plantilla.

### Paso 4 - Ejecutar el preview

Despues de realizar los pasos anteriores puede verificar si su componente está funcionando ejecutando el comando `vtex link` si todo funciona correctamente deberá ver en consola `Sending locale change event`.

Si la consola muestra algún error, por favor verificar los pasos anteriores y vuelva a ejecutar `vtex link`.

### Paso 5 - Implementar el componente

Por último, para utilizar el componente debe agregarlo a las `dependencies` en el `manifest.json` de su tienda (store-theme) de la siguiente manera:

- vendor.name : version. 

Por ejemplo: 
```js
  "dependencies": {
    "itgloberspartnercl.bullets-diagramation": "0.x",
  }
```

## Dependencies
```js
   "vtex.native-types": "0.x",
   "vtex.list-context": "0.x",
   "vtex.device-detector": "0.x",
   "vtex.css-handles": "0.x"
```
## Contributors ✨

Yesica Johana Blanco Torregrosa
