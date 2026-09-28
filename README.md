# Mainez Local · landing para GitHub y Vercel

Este proyecto es una web estática. `index.html`, `styles.css` y la carpeta `assets/` deben conservar esta estructura. La agenda de Calendly ya está integrada en la primera sección.

## Subir a GitHub

1. Descomprime el ZIP.
2. Crea un repositorio nuevo en GitHub.
3. En **Add file → Upload files**, sube **el contenido** de esta carpeta: `index.html`, `styles.css`, `assets/`, `vercel.json`, `.gitignore` y `README.md`. No subas el ZIP como único archivo.
4. Comprueba que `index.html` quede en la raíz del repositorio y que `assets/` conserve sus archivos.

## Publicar en Vercel

1. En Vercel, entra en **Add New → Project** e importa ese repositorio de GitHub.
2. Usa **Framework Preset: Other** y **Root Directory: `./`**.
3. No hace falta comando de instalación ni de compilación. `vercel.json` indica que se publique la raíz del repositorio.
4. Pulsa **Deploy**. Después, cada cambio que subas a la rama de producción generará un nuevo despliegue.

## Comprobación tras publicar

- Abre la URL de Vercel y revisa logos, tipografías y calendario.
- Pulsa un CTA desde una sección inferior: debe llevarte al calendario de arriba.
- Selecciona una fecha y comprueba que aparecen los horarios. El evento de Calendly dura 45 minutos.

La agenda se carga desde Calendly y requiere conexión a internet. No se necesitan variables de entorno ni dependencias de npm.
