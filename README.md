# Mainez Local · landing para GitHub y Vercel

Este proyecto es una web estática. `index.html`, `styles.css` y la carpeta `assets/` deben conservar esta estructura. La agenda de Calendly ya está integrada en la primera sección.

## Actualizar la web que ya está en GitHub

1. Descomprime el ZIP.
2. Abre el repositorio **`Josemainez/landing_mainez_local`** y sube **el contenido** de esta carpeta a la raíz de la rama `main`. No subas el ZIP como único archivo.
3. Si quieres actualizar solo lo necesario, sustituye el archivo **`index.html`** de la raíz: es el único archivo de la web que cambió para integrar el Pixel.
4. Confirma los cambios en GitHub. Vercel debería publicar automáticamente la nueva versión.

## Pixel de Meta

- ID: **1624497902558533**.
- Tras aceptar las cookies se envía `PageView`. Si se rechazan, el Pixel no se carga.
- `Lead` se envía cuando el calendario confirma la reserva. Abrir el formulario o seleccionar una fecha no cuenta como lead.
- El aviso enlaza a `https://mainezasociados.com/politicaprivacidad`, que debes activar antes de enviar tráfico de pago.

## Comprobación tras publicar

- Abre la URL de Vercel y revisa logos, tipografías y calendario.
- Pulsa un CTA desde una sección inferior: debe llevarte al calendario de arriba.
- Selecciona una fecha y comprueba que aparecen los horarios. El evento de Calendly dura 45 minutos.
- En una ventana privada, comprueba que aparece el aviso de cookies. Usa **Meta Pixel Helper** o **Eventos de prueba** para verificar `PageView` después de aceptar. Para verificar `Lead` en producción hace falta una reserva de prueba real que luego puedas cancelar.

La agenda se carga desde Calendly y requiere conexión a internet. No se necesitan variables de entorno ni dependencias de npm.
