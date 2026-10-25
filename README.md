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
  "quote": "",
  "note": ""
}
```
