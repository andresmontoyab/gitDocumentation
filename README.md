# Github

Git es una herramienta que nos permite una adecuada gestion de versionamiento.

### Index

* [Conceptos](#Conceptos)
	* [Repositorio](#Repositorio)
	* [Commit](#Commit)
	* [Stagging](#Stagging)
	* [Branch](#Branch)
* [Comandos](#Comandos)
* [Primer Commit](#Primer-Commit)
* [Buenas Practicas](#Buenas-Practicas)

# Conceptos

## Repositorio

Es el directorio del proyecto donde estan todos los archivos y todas sus versiones historicas.

## Commit

Es la accion con la cual se persisten los cambios en la computadora.

## Copia Local.

Es la copia que tenemos en nuestras computadores sobre todos los archivos que trabajamos,
todos los cambios generados se realizan localmente pueden persistirse en un commmit o ignorarse.

## Stagging

Es como un area de carga donde se decide que va guardarse en el proximo commit y que se ignora,
se puede usar para agregar cambios que ya estan listos para guardar.

## Branch

Son ramas que nos permiten trabajar en paralelo, se crean con base a otra rama, o por default a la rama
principal que es "master".


## Comandos

1. git init // Inicializar git en nuestro directorio.
	
2. git status // Permite ver el estado de la copia local.
	
3. git add <name_archivo> // se agrega los archivos especificados a el area de staggin.
	
4. git commit -m "Message" // Realizar un commit. 
	
5. git log 		// Muestra la historia de comandos realizados
	
6. git log --oneline // mismo git log pero con diferente formato.
	
7. git log -p // Se muestra los diferentes commit realizados y con los cambios por archivo.
	
8. git log -- <name_file> // Se ven los commits que modificaron este archivo.
	
9. git diff 	// Nos muestra los cambios que tuvieron cada uno de los archivos.
	
10. git checkout // Deshace los cambios para un archivo o si usamos . para todos los archivos modificados.
	
11. git checkout <number_commit> // Actualizamos nuestro repo local a una version anterior.
	
12. git checkout master // Volver a la cabeza o ultimo commit.
	
13. git branch <name_new_branch> // Crea una nueva rama con base en la rama master.
	
14. git checkout <name_branch> // Cambia de rama
	
15. git merge <branch_to_merge> // Comando usado par unir ramas, se unira la rama donde estoy parado con la rama especificada, ademas git merge combina informacion de merges realizados en una sola accion.
	
16. git branch -d <branch_name> // Eliminar una rama.
	
17. git clone <url> 	// Copia el repositorio central a un repositorio local.
	
18. git pull			// Bajar cambios del repositorio central.
	
19. git push 			// Subir cambios al repositorio central.
	
20. git remote add origin <url> // Conectarse a un repositorio ya creado en github.

21. git rebase <brach_name> 	// Git se fija en las dos ramas, en la actual y en "brach_name", git checkea ambas ramas y se fija en el ultimo commit que ambas ramas tienen en comun y actualiza la rama actual con los commits pendientes de "brach_name". !! DO not rebase commit that exist outside your repository.
	
	
## Primer Commit

1. git init

2. git add README.md

3. git commit -m "first Commit"

4. git remote add origin url

5. git push -u origin master

## Buenas Practicas

1. Hacer commits Periodicos
2. Son mas faciles de revertir.
3. Son más faciles de hacer tracking sobre un cambio.
4. Escribir buenas descripciones.



