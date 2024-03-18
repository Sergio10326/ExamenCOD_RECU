# Release v1.0 - Proyecto ExamenCOD

## Descripción del Proyecto

Este repositorio contiene el código del proyecto ExamenCOD. La URL del proyecto original es: [https://github.com/damiancastelao/ExamenCOD](https://github.com/damiancastelao/ExamenCOD).

Antes de comenzar, asegúrate de hacer un fork del repositorio original para poder trabajar en él.

## Descripción de las Ramas

- **main**: Esta rama solo debe contener commits etiquetados con las diferentes versiones de release.
- **datos**: Contiene la clase de conexión a una base de datos.
- **interface**: Se encarga de la parte gráfica del proyecto.

## Pasos Realizados

### 1. Creación del README

- Se creó una rama `readme` y se añadió el archivo README.md.

### 2. Gestión de Ramas y Commits

- Se hizo un reset en la rama `main` para eliminar el último commit.
- Se realizaron merges squash desde las ramas `datos` e `interface` a la rama `main`.
- Se realizó un commit marcado como v1.0 y se etiquetó con el mismo nombre.

### 3. Revisión del Código en la Rama `interface`

- Se detectó código no deseado en el último commit de la rama `interface`.

### 4. Modificación del Archivo .gitignore

- Se completó y añadió el archivo `.gitignore`.

### 5. Corrección y Push

- Se corrigió el commit etiquetado con v1.0 añadiendo el archivo `.gitignore`.
- Se realizó el push de los cambios y se creó la release v1.0.

## Comandos Realizados

```bash
git clone https://github.com/Sergio10326/ExamenCOD_RECU
cd ExamenCOD_RECU/
git checkout -b readme
sudo touch README.md
git add README.md 
git commit -m "Añadido README.md"
git checkout main
git reset --hard HEAD~1
git merge --squash origin/datos
git merge --squash origin/interface 
git commit -m "v1.0"
git tag -a v1.0 -m "version 1.0"
sudo nano .gitignore
git add .gitignore 
git commit --amend
git push origin v1.0
