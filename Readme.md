# Guia de docker: comandos básicos
1. Para **descargar** una **imagen** se debe de usar `docker pull ubuntu` y para **comprobar** que esta se **encuentre** en el **equipo** se usa `docker images`.

2. Para **crear** un **contenedor** con la imagen que recién descargamos se usa el comando `docker run ubuntu`  , ahora para comprobar si fue todo bien se utiliza ahora `docker ps -a` y así se lista todos los contenedores que estén actualmente, en mi caso tenia el nombre *nostalgic_dijkstra*
   
3. Para **crear** un **contenedor** con la imagen que recién descargamos y asignarle el nombre que queremos y ademas entrar en el se usa el comando `docker run -it --name dam_ubu1 ubuntu`, son los modificadores -it lo que lo permiten

4. Para poder saber la **ip**, se debe **actualizar** los **indices** con `apt update`, y luego usar el `apt install net-tools`  y para **ver la ip** se usa `ifconfig` y vemos el inet, para hacer un ping a google se debe usar el `apt install nslookup` y el `nslookup google.com` y para hacer el ping se usa el `apt install iputils-ping` y luego el nombre del citio o su direcciòn ip.

5. Para poder hacer ping se tiene que instalar otra vez el net tools en el otro contenedor abiendolo creado con `docker run -it --name dam_ubu2 ubuntu`, ahora en el primer contenedor se usa ping a la ip que tenga la otra maquina, y se puede hacer ping entre contenedores
   
6. Usando `exit`, para salir del docker y `docker ps -a` te muestra como quedo el contenedor, en este caso quedo como Exited