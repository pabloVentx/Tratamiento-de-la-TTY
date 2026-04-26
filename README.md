# Tratamiento-de-la-TTY
Secuencia de comandos a ejecutar para cuando recibamos una shell victima a través de una reverse shell, podamos tener una shell totalmente interactiva sin corrupciones de por medio.

Lo que nos va a permitir esto: <b>Poder limpiar la consolo(CTRL + L), ver el historial de comandos mediante las teclas "flechas direccionales" y tratar con la edición de ficheros mediante editores sin que se corrompan.</b>

<hr>
Comandos que hay seguir en orden para conseguir una shell estable:<br>
<br>
1.<b>script /dev/null -c bash</b>b>
<br>
2.<b>CTRL + Z</b>b>
<br>
3.<b>stty raw -echo; fg</b>b>
<br>
4.<b>reset xterm</b>b>
<br>
5.<b>export TERM=xterm</b>b>
<br>
6.<b>export SHELL=bash</b>b>
