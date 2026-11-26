# Twitter — base de datos de prueba con json-server

Arranque de un clon de Twitter. Por ahora solo tiene el `db.json`, el archivo que usa [json-server](https://github.com/typicode/json-server) para levantar una API REST falsa sin programar un backend.

## Qué hay

`db.json` trae los datos de ejemplo de json-server:

- `posts`: una lista de publicaciones (por ahora un post de prueba).
- `profile`: el perfil del usuario.

## Cómo levantar la API

```bash
npx json-server --watch db.json
```

Así quedan disponibles, por ejemplo:

- `GET http://localhost:3000/posts` → lista de posts
- `POST http://localhost:3000/posts` → crea un post
- `GET http://localhost:3000/profile` → perfil

json-server guarda los cambios directamente en `db.json`.

## Estado

Solo está la base de datos. Falta el front que consuma la API.
