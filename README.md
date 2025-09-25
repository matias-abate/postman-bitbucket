# demo-usuarios-tickets

Repo mínimo para demo **Bitbucket ↔ Postman**.

## Estructura
```
specs/openapi.yaml                     # OpenAPI 3.0 para importar en Postman
postman/collection.postman_collection.json  # Colección Postman (opcional)
postman/env.postman_environment.json        # Entorno Postman (opcional)
bitbucket-pipelines.yml                # CI con Newman (opcional)
```

## Cómo usar
1) Abrir carpeta en VS Code: `demo-usuarios-tickets/`
2) Subir a **Bitbucket** y en **Postman** usar *Import from Repository* → seleccionar repo y rama.
3) Postman detectará `specs/openapi.yaml` y generará colección/documentación automáticamente.
4) (Opcional) Ejecutar CI en **Bitbucket Pipelines** para correr tests con **Newman**.

## Variables
- `baseUrl` por defecto apunta a `https://api.demo.com`. Cambiar en `postman/env.postman_environment.json` o en el entorno de Postman.
