# docker-compose-apps

Este repositorio contiene un archivo **docker-compose.yml** que permite
orquestar una aplicación de **tres capas** (Frontend, API y Base de Datos)
utilizando imágenes Docker reforzadas en seguridad.

---

## Arquitectura

La aplicación está compuesta por los siguientes servicios:

- **Database**
  - PostgreSQL
- **API**
  - Aplicación Node.js
- **Frontend**
  - Servidor NGINX
  - Expone la interfaz web

Los servicios se comunican entre sí a través de la red interna creada por
Docker Compose.

---

## Imágenes Docker utilizadas

- Database
  `docker.io/melaniefig/db-security:1.0.0`

- API
  `docker.io/melaniefig/api-security:1.0.0`

- Frontend
  `docker.io/melaniefig/frontend-security:1.0.0`

---

## Contenido del repositorio

```text
.
├── docker-compose.yml
└── README.md
