1. Entrar a la raíz y ver los archivos y directorios
r:felipe@felipe-HP-Notebook:~$ cd /

2. Entrar a la carpeta usuario y ver los archivos y
directorios
r:felipe@felipe-HP-Notebook:~$ ls

3. Ir una carpeta más atrás de la carpeta usuario
r:felipe@felipe-HP-Notebook:~$ cd ..

4. Entrar a la carpeta de escritorio
r:felipe@felipe-HP-Notebook:~$ cd Escritorio

5. Crear una carpeta clase1 dentro del escritorio
r:felipe@felipe-HP-Notebook:~$ cd Escritorio/
felipe@felipe-HP-Notebook:~/Escritorio$ mkdir clase1

6. Entrar a la carpeta
r:felipe@felipe-HP-Notebook:~/Escritorio$ cd clase1

7. Volver atrás
r:felipe@felipe-HP-Notebook:~/Escritorio/clase1$ cd ..

8. Crear una carpeta clase2
r:felipe@felipe-HP-Notebook:~/Escritorio mkdir clase2

9. Mover la carpeta de la clase 2 dentro de la clase1
r:felipe@felipe-HP-Notebook:~/Escritorio mv clase2 clase1

10. Renombrar la carpeta de la clase 2 a estamos_terminando
r:felipe@felipe-HP-Notebook:~/Escritorio mv clase2 estamos_terminando

11. Borrar la carpeta de la estamos_terminando
r:felipe@felipe-HP-Notebook:~/Escritorio/clase1 mr -r estamos_terminando

12. Crear una carpeta llamada recursivo
r:felipe@felipe-HP-Notebook:~$ mkdir recursivo/

13. Crear dentro de la carpeta el archivo mi_documento
felipe@felipe-HP-Notebook:~/recursivo$ touch mi_documento

14. Borrar la carpeta recursivo
felipe@felipe-HP-Notebook:~$ rm recursivo

15. ¿Qué error se obtiene?
r:rm: no se puede borrar 'recursivo': Es un directorio

16. ¿Cómo se puede borrar la carpeta sin tener que borrar primero el
archivo que hay dentro?
r:felipe@felipe-HP-Notebook:~$ rm -r recursivo

