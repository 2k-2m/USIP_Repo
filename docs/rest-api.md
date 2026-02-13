# Especificación REST API - Módulo Usuarios



## [POST] /api/auth/login

**Payload:**

```json

{ "email": "user@example.com", "password": "secure\_password" }
```

**Response (200 OK):**

```json
{ "email": "user@example.com", "password": "secure\_password" }
```