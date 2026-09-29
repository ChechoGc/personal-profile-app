# Personal Profile App

Solución al proyecto **Build a Personal Profile App** de la certificación
[Back-End Development and APIs](https://www.freecodecamp.org/learn/back-end-development-and-apis-v9) de freeCodeCamp.

Servidor HTTP con Express que expone un perfil personal en cuatro rutas.

## Uso

```bash
npm install
node server.js
```

El servidor queda escuchando en `http://localhost:3000`.

## Rutas

| Método | Ruta | Respuesta |
|---|---|---|
| GET | `/` | Mensaje de bienvenida |
| GET | `/hobbies` | Aficiones, en texto plano |
| GET | `/skills` | Tecnologías, en texto plano |
| GET | `/api/profile` | JSON con `name`, `hobbies` y `skills` |

Las tres primeras responden con `res.send()`, que envía texto. La última usa
`res.json()`, que serializa un objeto de JavaScript y añade la cabecera
`Content-Type: application/json`.
