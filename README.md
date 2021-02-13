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
| `sudo <comando a escalar>` | Ejecuta un comando con permisos de superusuario. | `sudo rm -rf /etc/ulacit` eliminaría un directorio llamado ulacit y todos los elementos que contiene. |
| `apt <acción> <paquetes>` | Comando para manejar paquetes a través del gestor de paquetes APT. Algunas acciones podrían ser `install`, `upgrade`, `remove`, `search`, `prune`, etc. Necesita permisos de superusuario.  | `apt install apache2 mysql-server php7` instalaría los cuatro paquetes que conforman el famoso stack XAMP. Instalaría Apache, MySQL y PHP7. |
| `lsb_release` | Muestra la versión de la distribución actual. | `lsb_release -a` muestra toda la información de la distribución de Ubuntu que se usa actualmente.
| `uname` | Muestra la versión del kernel de Linux que se está usando. | `uname -a` muestra la información (gracias al flag `-a`) sobre el kernel actual. |
| `top` | Lista todos los procesos que se están ejecutando en la máquina junto a información de ellos, como el PID. | `top` muestra todos los procesos que están corriendo en el equipo. |
| `history` | Muestra el historial de todos los comandos que se han introducido y ejecutado en la terminal. | `history` muestra una lista de comandos, como `top`, `uname`, `lsb_release` en orden de ejecución. |
