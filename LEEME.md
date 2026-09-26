# OTERO BUILT — guía para empezar

Esta carpeta contiene una página web en un solo archivo. No necesita instalar programas ni conectarse a internet para verla en tu computadora.

## 1. Abrir la página

1. Abre la carpeta `outputs`.
2. Haz doble clic en `index.html`. Se abrirá en tu navegador.
3. Usa los botones **EN / ES** del encabezado para cambiar entre inglés y español.

La página está en inglés al abrirse porque está dirigida a clientes de Indianapolis. Incluye la opción en español.

El logo elegido es la **segunda muestra**. En `assets` encontrarás `oterobuilt-logo.png` (logo completo, recortado y con fondo transparente) y `oterobuilt-mark.png` (símbolo recortado que usa el encabezado). El encabezado combina ese símbolo con un nombre en una sola línea: **OTERO** en azul y **BUILT** en naranja.

## 2. Revisar o cambiar los datos de contacto

1. Abre `index.html` con un editor de texto. Puedes usar Bloc de notas; Visual Studio Code hace más cómodo editar el código.
2. Busca `const OTERO_CONTACT` cerca del final del archivo.
3. Los datos que compartiste ya están en esta configuración. El teléfono visible conserva el formato que enviaste; el botón **Call Now** agrega el código de país de EE. UU. al enlace telefónico `tel:`. El correo activa **Email Us** y el formulario de cotización:

```js
const OTERO_CONTACT = {
  phone: "317-840-8925",
  email: "oterobuilt@gmail.com",
  facebook: "http://www.facebook.com/share/1H2Tq1quNU/",
  instagram: "",
  youtube: "https://www.youtube.com/@DRACK-IRØNŞIDE",
  tiktok: ""
};
```

Usé el enlace de Facebook que compartiste. Es un enlace con formato `/share/`; comprueba que lleve al destino que quieres antes de publicar. También compartiste el texto `@ drack Otero`, pero no lo convertí en un enlace de Instagram ni cambié su escritura. Los botones de Instagram y TikTok quedan preparados y desactivados hasta que agregues sus URLs completas. No agregué un número de WhatsApp.

4. Guarda el archivo y actualiza el navegador para ver los cambios.

**Call Now** abre el marcador del teléfono, **Email Us** abre un correo nuevo y **Request a Free Estimate** lleva al formulario. Al enviar el formulario, se prepara un correo para la dirección configurada; no se guarda en una base de datos. Para recibir solicitudes directamente desde la web, más adelante habrá que conectarlo a un servicio de formularios.

## 3. Agregar fotos de trabajos

La galería tiene tres espacios de muestra, no proyectos ficticios. Cuando tengas fotos:

1. Crea una carpeta llamada `assets` junto a `index.html`.
2. Copia ahí tus fotos, por ejemplo `roofing-01.jpg`.
3. Reemplaza el bloque de muestra correspondiente en la sección `Selected projects` / `Proyectos realizados` por una imagen como esta:

```html
<img src="assets/roofing-01.jpg" alt="Instalación de techo en Indianapolis">
```

Usa fotos propias o fotos que tengas permiso para publicar. Podemos hacer juntos ese cambio cuando tengas las imágenes.

## 4. Editar los textos

Los textos visibles están dentro de `index.html`. Muchos tienen dos versiones, identificadas por `data-en` y `data-es`; si editas un texto, cambia ambas para que las versiones en inglés y español sigan coincidiendo.

## 5. Publicar el sitio

Por ahora el archivo solo está en tu computadora. Para que clientes lo encuentren en internet habrá que elegir una dirección web propia y un servicio de publicación. Antes de lanzarlo, reemplaza los campos marcados, prueba los enlaces de contacto y agrega fotos reales. Puedo guiarte en esos pasos cuando estés listo.
