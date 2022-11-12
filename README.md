# Prácticas A y B , procedimiento para solucionarlas:
---
1.Crear un directorio y dentro del mismo crear un archivo de texto.

---
2.Damos click derecho y en el menu desplegado seleccionamos _*Git Bash Here*_.

![](capturas/1.png)

---
3.Ejecutamso el comando ```git init```.

![](capturas/2.png)
---
4.Comprobamos el estado del _WorkSpace_ ejecutando el comando ```git status - s``` , donde observamos que nuestro archivo no ha sido indexado,es decir, no tiene seguimiento.

![](capturas/3.png)
---
5.Procedemos a ejecutar el comando ```git add``` seguido del nombre de nuestro archivo o ```git add .``` e indexamos todos los archivos y directorios del _WorkSpace_.

![](capturas/4.png)
---
6.Ejecutamos nuevamente el comando ```git status -s``` y comprobamos que justo al lado de el archivo aparece una _(A)_ de color verde indicando que el archivo se encuentra en _(staged area)_, es decir ,_esta indexado_ listo para formar parte del historial de cambios del proyecto.

![](capturas/5.png)
---
7.Ejecutamos el comando  ```git commit -m "Aqui podemos poner cualquier mensaje"``` eviando nuestro archivo de texo a _(Local Repository)_, es decir, nuestro historial de cambios o podria asociarse tambien con fotos de nuestro codigo.

![](capturas/6.png)
---
8.Si ejecutamos el comando ```git status -s``` esta vez no nos saldra ningun archivo , lo que indica que todos estan en _(Local Repository)_ y desde el ultimo cambio que guardamos,no hubo ninguno mas.

![](capturas/8.png)
---
9.Si deseamos ver el historial de cambios a lo largo del tiempo podemos ejecutar el comando ```git log --oneline```.

![](capturas/9.png)
---
10.Para poder subir dicho archivo a un repositorio externo como __GitHub__ o __GitLab__ debemos previamente crearnos un repositorio en el sitio web [GitHub](https://github.com/) o [GitLab](https://gitlab.com/) usando nuestra cuenta.

---
11.Una vez dentro y con nuestra cuenta creada , damos en el boton de nuevo repositorio.

![](capturas/10.png)

---
12.Le damos un nombre

![](capturas/11.png)

---
13.Damos en el boton crear 


---
14.Copiamos la url del repositorio



---
15.Nos dirigimos a la consola git y ejecutamos el comando ```git remote add origin``` _[url del repositorio](https://github.com/MRodriguezValdes/Ejercicios-A-y-B.git)_

![](capturas/13.png)

---
16.Ejecutamos el comando ```git branch -M main```

![](capturas/14.png)


---
17.Por ultimo ejecutamos el comando ```git push -u origin main```, si es primera vez que ejecutamos este comando en nuestro ordenador , nos solicitara las credenciales de nuestra cuenta en github.

![](capturas/15.png)


---
18.Siguiendo los pasos anteriores ya tendriamos nuestro archivo en git hub 

![](capturas/16.png)


# Git Lab

1.Manteniendo los pasos anteriores ,para subir nuestro archivo a _GitLab_ solo tendriamos que cambiar el repositorio remoto, utilizando el comando ```git remote add gitlab``` seguido del [url del repositorio](https://gitlab.com/MarcosRdguez/ejercicios-a-y-b.git) dode escribo gitlab puedes poner cualqier cosa.

![](capturas/1g.png)

2.Ejecutamos el comando ```git branch -M main```

![](capturas/2g.png)

3.Por ultimo ejecutamos el comando ```git push -u gitlab main```

![](capturas/3g.png)

Con los pasos anteriores tendriamos nuestro archivo en _GitLab_

![](capturas/4g.png)

# Modificaciones:
1.Esta linea ha sido insertada en _GitHub_ y posteriormente haré un ```commint``` de ella para actualizar los cambios en mi repositorio local haciendo uso del comando ```git pull orgin main ```
