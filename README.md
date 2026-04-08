# KnowMe — Portfolio de ALASTOR

Pequeño sitio estático con efecto de "cursor" personalizado y varios efectos visuales.

Resumen
- Archivo principal: `index.html`.
- Cursor personalizado: elementos `.cursor` y `.cursor-dot` controlados por JavaScript.
- Se ha añadido CSS global para ocultar el cursor nativo y la caret de inputs.

Cómo probar
1. Abrir `index.html` en un navegador moderno (Chrome, Edge, Firefox).
2. Verás el cursor personalizado en pantalla; el cursor nativo está oculto por CSS.

Revertir el ocultado del cursor nativo
- Abrir `index.html` y en el bloque `<style>` localizar las reglas agregadas:

  html, body, * {
      cursor: none !important;
  }

  input, textarea, select, [contenteditable="true"] {
      caret-color: transparent !important;
  }

- Eliminar o comentar esas reglas para restaurar el cursor del sistema y el caret.

Notas
- El cursor nativo se oculta con `cursor: none !important;`; en algunos contextos/OS puede haber comportamientos específicos del navegador.
- Si quieres que ciertos elementos (ej. botones) muestren el cursor nativo, puedo ajustar las reglas CSS para excluirlos.

¿Quieres que añada instrucciones para desplegarlo localmente con un servidor simple (`python -m http.server`) o que haga ajustes para inputs concretos?