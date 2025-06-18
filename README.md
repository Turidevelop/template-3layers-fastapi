# template-3layers-fastapi

> 🧱 Plantilla base para proyectos en Python — minimalista, adaptable y extensible.

## 📌 Descripción

`template-3layers-fastapi` es una **plantilla vacía y estructurada** para proyectos desarrollados en Python. Su propósito es servir como punto de partida común para crear aplicaciones o sistemas con una base limpia y bien organizada.

Esta plantilla **no impone una arquitectura específica**, sino que proporciona una estructura mínima que puede adaptarse a cualquier necesidad **vertical** (según el dominio del proyecto, ya sea web, CLI, ciencia de datos, automatización, APIs, etc.).

Ideal para equipos o desarrolladores que buscan un punto de partida común y personalizable para sus desarrollos Python.

---

## 📁 Estructura del proyecto

```bash
template-3layers-fastapi/
├── .env                     # Plantilla para variables de entorno
├── .gitignore               # Archivos ignorados por Git
├── requirements.txt         # Dependencias de Python
├── README.md                # Documentación principal del proyecto
├── main.py                  # Punto de entrada de la aplicación
│
├── core/                    # Lógica de negocio central
│   ├── config.py            # Configuración de la aplicación
│   ├── models.py            # Modelos de dominio (Pydantic)
│   └── schemas.py           # Esquemas de datos
│
├── services/                # Lógica de aplicación
│   └── example_service.py    # Servicio para operaciones con viajes
│
├── repositories/            # Acceso a datos
│   ├── base.py              # Interfaz base para repositorios
│   └── example_repo.py       # Implementación para viajes
│
├── api/                     # Capa de presentación
│   ├── dependencies.py      # Dependencias inyectables
│   └── endpoints/           # Endpoints de la API
│       └── example.py       # Endpoints específicos para viajes
│
└── database.py              # Configuración de base de datos

