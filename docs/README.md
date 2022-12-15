# Linio Store

Linio store es una tienda virtual que se hizo apartir de la plataforma de VTEX IO<br/>
Linio store es una copia de la tienda [Linio](http://linio.com.co)

### Linio Store

**Home**
![Linio](./images/preview.png)
<!-- ![Linio](./images/preview1.png)
![Linio](./images/preview2.png)
![Linio](./images/preview3.png)
![Linio](./images/preview4.png) -->




## Configuracion

### Paso 1

Acceda a la guia basica de configuracion de [VTEX IO](https://vtex.io/docs/getting-started/build-stores-with-store-framework/1). Ademas de esto debera tener instalado el [CLI](https://developers.vtex.com/vtex-developer-docs/docs/vtex-io-documentation-vtex-io-cli-installation-and-command-reference) (Command Line Interface) de VTEX IO

### Paso 2 - Clonar el repositorio

[Clona](https://github.com/MiguelFoliaco/store-theme-linio) este repositorio en tu maquina local para poder trabajar y accede a el por tu terminal.

### Paso 3 - Edita el `manifest.json`

Una vez clonado el repositorio hay que hacer unas cuantas modificaciones en el manifest.json del proyecto.

Tendras que modificar valores de la propiedad `vendor` por el nombre de la cuenta en la que estes trabajando. la propiedad `name` no es obligatoria modificarla para su uso pero puedes cambiarla por el nombre que quieras

```json
{
  "vendor": "storecomponents",
  "name": "my-test-theme"
}
```

### Step 4 - Instala las app requeridas

Para usar Store Framework y trabajar en el tema de su tienda, es necesario tener instalados `vtex.store-sitemap` y `vtex.store`.

Ejecute `vtex list` y verifique si esas aplicaciones ya están instaladas.

Si no lo están, ejecute el siguiente comando para instalarlos: `vtex install vtex.store-sitemap vtex.store -f`

Adicionalmente tendras que instalar las siguientes aplicaciones customizadas de la tienda

```json
{
  "{vendor}.whatsapp-button": "0.x",
  "{vendor}.bullets-diagramations": "0.x",
  "{vendor}.add-to-cart-info": "0.x",
  "{vendor}.read-pdf": "0.x",
  "{vendor}.special-diagramations": "0.x"
}
```

#### Aplicaciones

| Nombre                                                                                                | Version |
| ----------------------------------------------------------------------------------------------------- | ------- |
| [{vendor}.whatsapp-button](https://github.com/MiguelFoliaco/itgloberspartnercl.whatsapp-button)       | 0.x     |
| [{vendor}.bullets-diagramations](https://github.com/MiguelFoliaco/itgloberspartnercl.whatsapp-button) | 0.x     |
| [{vendor}.add-to-cart-info](https://github.com/MiguelFoliaco/itgloberspartnercl.whatsapp-button)      | 0.x     |
| [{vendor}.read-pdf](https://github.com/MiguelFoliaco/itgloberspartnercl.whatsapp-button)              | 0.x     |
| [{vendor}.special-diagramations](https://github.com/MiguelFoliaco/itgloberspartnercl.whatsapp-button) | 0.x     |

### Paso 5 - Desinstalar el store-theme predeterminado

Al ejecutar `vtex list`, puede verificar si algún tema está instalado.

Es común tener ya instalado un `vtex.store-theme` cuando inicia el proceso de desarrollo frontal de la tienda.

Por lo tanto, si lo encuentra en la lista de aplicaciones, copie su nombre y version, luego utilícelo junto con el comando `vtex uninstall`. Por ejemplo:

```json
vtex uninstall vtex.store-theme@0.0.1
```

### Paso 6 - Ejecute un preview de la tienda

Entonces ha llegado el momento de cargar todos los cambios que realizó en sus archivos locales a la plataforma. Para eso, use el comando `vtex link`.

Si el proceso se ejecuta sin ningún error, se mostrará el siguiente mensaje: `Aplicación vinculada con éxito`. Luego, ejecute el comando `vtex browser` para abrir una ventana del navegador que tenga su tienda vinculada.

Esto le permitirá ver los cambios aplicados en tiempo real, a través de la cuenta y el espacio de trabajo en el que está trabajando.

## peerDependencies

```json
{
  "vtex.mega-menu": "2.x"
}
```

## Store Components

```json
{
  "vtex.store": "2.x",
  "vtex.store-icons": "0.x",
  "vtex.store-link": "0.x",
  "vtex.store-header": "2.x",
  "vtex.store-image": "0.x",
  "vtex.product-summary": "2.x",
  "vtex.store-footer": "2.x",
  "vtex.store-components": "3.x",
  "vtex.styleguide": "9.x",
  "vtex.slider": "0.x",
  "vtex.carousel": "2.x",
  "vtex.shelf": "1.x",
  "vtex.menu": "2.x",
  "vtex.minicart": "2.x",
  "vtex.product-highlights": "2.x",
  "vtex.product-details": "1.x",
  "vtex.product-kit": "1.x",
  "vtex.search-result": "3.x",
  "vtex.search": "2.x",
  "vtex.search-resolver": "1.x",
  "vtex.login": "2.x",
  "vtex.my-account": "1.x",
  "vtex.flex-layout": "0.x",
  "vtex.rich-text": "0.x",
  "vtex.store-drawer": "0.x",
  "vtex.locale-switcher": "0.x",
  "vtex.product-quantity": "1.x",
  "vtex.product-price": "1.x",
  "vtex.product-identifier": "0.x",
  "vtex.product-specification-badges": "0.x",
  "vtex.product-review-interfaces": "1.x",
  "vtex.telemarketing": "2.x",
  "vtex.order-placed": "2.x",
  "vtex.stack-layout": "0.x",
  "vtex.tab-layout": "0.x",
  "vtex.modal-layout": "0.x",
  "vtex.responsive-layout": "0.x",
  "vtex.slider-layout": "0.x",
  "vtex.iframe": "0.x",
  "vtex.breadcrumb": "1.x",
  "vtex.sticky-layout": "0.x",
  "vtex.add-to-cart-button": "0.x",
  "vtex.product-specifications": "1.x",
  "vtex.product-gifts": "0.x",
  "itgloberspartnercl.whatsapp-button": "0.x",
  "itgloberspartnercl.bullets-diagramations": "0.x",
  "itgloberspartnercl.add-to-cart-info": "0.x",
  "itgloberspartnercl.read-pdf": "0.x",
  "itgloberspartnercl.special-diagramations": "0.x",
  "vtex.store-newsletter": "1.x",
  "vtex.category-menu": "2.x",
  "vtex.disclosure-layout": "1.x"
}
```
