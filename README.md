# Machine Learning Courses - Github Template

![example workflow](https://github.com/fralfaro/mlcourses_gh_template/actions/workflows/documentation.yml/badge.svg)
<a href="https://fralfaro.github.io/mlcourses_gh_template/"><img alt="Link a la Documentación" src="https://img.shields.io/badge/docs-link-brightgreen"></a>


Cursos de Machine Learning generados de manera automática 
con [Google Colab](https://colab.research.google.com/?hl=en), [Mkdocs](https://www.mkdocs.org/) y [Github Actions](https://github.com/features/actions) mediante **Github Template**.


## Descripción del Repositorio

```
|
+---.github
|   \---workflows
|           documentation.yml
|
\---docs
|   |   index.md
|   |   __init__.py
|   |
|   +---homeworks
|   |       add_homework.txt
|   |
|   +---images
|   |       logo.bmp
|   |
|   +---labs
|   |       add_lab.txt
|   |
|   \---lectures
|           colab.ipynb
|           jupyter.ipynb
|           python.ipynb
|           
|   .gitignore
|   LICENSE
|   mkdocs.yml
|   poetry.lock
|   pyproject.toml
|   README.md
```

donde:

* ` documentation.yml`: archivo para generar el CI del proyecto.
* `homeworks`: carpeta donde se almacenan las tareas (opcional)
* `labs`: carpeta donde se almacenan los laboratorios (opcional)
* `homeworks`: carpeta donde se almacenan las tareas (opcional)
* `lectures`: carpeta donde estan los archivos `.ipynb` que queremos documentar.
* `.gitignore`: lugar donde se define los archivos a ignorar.
* `LICENSE`: licencia asociada al proyecto.
* `mkdocs.yml`: archivo que orquestará la documentación del proyecto.
* `poetry.lock`: archivo que orquestará el proyecto y sus dependencias.
* `pyproject.toml`: archivo que orquestará el proyecto y sus dependencias.
* `pyproject.toml`: archivo que contiene  información necesaria para que los desarrolladores comiencen a hacer contribuciones en el proyecto.

## Archivos a modificar

### Readme.md

```
![example workflow](https://github.com/fralfaro/mlcourses_gh_template/actions/workflows/documentation.yml/badge.svg)
<a href="https://fralfaro.github.io/mlcourses_gh_template/"><img alt="Link a la Documentación" src="https://img.shields.io/badge/docs-link-brightgreen"></a>
```

Debe cambiar:

* **fralfaro**: nombre de usuario en github.
* **mlcourses_gh_template**: nombre del proyecto asignado.

### `mkdocs.yml`

**Sección**: Project information - Repository

```
# Project information
site_name: Home
site_url: https://github.com/fralfaro/mlcourses_gh_template 
site_author: Francisco Alfaro  
site_description:  

# Repository
repo_name: fralfaro/mlcourses_gh_template  
repo_url: https://github.com/fralfaro/mlcourses_gh_template  
edit_uri: ''
```

Debe cambiar:

* **fralfaro**: nombre de usuario en github.
* **mlcourses_gh_template**: nombre del proyecto asignado.
* **site_author**: Nombre del autor

**Sección**: Customization

```
# Customization
extra:
  social:
    - icon: fontawesome/brands/github
      link: https://github.com/fralfaro
    - icon: fontawesome/brands/gitlab
      link: https://gitlab.com/fralfaro
    - icon: fontawesome/brands/linkedin
      link: https://www.linkedin.com/in/faam/
    - icon: fontawesome/brands/kaggle
      link: https://www.kaggle.com/faamds
    - icon: fontawesome/brands/medium
      link: https://medium.com/@fralfaro
```
En esta sección se agregan las redes sociales 
que ustedes maneja (más detalles, 
ver el siguiente [link](https://squidfunk.github.io/mkdocs-material/reference/icons-emojis/#with-animations)).

**Sección**: TOC

```
# TOC 
nav:
    - Home: index.md
    - Introducción:
        - Python: lectures/python.ipynb
        - Jupyter Notebook: lectures/jupyter.ipynb
        - Google Colab: lectures/colab.ipynb
```

En esta sección se agregan los archivos `.ipynb` que necesita agregar a su documentación.

### Otros

#### `pyproject.toml`

```
[tool.poetry]
name = "docs"
version = "0.1.0"
description = "mkdocs - courses"
authors = ["Francisco Alfaro <francisco.alfaro.496@gmail.com>"]
license = "MIT"
readme = "README.md"
```

Cambiar `authors` por su nombre y correo personal.

#### `index.md`

```
# Home
![example workflow](https://github.com/fralfaro/mlcourses_gh_template/actions/workflows/documentation.yml/badge.svg)
<a href="https://fralfaro.github.io/mlcourses_gh_template/"><img alt="Link a la Documentación" src="https://img.shields.io/badge/docs-link-brightgreen"></a>


Machine Learning Courses - Github Template


## Material

El material está disponible en el siguiente [repositorio](https://github.com/fralfaro/mlcourses_gh_template), para obtener el código de fuente basta con que ejecutes el siguiente comando:

> https://github.com/fralfaro/mlcourses_gh_template


## Contenidos

### Introducción
* Python
* Jupyter Notebook
* Google Colab
```

Debe cambiar:

* **fralfaro**: nombre de usuario en github.
* **mlcourses_gh_template**: nombre del proyecto asignado.

#### Carpetas `homeworks` y `labs` 

En esta sección puede agregar las tareas y laboratorios asociados al curso que realizará (opcional).

> **Nota**: Si necesita customizar su repositorio, se recomienda leer el siguiente [link](https://squidfunk.github.io/mkdocs-material/).

