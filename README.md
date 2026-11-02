# Base de organización de proyectos

Repositorio de partida para trabajar con una IA de forma ordenada, documentar el progreso y conservar un historial en GitHub. No contiene todavía una aplicación ni un catálogo de Alion Tech.

Destino autorizado: `loganpaulfortnite-beep/random`.

## Estructura

```text
AGENTS.md             Reglas permanentes para la IA
README.md             Descripción y forma de trabajar
docs/
  objetivos.md        Alcance y criterios de la base
  estado.md           Avance, verificaciones y limitaciones
  decisiones.md       Decisiones y motivos
  tareas.md           Trabajo pendiente
  seguridad.md        Protección de secretos y publicación
src/
  README.md           Reserva para el código de la aplicación
tests/
  README.md           Reserva para las pruebas automáticas
.gitignore            Exclusiones de secretos y archivos locales
```

Adapta esta estructura a cada proyecto real. No muevas código ni sustituyas archivos existentes solo para ajustarte a este esquema. Mantén proyectos distintos en repositorios separados, no todos dentro de este repositorio.

## Cómo empezar en T3 Code

1. Abre la carpeta local correspondiente al repositorio con el que vayas a trabajar. Esta carpeta de preparación contiene los archivos de la base, pero no es aún un clon Git.
2. Pide a la IA que lea `AGENTS.md` y la documentación de `docs/`.
3. Define el objetivo y aporta o identifica el código real antes de pedir cambios en una aplicación.
4. Comprueba el resultado, guarda el progreso y sincroniza cuando lo solicites.

Para trabajar con commits locales, primero necesitas Git instalado y un clon de este repositorio. La conexión de GitHub y la autenticación de la terminal son independientes: que una esté conectada no implica que la otra lo esté.

## Cómo ejecutar la aplicación y las pruebas

No aplica todavía: no hay aplicación, gestor de dependencias ni pruebas automáticas configuradas. No hay que ejecutar `npm install`, `npm test` ni otros comandos de una tecnología que aún no se ha elegido.

Cuando exista una aplicación, actualiza este apartado con requisitos, instalación, ejecución, pruebas y construcción, usando comandos realmente comprobados.

## Órdenes de trabajo

- **«Guarda progreso»**: revisa los cambios y los secretos y crea un commit local descriptivo. No sube cambios. Requiere Git local.
- **«Guarda y sincroniza en GitHub»**: revisa y comprueba los cambios, verifica el destino autorizado, guarda el commit y sincroniza; confirma el resultado remoto. Si se usa la conexión de GitHub en lugar de Git local, debe indicarse.
- **«Modifica el catálogo, comprueba que funciona y guarda y sincroniza el progreso»**: úsala cuando el repositorio ya contenga el catálogo real. No autoriza desplegarlo.

## Seguridad y privacidad

**Este repositorio era público al comprobarlo el 2 de noviembre de 2026.** Esta primera base contiene solo instrucciones y documentación genéricas. No contiene credenciales ni código privado.

Antes de incorporar material privado, verifica que el repositorio sea privado. Cambiar la visibilidad no retira copias que terceros pudieran haber hecho antes. No se han cambiado la visibilidad ni los demás repositorios de la cuenta.

Consulta `docs/seguridad.md`. Las exclusiones de `.gitignore` son una primera barrera, no una garantía automática.
