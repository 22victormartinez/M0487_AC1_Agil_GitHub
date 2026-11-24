# Pasos para hacer una Pull Request en GitHub

Una Pull Request (PR) es una peticion para que los cambios que has hecho en tu rama se junten (merge) con la rama principal (main). Sirve para que otro compañero revise el codigo antes de meterlo.

## Pasos

### 1. Crear una rama nueva

Desde GitHub, en la pestaña Code, pulsas en el desplegable de ramas (donde pone main), escribes el nombre de la rama nueva y le das a "Create branch". Tambien se puede hacer desde la terminal:

```
git checkout -b rama/nombre-tarea
```

### 2. Hacer los cambios

Creas o editas los archivos que necesites en tu rama.

### 3. Hacer commit

Guardas los cambios con un mensaje que explique que has hecho:

```
git add .
git commit -m "añadida seccion de pull request"
git push origin rama/nombre-tarea
```

Si lo haces desde la web de GitHub, al editar el archivo te sale el boton "Commit changes" y ya escribes el mensaje ahi.

### 4. Abrir la Pull Request

Cuando subes la rama GitHub te muestra un aviso amarillo con el boton "Compare & pull request". Le das y:

- Pones un titulo
- En la descripcion explicas los cambios
- Escribes `Closes #numero` con el numero de la issue para que se cierre sola cuando se haga el merge

Luego le das a "Create pull request".

### 5. Revision

Otro compañero entra en la PR, va a la pestaña "Files changed" y mira los cambios. Puede dejar comentarios en las lineas y despues le da a "Review changes" y "Approve".

Importante: uno no puede aprobar su propia PR.

### 6. Merge

Cuando esta aprobada se le da al boton "Merge pull request" y luego "Confirm merge". Los cambios ya estan en main y la issue se cierra automaticamente. Despues se puede borrar la rama.
