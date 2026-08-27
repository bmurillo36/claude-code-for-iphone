# CLAUDE.md — Claude Code for iPhone

La web publica de venta y la **guia de instalacion** del producto. Tres ficheros
y nada mas: `index.html`, `guia-instalacion.html` y `guia-instalacion.pdf`.

## Que es

Estatico puro, sin compilacion y sin dependencias. Es el repositorio **publico**
de la cuenta (los demas son privados), justamente porque es el escaparate.

El producto que explica es [[claude-movil]]: Claude Code en un VPS propio,
manejado desde el iPhone por una terminal web con tmux persistente.

## La regla que mas veces se ha roto aqui

**El HTML y el PDF tienen que decir lo mismo.** El PDF no se regenera solo: si
cambias `guia-instalacion.html` y no vuelves a exportar el PDF, quedan dos guias
que se contradicen y el cliente lee la que se descargo. Ya paso con el precio,
que estaba a 9,99 € **al año** en un sitio y **al mes** en el otro.

Precio correcto: **9,99 €/mes**. Y **Claude Code funciona con el plan Pro** de
Anthropic; Max solo hace falta si se topa con el limite semanal.

## Lo que la guia debe exigir, y por que

El token de GitHub tiene que crearse con **«All repositories»**, no con «Only
select repositories». Con la opcion restringida, la pantalla de GitHub de la app
lista dos repositorios en vez de los veintiuno y parece un fallo del programa
cuando es un permiso del token. La guia lo indujo una vez; ya esta corregido, no
lo reintroduzcas.

## Publicar

GitHub Pages: `git push` a `main`.
