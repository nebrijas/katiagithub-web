# ACTIVIDAD DIRIGIDA 2
## En esta actividad, voy a revelar los pasos que he seguido para iniciar mi aprendizaje en git hub:

1. Primero ingresaba al link  https://github.com/nebrijas/katiagithub-web Le daba mi nombre al repositorio que habíamos creado previamentee.
4. Luego seleccionamos en Source en la primera opción que dice: main y en la opción 2: root
5. le damos a crear un  nuevo archivo (con Add file) y a uno le llamamos  ad2.md
7. Descargar Git Bash y abrirlo
8. Escribimos:pwd
y continuamos con enter
9. luego escribimos:
git clone https://github.com/nebrijas/katiagithub-web
con esto, modificamos nuestro repositorio y clonamos  la carpeta e Git hub al ordenador. 
10. Escribimos:
cd katiagithub-web/
y presionamos:
Ahora renombreamos nuestro fichero. 
11. Escribir:
ls
y dar enter para visualizar que archivos hay dentro ze la carpeta
12. Escribir:
git config user.name (seguido de vuestro usuario de GitHub)
y dar enter
13. luego escribí
git config user.email (seguido del correo que utilizáis en GitHub)
y le di enter
14. En el buscador web fui a: https://github.com/settings/tokens
15. luego le di a  "Generate new token" y darle el nombre en Note que queramos. En la expiration elegimos ponerle 60 días. En select scopes seleccionamis "repo" (se activarán todas las de repo) y las demás se dejan sin seleccionar. Y le damos a "Generar token".
16. Copiar el token que se crea (es una cadena de muchos caracteres que os saldrá en pantalla)
16. luego volví a escribir a Git Bash y escribí:
echo "(aquí poner el token previamente)" > ../.token
De este modo se os creará un archivo oculto de nombre .token en el directorio previo.
17. Escribí:
README.md ad1.md
18. Escribí:
nano README.md y cambiñe el archivo poniéndole un título y dos enlaces uno a ad1.md y otro a ad2.md
19. En la parte de abajo aparece una ayuda, por ejemplo para salir le damos siempre CTRL + X y te manda a la página anterior .
20. luego hacemos un:
git status
y damos enter
21. Ahora la nueva carpeta que antes no existía o está modificada aparecerá como sin trackear, pero para añadir online hay que escribir lo siguietne: 
git add ad1.md
y damos enter.
22. Escribimos ahora:
git commit -m "añado ad1.md"
y volvemos a dar enter
23. Escribimos por últumo:
git push
y damos enter otra vez.
24. Ahora nos aseguramos de que la carpeta se encuentre online

## ALGUNOS CONSEJOS: Cuando te aparece este símbolo que no deja avanzar ^, siempre dar a control y puedes continuar.
