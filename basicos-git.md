# Basicos de Git

## Que es Git

Git es un sistema de control de versiones. Lo creo Linus Torvalds en 2005 (el mismo que hizo Linux). Sirve para guardar el historial de cambios de un proyecto, asi puedes volver a una version anterior si algo se rompe, y tambien para que varias personas trabajen en el mismo proyecto sin pisarse.

Git y GitHub no son lo mismo: Git es el programa que se instala en el ordenador, y GitHub es una pagina web donde se suben los repositorios de Git para compartirlos.

## Conceptos

- **Repositorio**: la carpeta del proyecto con todo el historial de cambios.
- **Commit**: una "foto" de los cambios en un momento. Cada commit tiene un mensaje.
- **Rama (branch)**: una linea de trabajo separada. La principal se llama main. Sirve para trabajar en algo sin tocar lo que ya funciona.
- **Merge**: juntar los cambios de una rama en otra.
- **Remote**: el repositorio que esta en el servidor (GitHub).
- **Clone**: descargar un repositorio a tu ordenador.

## Comandos mas usados

| Comando | Que hace |
|---|---|
| `git init` | Crea un repositorio nuevo en la carpeta |
| `git clone url` | Descarga un repositorio de GitHub |
| `git status` | Muestra que archivos han cambiado |
| `git add archivo` | Añade el archivo al staging (preparado para el commit). Con `git add .` se añaden todos |
| `git commit -m "mensaje"` | Guarda los cambios con un mensaje |
| `git push` | Sube los commits a GitHub |
| `git pull` | Baja los cambios que hay en GitHub |
| `git branch` | Muestra las ramas |
| `git checkout -b nombre` | Crea una rama y se cambia a ella |
| `git merge rama` | Junta una rama con la actual |
| `git log` | Muestra el historial de commits |

## Flujo normal de trabajo

1. `git pull` para tener lo ultimo
2. Hacer los cambios
3. `git add .`
4. `git commit -m "lo que he hecho"`
5. `git push`
