# Componentes
Web components para nuestros productos

## Configuración

Cualquier componente disponible puede ser instalado utilizando `bower`. En el archivo de configuración `bower.json` introduce los componentes a utilizar en la lista de dependencias.

```
{
  "dependencies"  : {
    "dgm-navbar"  : "mxabierto/dgm-navbar#^0.0.7"
  }
}
```

Una vez listados los componentes a utilizar instalalos con:

```
bower install
```

## Dependencias

Para utilizar los componentes web en cualquier aplicación es necesario utilizar `Polymer`.

`Polymer` requiere el componente HTML `polymer` y la librería `webcomponents.js` ambos son instalados como dependecias utilizando bower.

## Instalación

Una vez instalado el componente utilizando `bower` se creará una estructura como la siguiente:

```
- bower_components
  - dgm-navar
  - polymer
  - webcomponentsjs
```

Para utilizar los componentes es necesario incluir `webcomponents.js`, incluye el siguiente script antes de la etiqueta de cierre `</body>`.

```
<script src="bower_components/webcomponentsjs/webcomponents-lite.min.js"></script>
```

Y en la etiqueta `<head>` del documento.

```
<link rel="import" href="bower_components/polymer/polymer.html">
<link rel="import" href="bower_components/dgm-navbar/dgm-navbar.html">
```

No olvides reemplazar el path a `bower_components` que corresponda a tu instalación.

Ya que hayas incluido el componente y las dependencias necesarias, basta con agregar el tag HTML en el sitio donde deba colocarse el componente.

```
<dgm-navbar></dgm-navbar>
```

## Visualización

Para visualizar los componentes existentes es necesario realizar una copia del repositorio de manera recursiva.

```
git clone --recursive https://github.com/mxabierto/componentes.git
```

Esto generará una copia de la aplicación `mxabierto/componentes` incluyendo los diferentes submodulos con los componentes existentes.

Una vez con la aplicación descargada serán necesarias las dependencias `nodejs` para su instalación basta correr el siguiente comando en la raíz de la aplicación.

```
npm isntall
```

Esto creará una nueva carpeta `node_modules` e instalará la dependencía `polyserve`. Una vez hecho esto ejecuta el comando `./node_modules/polyserve/bin/polyserve` y apunta el navegador a la dirección `http://localhost:8080/components/MXAbiertoWebComponents/` en donde se presentará una ventana con un dropdown de los componentes existentes, incluyendo documentación y una demostración del componente.
# componentes
