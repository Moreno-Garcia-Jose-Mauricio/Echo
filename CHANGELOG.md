# Changelog

Formato: **mayor.menor.parche**. Los parches (1.2.1, 1.2.2…) son frases guardadas desde la app y quedan en el historial de commits de `echo.json`.

## v2.1
- Inicio por filas: cada serie, película o persona en su propia fila con sus episodios (T1:E3). Las frases ya no se muestran hasta tocarlas.
- Tocar un episodio abre solo su frase (o frases); tocar el nombre abre la ventana con todas.
- Episodios sin frase en tono tenue; al tocarlos se abre el editor para escribirla.
- Frase de bienvenida en inglés con la palabra Echo.

## v2.0
- Rediseño completo en una sola pantalla: frase de bienvenida, buscador, filtros por tipo (Series, Películas, Personas) y fuentes en una tira deslizable.
- Solo se muestran las temporadas y episodios que ya tienen frase; las escenas sin frase quedan en "Por completar".
- Nuevo tipo de fuente **Persona**: científicos, profesores, frases propias u otras, con campo "Dónde o cuándo".
- Una sola hoja para agregar: eliges tipo, fuente (o creas una nueva ahí mismo), episodio y frase.
- Diálogos con varias líneas del mismo personaje se agrupan; etiqueta arriba de cada frase.

## v1.3
- Frases largas: se muestran recortadas con "Ver completa" para no saturar la pantalla.
- Diálogos entre personajes: las líneas con formato `Nombre: texto` se muestran como conversación, con cada personaje marcado.
- Mapa de episodios: tono tenue si la escena aún no tiene frase y color sólido cuando ya la tiene.
- Cartelera: cada póster muestra frases escritas sobre escenas (por ejemplo, 3/7) con barra de avance.

## v1.2
- Versión visible en la app, junto al logo y en Ajustes, con historial de novedades.
- Cada guardado desde la app sube el parche (v1.2.1, v1.2.2…) y lo incluye en el mensaje del commit.

## v1.1
- Rediseño: cada escena se muestra como página de guion (encabezado, personaje, acotación y diálogo).
- Proyección de hoy, aviso de escenas sin frase y pósters por serie.
- Selector de temporada y episodio con botones; minuto en un solo campo (39:50-42:37).
- Campo "Quién lo dice" y botón para compartir la frase.

## v1.0
- Primera versión en GitHub Pages: escenas por serie, mapa de episodios, guardado con commits vía la API de GitHub.
- Datos iniciales: 11 escenas de Suits, The Rookie y House.
