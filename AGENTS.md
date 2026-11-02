# Instrucciones permanentes para agentes

Estas reglas se aplican a todo el repositorio. Respeta también las instrucciones más específicas de los subdirectorios.

## 1. Leer el contexto antes de trabajar

- Lee `README.md`, `docs/estado.md`, `docs/decisiones.md` y `docs/tareas.md` antes de hacer cambios.
- Inspecciona la estructura real, las instrucciones adicionales, los comandos disponibles y los cambios existentes. Si hay Git local, consulta su estado y el remoto.
- No des por hecho que existen una aplicación, dependencias o pruebas: compruébalo.

## 2. Mantener orden sin duplicar ni sobrescribir

- Reutiliza los archivos y convenciones existentes. Actualiza la documentación original en vez de crear copias con nombres como `final`, `nuevo` o `v2`.
- Considera `docs/`, `src/` y `tests/` una propuesta inicial, no una obligación de mover un proyecto existente.
- No borres, reemplaces ni reorganices trabajo ajeno sin autorización. Conserva los cambios que no pertenecen a la tarea.
- Limita los cambios al objetivo solicitado; no incorpores dependencias, instalaciones o refactorizaciones innecesarias.

## 3. Actualizar estado, decisiones y pendientes

- Mantén `docs/estado.md` con lo realizado, las verificaciones reales, los problemas y el próximo paso.
- Registra decisiones relevantes y su motivo en `docs/decisiones.md`.
- Actualiza `docs/tareas.md` sin marcar como terminadas tareas no verificadas.
- Usa fechas reales y distingue lo completado, lo pendiente y lo bloqueado.

## 4. Ejecutar pruebas y documentar errores

- Descubre y ejecuta las pruebas disponibles, empezando por las relacionadas con el cambio. Ejecuta las comprobaciones de construcción y formato que estén configuradas y sean pertinentes.
- Si no hay pruebas o falta una herramienta, indícalo claramente. No inventes comandos ni presentes una revisión documental como una prueba de aplicación.
- Documenta el comando utilizado, su resultado y los errores relevantes, sin incluir secretos en los registros.
- No arregles problemas ajenos a la tarea salvo autorización expresa; descríbelos en el resumen.

## 5. Al decir «guarda progreso»

- Revisa el estado de Git y el diff, separa los cambios de la tarea de los preexistentes y comprueba que no haya secretos.
- Añade únicamente archivos revisados y crea un commit local con un mensaje descriptivo si Git está disponible y configurado.
- No hagas push con esta orden. Si no hay cambios, dilo sin crear un commit vacío.
- Si no es posible crear un commit local, explica el bloqueo. No sustituyas esta orden por un commit remoto sin autorización.

## 6. Al decir «guarda y sincroniza en GitHub»

- Realiza primero la revisión y las comprobaciones del apartado anterior.
- Confirma que la cuenta, el repositorio remoto y la rama de destino son los autorizados. El destino inicial es `loganpaulfortnite-beep/random`; no uses otro sin autorización.
- Comprueba el estado remoto antes de publicar. No fuerces un push, no reescribas el historial y no descartes cambios remotos para resolver conflictos automáticamente.
- Crea el commit y haz push cuando Git local esté disponible. Si la autorización incluye subir los cambios y solo está disponible la conexión de GitHub, puedes guardarlos con ella, verificando que las rutas no sobrescriban trabajo existente.
- Comprueba después el commit y los archivos en GitHub. Distingue «guardado localmente», «guardado mediante la conexión de GitHub» y «sincronizado mediante push»; no afirmes pasos no ejecutados.
- No publiques código o información privada mientras el repositorio sea público. Esta base solo contiene instrucciones genéricas; antes de incorporar contenido privado hay que verificar o cambiar la visibilidad con autorización.

## 7. Proteger los secretos

- Nunca añadas a Git ni subas contraseñas, tokens, claves API, archivos `.env`, claves privadas, credenciales, copias de bases de datos o certificados privados.
- Revisa el contenido y los archivos que se van a guardar: `.gitignore` no elimina archivos ya versionados ni garantiza por sí solo que no haya secretos.
- No muestres secretos en respuestas, capturas, documentación, commits o registros. No pidas que se peguen en el chat; usa el mecanismo seguro de credenciales disponible.
- Si encuentras un secreto ya versionado, detén la publicación y avisa sin reproducir su valor. No reescribas el historial ni revoques credenciales sin autorización.

## 8. Resumir el resultado

Finaliza con un resumen breve de los cambios, las pruebas y su resultado, los problemas o limitaciones y el próximo paso. Incluye el commit y el repositorio cuando se hayan guardado cambios. Indica expresamente si no se ha realizado un commit, push o despliegue.

## 9. No desplegar ni actuar fuera de alcance

- No despliegues ni cambies servicios de producción sin autorización explícita para esa acción.
- No cambies la visibilidad, los permisos o la configuración de otros repositorios sin autorización.
- No instales o reinstales T3, GitHub Desktop u otras herramientas solo por aparecer mencionadas en la documentación.
- Un commit o una sincronización no autorizan un despliegue. Si detectas automatizaciones de despliegue al hacer push, informa y resuelve ese riesgo antes de publicar.
