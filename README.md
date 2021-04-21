
# Bitácora de comandos de Sistemas Operativos
Bitácora de comandos para la clase de sistemas operativos

| Comando | Descripción | Ejemplo de uso |
|--|--|--|
| `clear` | Limpia la pantalla de la sesión de consola actual. | `clear` muestra toda la información (gracias al flag `-a`) sobre 
| `cd <ruta de directorio>` | Cambia el directorio actual | `cd ~/Ulacit` para ir a una carpeta llamada Ulacit en el home (~) del usuario actual. |
| `ls <directorio>` | Lista los archivos y directorios que están dentro de un directorio. Si no se pasa ningún directorio cómo parámetro se listan los del directorio actual. | `ls ~/Ulacit` para mostrar todas las carpetas y archivos dentro de la carpeta Ulacit. |
| `cp <origen> <destino>` | Copia un archivo (o directorio si se usa el flag `-r`) de un origen a un destino. | `cp -r ~/Ulacit/* ~/` para copiar todo el contenido de la carpeta llamada Ulacit al home del usuario actual. |
| `pwd` | Imprime en pantalla la ruta actual del directorio en el que me encuentro. | Si se corre `pwd` dentro de `~/Ulacit` se imprimiría `/home/diego/Ulacit`. |
| `mkdir <ruta del directorio por crear>` | Crea un directorio | `mkdir ~/Ulacit/SO` para hacer un directorio llamado SO dentro del directorio Ulacit. |
| `ip addr` | Muestra la dirección IP y dirección MAC de cada adaptador de red que tiene conectado el equipo. | `mkdir ~/Ulacit/SO` para hacer un directorio llamado SO dentro del directorio Ulacit. |
| `touch <ruta de nuevo archivo>` | Crea un nuevo archivo de texto vacío. | `touch ~/Ulacit/whatever.txt` crearía un archivo de texto vacío llamado whatever.txt dentro de la carpeta Ulacit. |
| `nano <ruta de archivo>` | Editor de texto. | `nano ~/Ulacit/whatever.txt` abriría un el editor de texto Nano con el archivo whatever.txt dentro de la carpeta Ulacit. |
| `cat <ruta de archivo>` | Imprime todo el contenido de un archivo de texto en consola sin tener que abrir un editor de texto. | `cat ~/Ulacit/whatever.txt` imprimiría todo el contenido de whatever.txt. |
| `sudo <comando a escalar>` | Ejecuta un comando con permisos de super usuario. | `sudo rm -rf /etc/ulacit` eliminaría un directorio llamado ulacit y todos los elementos que contiene. |
| `apt <acción> <paquetes>` | Comando para manejar paquetes a través del gestor de paquetes APT. Algunas acciones podrían ser `install`, `upgrade`, `remove`, `search`, `prune`, etc. Necesita permisos de superusuario.  | `apt install apache2 mysql-server php7` instalaría los cuatro paquetes que conforman el famoso stack XAMP. Instalaría Apache, MySQL y PHP7. |
| `lsb_release` | Muestra la versión de la distribución actual. | `lsb_release -a` muestra toda la información de la distribución de Ubuntu que se usa actualmente.
| `uname` | Muestra la versión del kernel de Linux que se está usando. | `uname -a` muestra la información (gracias al flag `-a`) sobre el kernel actual. |
| `top` | Lista todos los procesos que se están ejecutando en la máquina junto a información de ellos, como el PID. | `top` muestra todos los procesos que están corriendo en el equipo. |
| `history` | Muestra el historial de todos los comandos que se han introducido y ejecutado en la terminal. | `history` muestra una lista de comandos, como `top`, `uname`, `lsb_release` en orden de ejecución. |
|`pacman`| Utiliza el gestor de paquetes pacman. Tiene un uso similar al de APT, siendo empleado para administrar paquetes instalados e instalables en un equipo. | `pacman install nginx` instalaría Nginx |
|`ssh`| Empieza una sesión de SSH. SSH es un protocolo de shell segura que le permite al usuario entrar a la terminal de un equipo de manera remota. | `ssh -i identity.pem ubuntu@192.168.0.1` le permitiría acceder al shell una máquina ubicada en 192.168.0.1 |
|`dmidecode`|||
|`free`| `free` permite visualizar el espacio disponible en la memoria RAM y la memoria Swap del equipo | `free -h` mostaría una tabla fácilmente legible con la información del espacio usado y librede los diferentes tipos de memoria. |
|`swapon`| `swapon` permite habilitar dispositivos como memoria Swap, permitiéndole así transferir partes no utilizadas tan recurrentemente de la memoria RAM hacia este espacio, liberando RAM. | `swapon` puede ser utilizado sobre una partición haciendo que el equipo pueda usarla como memoria Swap. |
|`mount`| Monta una partición de disco en un directorio especificado con un tipo de archivos determinado. | `mount -t nfts /dev/dev0 /mnt/midisco` montaría una partición de disco tipo NFTS ubicada en /dev/dev0 en el directorio /mnt/midisco |
|`du`| Permite saber la capacidad en disco utilizada por un dado directorio o archivo. | `du -sh /home` devolvería la capacidad de disco utilizada por el directorio /home |
|`stat`| Devuelve información sobre los metadatos de un archivo, como su tamaño, permisos, quién es el dueño, etc. | `stat index.html` devolvería la información descrita sobre un archivo index.html dado. |
|`file`| Devuelve el tipo y la encodificación que tiene un archivo. | `file index.html` diría que es un documento HTML encodeado en UTF-8 |
|`chown`| Permite cambiar el usuario y el grupo dueño de un archivo o directorio. | `chown -R diego:usuarios /var/micarpeta` haría que todo el directorio /var/micarpeta (de forma recursiva) sea del usuario "diego" y del grupo "usuarios" |
|`chmod`| Permite cambiar los permisos y el modo de ejecución de un archivo dado. | `chmod +x miscript.sh` cambiaría el modo del archivo miscript.sh para que este sea ejecutable. |
|`kill`| Finaliza un proceso que actualmente se ejecuta identificado por su PID (process identifier). | `kill -9 1000` mataría con código de finalización 9 al proceso que tenga el pid 1000 |
|`ps`| Muestra la información de los procesos que actualmente están en ejecución. | `ps -aux` muestra los procesos que están siendo ejecutados agrupados por los usuarios dueños de cada proceso. |
|`su`| Le permite a los usuarios que son parte del grupo sudo abrir una sesión de terminal con el usuario root (tiene los permisos más elevados) | `sudo su` abriría una sesión shell bajo el usuario root |
|`curl`| Es un útil comando principalmente empleado a la hora de querer imprimir en pantalla lo que retorna visitar un endpoint de un API o descargar un archivo desde la terminal. Este comando sirve para enviar y recibir solicitudes de red. | `curl -O https://diegocalme.com/ejemplo.zip` permitiría descargar el archivo ejemplo.zip de diegocalme.com |
|`add-apt-repository`| Añade una nueva fuente de repositorio al gestor de paquetes APT, habilitando así acceder a los paquetes que se encuentran dentro de este repositorio. | `add-apt-repository ppa:ondrej/php` permite añadir un repositorio donde se encuentran las últimas versiones de PHP |
|`usermod`| Permite modificar los ajustes de un usuario. | `usermod -aG sudo diego` permitiría añadir el usuario diego al grupo de superusuarios |
|`yum`| Comando para utilizar el gestor de paquetes Yum. Tiene una funcionalidad muy similar a APT, pacman, Zypper, etc. | `yum install nginx` instalaría el paquete Nginx |
|`echo`| Imprime en pantalla una cadena de texto. | `echo "Hola"` imprimiría Hola en la salida de la terminal. |
