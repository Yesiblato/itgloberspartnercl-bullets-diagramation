# BULLETS DIAGRAMATION COMPONENT

This is a custom component that allows you to display lower levels of navigation within a list of bullets with images, and can be rendered differently depending on the device.

In this component we worked with the following technologies:

- Vtex.
- React.
- Typescript.
- Css.

## Component's images.

- Slider in desktop.

![slider bullets](https://user-images.githubusercontent.com/87024446/219830339-88600adb-b00e-4498-b925-964f9564c453.JPG)

- Slider in mobile.

![bullets diagramation mobile](https://user-images.githubusercontent.com/87024446/219830343-e45b24de-b612-4eb9-bf99-fdc5a3e1470d.JPG)

## Configuration 

### Step 1 - Clone

Cloning the following repository
- [Repository](https://github.com/Yesiblato/itgloberspartnercl-bullets-diagramation)

### Step 2 - Edit the Manifest.json 

Enter the manifest.json file and make the following changes to: `vendor`, `name`, `version`, `title` and `description`
as shown in the following example:

```js
  {
    "vendor": "itgloberspartnercl",
    "name": "bullets-diagramation",
    "version": "0.0.1",
    "title": "Bullets Diagramation",
    "description": "Es un contexto de elementos que renderizan los nieveles inferiores de la navegación dentro de una lista de bullets con imagenes.",
  }
```
Also, check that the file has the following builders and the dependencies:

```js
  "builders": {
    "react": "3.x",
    "messages": "1.x",
    "docs": "0.x",
    "store": "0.x"
  }
```

## Dependencies
```js
   "vtex.native-types": "0.x",
   "vtex.list-context": "0.x",
   "vtex.device-detector": "0.x",
   "vtex.css-handles": "0.x"
```

### Step 3 - Install node-modules.

To carry out this installation of Node-Modules, it must be located in the `react` folder of the application and execute the `yarn` command, and will have all the necessary units to use this template installed.

### Step 4 - Execute the preview.

After performing the previous steps you can verify if its component is running by running the `Vtex Link` command if everything works correctly should see in` Sending locale change event`.

If the console shows any error, please verify the previous steps and re -execute `vtex link`.

### Step 5 - Deploy the component

Finally, to use the component you must add it to the `dependencies` in the `manifest.json` of your store (store-theme) as follows:

- vendor.name : version. 

For example:
```js
  "dependencies": {
    "itgloberspartnercl.bullets-diagramation": "0.x",
  }
```
And add the list-context block to the store-theme. For example:

```js
  {
    "flex-layout.col#bullets": {
      "title": "Contenedor Bullest Diagramation col",
      "children": [
        "list-context.bullet-group"
      ]
    },
      "list-context.bullet-group": {
      "title": "Mi contexto de lista bullet",
      "children": [
        "slider-layout#bullet-group"
      ],
      "props": {
        "bullets": [
          {
            "image": "Here is your image to render",
            "titleBullet": "Here goes the title",
            "link": {
            "url": "/"
            }
          },
        ]
      }
    },
    "slider-layout#bullet-diagramation": {
    ...
    }
  }
```
 ### Bullets Props

| Prop name    | Type            | Description    | Default value                                                                                                                               |
| ------------ | --------------- | --------------------------------------------------------------------- | ---------- | 
| `img`        | `String`       | Define the image to render in the list-context       | `undefined`              |
| `titleBullet`        | `String`       | Define the title to render in the list-context       | `undefined`              |
| `Link`        | `LinkProps`       |  Define the url to render in the list-context       | `undefined`              |


## Customization

In order to apply CSS customizations in this and other blocks, follow the instructions given in the recipe on 

| CSS Handles |
| ----------- | 
| `bullet__container` | 
| `bullet__item` | 
| `bullet__item--title` | 
| `bullet__item--image` | 
| `bullet__item--link` |




Check out some documentation models that are already live: 
- [CSS Handles](https://vtex.io/docs/recipes/style/using-css-handles-for-store-customization)
- [Breadcrumb](https://github.com/vtex-apps/breadcrumb)
- [Image](https://vtex.io/docs/components/general/vtex.store-components/image)
- [Condition Layout](https://vtex.io/docs/components/all/vtex.condition-layout@1.1.6/)
- [Add To Cart Button](https://vtex.io/docs/components/content-blocks/vtex.add-to-cart-button@0.9.0/)
- [Store Form](https://vtex.io/docs/components/all/vtex.store-form@0.3.4/)



## Contributors ✨

Yesica Johana Blanco Torregrosa
