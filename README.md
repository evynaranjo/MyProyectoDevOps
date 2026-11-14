# MyProyectoDevOps

[![Verificar estructura](https://github.com/evynaranjo/MyProyectoDevOps/actions/workflows/verificar-estructura.yml/badge.svg)](https://github.com/evynaranjo/MyProyectoDevOps/actions/workflows/verificar-estructura.yml)

> Repositorio académico para practicar la organización de proyectos de software, el control de versiones con Git y la automatización básica con GitHub Actions.

**Estado:** estructura inicial de aprendizaje. **Aún no contiene una aplicación ejecutable.**  
**Mantenimiento:** [@evynaranjo](https://github.com/evynaranjo) · **Licencia:** [MIT](LICENCE)

## Contenido

- [Descripción](#descripción)
- [Objetivos](#objetivos)
- [Características actuales](#características-actuales)
- [Estructura del repositorio](#estructura-del-repositorio)
- [Herramientas utilizadas](#herramientas-utilizadas)
- [Requisitos e instalación](#requisitos-e-instalación)
- [Cómo trabajar en el proyecto](#cómo-trabajar-en-el-proyecto)
- [Integración continua](#integración-continua)
- [Próximos pasos](#próximos-pasos)
- [Contribuciones y soporte](#contribuciones-y-soporte)
- [Autoría y licencia](#autoría-y-licencia)

## Descripción

**MyProyectoDevOps** es una práctica de documentación y organización de un repositorio de desarrollo. Su estructura separa las responsabilidades de backend, frontend, base de datos, documentación, recursos gráficos y automatizaciones.

El proyecto sirve como punto de partida para aprender a documentar el trabajo de forma profesional y utilizar un flujo básico de Git y GitHub. No se ha definido todavía un lenguaje, framework ni motor de base de datos para construir una aplicación.

## Objetivos

- Mantener una estructura de carpetas clara y escalable.
- Documentar la finalidad y el uso del repositorio con Markdown.
- Aplicar buenas prácticas de control de versiones mediante Git.
- Distinguir los archivos que deben y no deben publicarse utilizando `.gitignore`.
- Introducir comprobaciones automáticas con GitHub Actions.

## Características actuales

| Elemento | Función | Estado |
| --- | --- | --- |
| `README.md` | Documentación inicial y guía de uso | Disponible |
| `LICENCE` | Texto de la licencia MIT | Disponible |
| `.gitignore` | Exclusión de archivos temporales, secretos locales y dependencias generadas | Disponible |
| Carpetas organizadas | Separación de componentes del proyecto | Disponible |
| GitHub Actions | Comprobación de la estructura del repositorio | Configurado |
| Backend y frontend funcionales | Aplicación de ejemplo | Pendiente |

## Estructura del repositorio

```text
MyProyectoDevOps/
├── backend/                       # Lógica y servicios del servidor
│   └── .gitkeep
├── frontend/                      # Interfaz de usuario
│   └── .gitkeep
├── database/                      # Scripts y recursos de base de datos
│   └── .gitkeep
├── docs/                          # Documentación complementaria
│   └── .gitkeep
├── images/                        # Imágenes y recursos visuales
│   └── .gitkeep
├── .github/
│   └── workflows/
│       └── verificar-estructura.yml  # Validación automática
├── README.md                      # Guía principal
├── LICENCE                        # Licencia MIT
└── .gitignore                     # Reglas de exclusión de Git
```

> **Nota:** los archivos `.gitkeep` permiten mantener visibles carpetas todavía vacías; `.gitkeep` es una convención de uso, no una función especial de Git.

## Herramientas utilizadas

| Herramienta | Propósito |
| --- | --- |
| **Git** | Registrar y consultar cambios en los archivos. |
| **GitHub** | Alojar y compartir el repositorio. |
| **GitHub Actions** | Ejecutar validaciones automáticas. |
| **Markdown** | Redactar la documentación del proyecto. |
| **Visual Studio Code (opcional)** | Editar archivos localmente. |

Los directorios `backend/`, `frontend/` y `database/` todavía no tienen tecnologías de implementación asignadas.

## Requisitos e instalación

Para obtener una copia local por línea de comandos necesitas **Git** instalado y acceso a Internet. Para editar el proyecto puedes usar cualquier editor de código.

**1. Clonar el repositorio**

```bash
git clone https://github.com/evynaranjo/MyProyectoDevOps.git
```

**2. Entrar a la carpeta del proyecto**

```bash
cd MyProyectoDevOps
```

**3. Abrir el proyecto (opcional, con Visual Studio Code)**

```bash
code .
```

También puedes descargar los archivos desde GitHub usando **Code → Download ZIP**, sin instalar Git.

## Cómo trabajar en el proyecto

Coloca los archivos de cada componente en la carpeta que corresponda. Por ejemplo, el código del servidor debe ir en `backend/` y los documentos técnicos en `docs/`.

Para registrar y publicar tus cambios desde una copia local:

```bash
git status
git add .
git commit -m "docs: actualizar documentacion del proyecto"
git push origin main
```

Antes de confirmar cambios, revisa [`.gitignore`](.gitignore) y evita subir contraseñas, tokens, archivos `.env` o datos personales.

## Integración continua

El flujo [**Verificar estructura**](.github/workflows/verificar-estructura.yml) está configurado para ejecutarse ante eventos `push` y `pull_request`. Utiliza GitHub Actions para comprobar que existen las carpetas y los archivos principales del proyecto.

Puedes revisar sus ejecuciones en la pestaña [**Actions**](https://github.com/evynaranjo/MyProyectoDevOps/actions). Este flujo **no compila ni prueba una aplicación**, ya que todavía no se ha desarrollado el backend o frontend.

## Próximos pasos

- [x] Crear el repositorio y su estructura inicial.
- [x] Añadir README, licencia y `.gitignore`.
- [x] Configurar una validación estructural con GitHub Actions.
- [ ] Elegir tecnologías para frontend, backend y base de datos.
- [ ] Incorporar una aplicación mínima funcional.
- [ ] Añadir pruebas y automatizar su ejecución.
- [ ] Ampliar la documentación técnica en `docs/`.

## Contribuciones y soporte

Si deseas proponer una mejora, abre un [**Issue**](https://github.com/evynaranjo/MyProyectoDevOps/issues) describiendo el objetivo y los pasos para reproducir un problema, si corresponde. Para colaborar con cambios de código, puedes crear una rama y proponer un *pull request*.

Este es un repositorio académico en etapa inicial: las sugerencias deben ser coherentes con sus objetivos de aprendizaje.

## Autoría y licencia

**Responsable:** Evelyn Naranjo · [Perfil de GitHub](https://github.com/evynaranjo).

El proyecto contiene una licencia **MIT**. Consulta las condiciones en el archivo [`LICENCE`](LICENCE).

## Referencias

- [GitHub Docs: Acerca del archivo README del repositorio](https://docs.github.com/es/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- [GitHub Docs: Sintaxis básica de Markdown](https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [Open Source Guides: Comenzando un proyecto de código abierto](https://opensource.guide/es/starting-a-project/)
