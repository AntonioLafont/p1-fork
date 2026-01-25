# Práctica 1

Un repositorio para empezar a usar [git](https://git-scm.com/) y Github

## ¿Como probar en la nube?

[Github-Codespaces](https://github.com/features/codespaces)

## Comandos git básicos

```
git clone https://github.com/gitt-3-pat/p1
git status
git add .
git commit -m "TU MENSAJE"
git push

git checkout -b feature/1
git checkout main
```

## ¿Cómo escribir un README.md con formato?

[Github Markdown](https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)


## Resumen comandos

 

Git clone crea una copia de un repositorio remoto en nuestro ordenador. Lo utilizamos para trabajar en un proyecto ya existente. 
 

Git status muestra el estado del repositorio local.  Nos informa sobre en que rama nos encontramos, que archivos han sido alterados, que archivos están listos para commit (han sido añadidos/están en staging), y que archivos estan “untracked” (no seguidos por git). Lo utilizamos para evitar errores antes de hacer un commit, como podría ser no añadir todos los archivos deseados. 


Git add añade cambios al git para que estén preparados para el siguiente commit, es decir, los pasa a staging. Añadiendo “.” estamos indicando que queremos añadir todo el contenido de la carpeta en la que nos encontramos. Como git no guarda los cambios automáticamente, tenemos que utilizar git add . para indicar cuales queremos guardar antes de hacer commit. 

 
 Git commit sirve para guardar una nueva versión del proyecto con todos los cambios que estaban en staging. -m “texto” añade el mensaje que hayamos escrito entre comillas. Este mensaje debería de ser una explicación breve de los cambios añadidos en el commit. Utilizamos los commits para tener un registro ordenado de las versiones del proyecto, facilitando enormemente regresar a versiones anteriores, trabajar con otras personas, y tener documentado en qué momento se añadió cada cambio. 

  
Git push envía todos los commits hechos en local al repositorio remoto. Lo utilizamos para que el resto del equipo con el que trabajamos tenga acceso a nuestras versiones. Añadiendo origin main aclaramos en que repositorio y rama queremos que se suban los cambios, pero si no lo añadimos los commits se mandan a la rama y repositorio usados por defecto. Normalmente estos también son origin y main, y ambos comandos tienen el mismo efecto. 


Git checkout cambia de rama. -b feature/1 crea una rama nueva con el nombre de “feature/1”, así que el comando entero crea una nueva rama y nos cambia a ella. Trabajar con ramas nos permite añadir cambios sin alterar la rama principal, una buena práctica para no causar problemas al resto del equipo. 

Git checkout main nos devuelve a la rama principal. 
