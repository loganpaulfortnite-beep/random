# Seguridad y publicación

## Antes de cada commit o sincronización

1. Revisa los archivos incluidos y su contenido, no solo sus nombres.
2. Confirma la cuenta, el repositorio y la rama de destino.
3. Comprueba la visibilidad antes de incorporar material privado.
4. Excluye contraseñas, tokens, claves API, `.env`, claves privadas, credenciales y datos locales.
5. Revisa que no haya automatizaciones que desplieguen sin autorización al publicar cambios.
6. Guarda únicamente los cambios de la tarea y comprueba después el resultado.

## Alcance de `.gitignore`

Las reglas evitan añadir por defecto varios archivos locales frecuentes. No detectan secretos dentro de archivos permitidos ni dejan de versionar archivos que ya estuvieran en Git. Toda publicación requiere revisar también el contenido.

Los archivos de entorno, incluidos `.env` y `.env.*`, se excluyen. Si hacen falta instrucciones de configuración, documenta solo los nombres de las variables y ejemplos ficticios en Markdown, nunca valores reales.

Los patrones de bases de datos y archivos SQL son conservadores para esta base vacía. Cuando exista una aplicación, adapta esas reglas para permitir las migraciones o los recursos necesarios tras revisar que no contienen datos privados.

## Si aparece un secreto ya publicado

Detén la sincronización y avisa sin reproducir el valor. Borrar el archivo en un commit posterior no borra el historial. Coordina la rotación y cualquier limpieza del historial con el titular antes de actuar.

## Visibilidad y credenciales

La última comprobación de este trabajo muestra un repositorio público. La documentación genérica no lo convierte en privado y `.gitignore` tampoco cambia quién puede leerlo.

Usa el almacén seguro o el flujo de autenticación de la herramienta correspondiente. No guardes tokens en archivos del proyecto ni los pegues en el chat. Una conexión de GitHub no autentica automáticamente una terminal ni instala Git.
