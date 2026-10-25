# Echo

The lines that keep echoing: favorite scenes from shows and movies.

App personal para guardar escenas y frases de series y películas, con el minuto exacto, el episodio y un mapa visual de temporadas.

## Cómo funciona

- **App:** `index.html`, un solo archivo HTML, publicado con GitHub Pages.
- **Datos:** `echo.json`, con todas las escenas (`clips`) y las temporadas de cada serie (`catalog`).
- **Guardar:** cada escena que agregas, editas o eliminas desde la app es un commit a `echo.json` vía la API de GitHub.

## Configuración

1. **Pages:** Settings → Pages → *Deploy from a branch* → `main` / `(root)`.
2. **Token:** crea un fine-grained token con acceso solo a este repo y permiso **Contents: Read and write**.
3. **Conectar:** abre la app, toca ⚙ y pega el token. Se guarda solo en el navegador de ese dispositivo.

Sin token, la app funciona en modo solo lectura.

## Versiones

La versión aparece en la app (junto al logo y en Ajustes) y en cada commit.

| Cambio | Ejemplo | Quién lo sube |
|---|---|---|
| **Mayor**: cambio de fondo en la app, solo cuando se pide | 1.x → 2.0 | Claude, a petición |
| **Menor**: cambio en la app (diseño, funciones) | 1.2 → 1.3 | Claude |
| **Parche**: frases y escenas guardadas desde la app | 1.2.1, 1.2.2… | La app, en automático |

El número de parche vive en `echo.json` (`meta.patch`) y se reinicia cuando sale una nueva versión de la app. Las versiones de la app están marcadas con tags (`v1.0`, `v1.1`, `v1.2`…). Historial completo en [CHANGELOG.md](CHANGELOG.md).

## Formato de una escena

```json
{
  "id": "suits-t7e10b",
  "show": "Suits",
  "kind": "serie",
  "platform": "Netflix",
  "season": 7,
  "episode": 10,
  "episodeTitle": "Donna",
  "start": "43:40",
  "end": "44:30",
  "label": "El beso",
  "character": "",
  "quote": "",
  "note": ""
}
```
