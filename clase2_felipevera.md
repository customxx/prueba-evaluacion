1) drwxr-xr-x
r: directorio, dueño lee, escribe y ejecuta; grupo ejecuta y lee; otro lee y ejecuta

2) -rwxr-xr-x
r: archivo, dueño lee, escribe y ejecuta; grupo ejecuta y lee; otro lee y ejecuta

3) dr-xrwx-wx
r: directorio, dueño lee y ejecuta; grupo lee, ejecuta y escribe; otro escribe y ejecuta

4) -rw-rw-rw-
r: archivo, dueño lee y escribe ; grupo escribe y lee; otro lee y escribe

5) -rw-r--r--
r: archivo, dueño lee, escribe ; grupo  lee; otro lee 

6) d-w-rwx-w-
r: directorio, dueño escribe; grupo escribe,ejecuta y lee; otro escribe

7) 414
dueño: 
4: permiso de lectura 
grupo
1: permiso de ejecución. 
otro
4: permiso de lectura 

8) 422
dueño 4: permiso de lectura 
grupo 2: permiso de escritura. 
otro 2: permiso de escritura

9) 303
dueño 3: permiso de escritura y ejecucion
grupo 0: ninguno. 
otro 3: permiso de escritura y ejecucion

10) 404
dueño 4: permiso de lectura 
grupo 0: ninguno 
otro 4: permiso de lectura 

11) 755
dueño 7: todos los permisos 
grupo 5: ejecucion y lectura. 
otro 5: ejecucion y lectura

12) 766
dueño 7: todos los permisos 
grupo 6: lectura y escritura. 
otro 6: lectura y escritura 

13) 711
dueño 7: todos los permisos
grupo 1: permiso de ejecucion. 
otro 1: permiso de ejecucion 

14) 070
dueño 0: ninguno
grupo 7: todos. 
otro 0: ninguno.

20. Crear un archivo
r:felipe@felipe-HP-Notebook:~$ touch nada

21. Quitarle todos los permisos
r:felipe@felipe-HP-Notebook:~$ chmod 000 nada
22. Abrirlo con sublime
r:felipe@felipe-HP-Notebook:~$ subl nada
23. ¿Qué error aparece?
r: no aparece ningun error
24. Dar permisos de lectura al dueño
r:felipe@felipe-HP-Notebook:~$ chmod 400 nada
25. Abrirlo con sublime, modificarlo y guardarlo.
r:felipe@felipe-HP-Notebook:~$ subl nada
26. Dar permisos de escritura
felipe@felipe-HP-Notebook:~$ chmod 222 nada
27. Crea un archivo .txt utilizando sudo
r:felipe@felipe-HP-Notebook:~$ sudo touch texto.txt
28. ¿Qué usuario queda al hacer ls -la ?
r:-rw-r--r--  1 root   root          0 ene 16 17:31 texto.txt
29. Cambia los permisos para que todos puedan escribir en él sin sudo
r:chmod 222 texto.txt
30. ¿Permitido?
r:chmod: cambiando los permisos de 'texto.txt': Operación no permitida
31. Cambia el owner a tu usuario (chown)
r:felipe@felipe-HP-Notebook:~$ sudo chown felipe texto.txt

32. Confirma el cambio con ls -la
r:-rw-r--r--  1 felipe root          0 ene 16 17:31 texto.txt

33. Cambia los permisos para que sólo el usuario pueda leer y escribir
r:chmod 600 texto.txt
34. ¿Permitido?
r: si ..:(

