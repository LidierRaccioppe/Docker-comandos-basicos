# Guia de docker: comandos básicos
1. Para **descargar** una **imagen** se debe de usar `docker pull ubuntu` y para **comprobar** que esta se **encuentre** en el **equipo** se usa `docker images`.

2. Para **crear** un **contenedor** con la imagen que recién descargamos se usa el comando `docker run ubuntu`  , ahora para comprobar si fue todo bien se utiliza ahora `docker ps -a` y así se lista todos los contenedores que estén actualmente, en mi caso tenia el nombre *nostalgic_dijkstra*