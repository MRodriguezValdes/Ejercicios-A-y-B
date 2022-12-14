# Prácticas A y B , procedimiento para solucionarlas:
---
1.Crear un directorio y dentro del mismo crear un archivo de texto.

---
2.Damos click derecho y en el menú desplegado seleccionamos _*Git Bash Here*_.

![](capturas/1.png)

---
3.Ejecutamos el comando ```git init```.

![](capturas/2.png)
---
4.Comprobamos el estado del _WorkSpace_ ejecutando el comando ```git status - s``` , donde observamos que nuestro archivo no ha sido indexado,es decir, no tiene seguimiento.

![](capturas/3.png)
---
5.Procedemos a ejecutar el comando ```git add``` seguido del nombre de nuestro archivo o ```git add .``` e indexamos todos los archivos y directorios del _WorkSpace_.

![](capturas/4.png)
---
6.Ejecutamos nuevamente el comando ```git status -s``` y comprobamos que justo al lado de el archivo aparece una _(A)_ de color verde indicando que el archivo se encuentra en _(staged area)_, es decir ,_está indexado_ listo para formar parte del historial de cambios del proyecto.

![](capturas/5.png)
---
7.Ejecutamos el comando  ```git commit -m "Aquí podemos poner cualquier mensaje"``` eviando nuestro archivo de texo a _(Local Repository)_, es decir, nuestro historial de cambios o podría asociarse también con fotos de nuestro código.

![](capturas/6.png)
---
8.Si ejecutamos el comando ```git status -s``` esta vez no nos saldrá ningún archivo , lo que indica que todos están en _(Local Repository)_ y desde el último cambio que guardamos,no hubo ninguno más.

![](capturas/8.png)
---
9.Si deseamos ver el historial de cambios a lo largo del tiempo podemos ejecutar el comando ```git log --oneline```.

![](capturas/9.png)
---
10.Para poder subir dicho archivo a un repositorio externo como __GitHub__ o __GitLab__ debemos previamente crearnos un repositorio en el sitio web [GitHub](https://github.com/) o [GitLab](https://gitlab.com/) usando nuestra cuenta.

---
11.Una vez dentro y con nuestra cuenta creada , damos en el botón de nuevo repositorio.

![](capturas/10.png)

---
12.Le damos un nombre.

![](capturas/11.png)

---
13.Damos en el botón crear.


---
14.Copiamos la url del repositorio.



---
15.Nos dirigimos a la consola git y ejecutamos el comando ```git remote add origin``` _[url del repositorio](https://github.com/MRodriguezValdes/Ejercicios-A-y-B.git)_

![](capturas/13.png)

---
16.Ejecutamos el comando ```git branch -M main```

![](capturas/14.png)


---
17.Por último ejecutamos el comando ```git push -u origin main```, si es primera vez que ejecutamos este comando en nuestro ordenador , nos solicitará las credenciales de nuestra cuenta en github.

![](capturas/15.png)


---
18.Siguiendo los pasos anteriores ya tendríamos nuestro archivo en git hub 

![](capturas/16.png)


# Git Lab

1.Manteniendo los pasos anteriores ,para subir nuestro archivo a _GitLab_ solo tendríamos que cambiar el repositorio remoto, utilizando el comando ```git remote add gitlab``` seguido del [url del repositorio](https://gitlab.com/MarcosRdguez/ejercicios-a-y-b.git) donde escribo gitlab puedes poner cualqier cosa.

![](capturas/1g.png)

2.Ejecutamos el comando ```git branch -M main```

![](capturas/2g.png)

3.Por último ejecutamos el comando ```git push -u gitlab main```

![](capturas/3g.png)

Con los pasos anteriores tendríamos nuestro archivo en _GitLab_

![](capturas/4g.png)

# Modificaciones:
1.Esta línea ha sido insertada en _GitHub_ y posteriormente haré un ```commint``` de ella para actualizar los cambios en mi repositorio local haciendo uso del comando ```git pull orgin main ```

![](capturas/1m.png)

![](capturas/2m.png)


![](capturas/3m.png)

2.Si hacemos un cambio en el documento y antes de ejecutar el comando ```git add nombre_del_archivo``` ejecutamos el comando ```git checkout nombre_del_archivo``` todos los cambios se deshacen.

![](capturas/4m.png)

![](capturas/5m.png)

3.Si hacemos un cambio en el documento y luego ejecutamos el comando ```git add nombre_del_documento``` y autoseguido intentamos lo comentado anteriormente ```git checkout nombre_del_archivo``` observamos que no sucede nada porque ya hemos indexado el archivo, es decir , ahora se encuentra en la _(staged area)_ y primero debemos sacarlo de ahí para poder ejecutar el comando anterior , para ello, hacemos uso del comando ```git reset HEAD nombre_del_archivo``` y luego aplicamos el comando ```git checkout nombre_del_archivo``` y observamos que todos los cambios en el documento se deshacen.


![](capturas/6m.png)

4.Para regresar a una versión específica de un archivo de forma temporal ejecutamos el comando ```git checkout hash_del archivo nombre_del_archivo```

- El hash del archivo en sus diferentes versiones podemos buscarlo en:
    
    - _GitHub_:Damos click en el archivo y luego nos dirigimos a _history_,donde encontramos las diferentes versiones del mismo y podemos acceder al hash que deseemos.
    - Ejecutando el comando ```git log -- oneline``` nos sale justo al lado de cada commit.



![](capturas/7m.PNG)


![](capturas/8m.PNG)


![](capturas/9m.PNG)


![](capturas/10m.png)

5.Podemos regresar a una fase del proyecto de forma permanente ejecutando el comando ```git reset --hard hash_del_commit```

![](capturas/11m.png)

6.Si perdemos nuestro proyecto y lo tenemos en github podemos clonarlo al directorio que deseemos haciendo uso del comando ```git clone``` [url del proyecto](https://github.com/MRodriguezValdes/Ejercicios-A-y-B.git)

![](capturas/12m.png)


![](capturas/13m.png)


![](capturas/14m.png)

```Con esto damos por concluidos los Ejercicios```