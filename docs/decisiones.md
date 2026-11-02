# Decisiones

## 2026-11-02 — Usar un repositorio existente y vacío

Se utiliza `loganpaulfortnite-beep/random` porque el usuario autoriza usar otro nombre y se ha comprobado que está vacío. No se renombran ni modifican los demás repositorios.

## 2026-11-02 — Publicar únicamente una base genérica

El destino sigue siendo público. La base no incluye secretos, datos personales del trabajo ni código privado. Se documenta la necesidad de verificar o cambiar la visibilidad antes de incorporar información privada; no se cambia la configuración de acceso.

## 2026-11-02 — No elegir una tecnología todavía

No se ha recibido código de una aplicación ni requisitos funcionales. Se reservan `src/` y `tests/` con una explicación de su propósito y no se añaden dependencias ni comandos ficticios.

## 2026-11-02 — Separar el guardado remoto del Git local

La conexión de GitHub está disponible, pero Git local no lo está y GitHub CLI no está autenticado. Para esta petición de subir la base se usará la conexión de GitHub, sin presentarlo como un commit o push realizados desde Windows.
