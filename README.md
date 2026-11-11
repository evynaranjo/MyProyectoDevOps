# MyProyectoDevOps

Repositorio de práctica para aprender a organizar un proyecto de desarrollo y aplicar conceptos básicos de Git, GitHub y DevOps.

## Objetivo
Organizar un proyecto en áreas de backend, frontend, base de datos, documentación, recursos gráficos y automatización.

## Estructura

```text
MyProyectoDevOps/
├── backend/              # Servicios y lógica del servidor
├── frontend/             # Interfaz de usuario
├── database/             # Scripts y modelos de base de datos
├── docs/                 # Documentación adicional
├── images/               # Recursos visuales del proyecto
├── .github/
│   └── workflows/        # Automatizaciones de GitHub Actions
├── README.md             # Presentación y uso del repositorio
├── LICENCE               # Licencia de software MIT
└── .gitignore            # Archivos excluidos del control de versiones
```

Las carpetas de desarrollo contienen un archivo `.gitkeep` temporal para que Git pueda incluirlas aunque no tengan código todavía.

## Cómo empezar

1. Clona el repositorio o descarga su contenido.
2. Abre la carpeta en Visual Studio Code.
3. Agrega los archivos de cada componente en su carpeta correspondiente.
4. Revisa las reglas de `.gitignore` antes de confirmar cambios.

## Automatización
En `.github/workflows/verificar-estructura.yml` se incluye una comprobación básica de las carpetas y archivos del proyecto. Se ejecuta al realizar un push o abrir una pull request.

## Estado del proyecto
Estructura inicial de práctica. No contiene todavía una aplicación funcional.

## Licencia
Este repositorio utiliza la licencia MIT. Consulta `LICENCE` y reemplaza el marcador del titular de los derechos de autor antes de publicarlo como proyecto propio.
