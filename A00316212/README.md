# Taller 1

**Nombre:** Jhon Eduar Tobar Gómez  
**Código:** A00316212

## Descripción

Corta descripcion de lo ralizado en el taller.

## Soluciones

### 1.

| Directorio   | Archivo ejemplo | Descripción del contenido del directorio  |
|------|------|------|
|/bin|cd|Almacena la mayoría de los programas esenciales del sistema.|
|/boot|config-3.10.0-514-26-2-el7-x86_64|Archivos estáticos utilizados por el cargador de arranque(boot-loader) del sistema.|
|/dev|zero: es un archivo especial que provee tantos caracteres null| Contiene archivos especiales del sistema, conocidos como controladores de dispositivo (device drivers), los cuales se usan para acceder a los dispositivos del sistema y recursos, como discos duros, modems, memoria, etc.|
|/etc|passwd: Contiene información sobre los usuarios, como login, nombre y otra información que el administrador quiera agregar.|Este directorio está reservado para los ficheros de configuración y arranque del sistema Linux. En este directorio no debe aparecer ningún fichero binario (programas).|
|/home |...|Contiene los directorios personales (casas) de los usuarios. En un sistema recién instalado, no habrá ningún usuario en este directorio.|
|/lib |...|Estos ficheros contienen código que compartirán muchos programas. En lugar de que cada programa contenga una copia propia de las rutinas compartidas, éstas son guardadas en este fichero. Esto hace que los programas ejecutables sean menores y reduce el espacio usado en disco.|
|/mnt |...|Punto de mon taje. Montar temporalmente otros sistemas de archivos.|
|/opt |...|Proporciona una ubicación donde instalar aplicaciones opcionales (de terceros)|
|/proc|kcore|Contiene Archivos especiales que o bien reciben o envían información al kernel del sistema. Información asociada con el núcleo que se está ejecutando, para obtener información de recursos utilizados en el sistema (CPU, memoria, swap, dispositivos..) Este directorio es un sistema de archivo virtual, es decir, no existe físicamente en el disco duro, sólo en memoria.|
|/media|...|Generalmente aquí es donde se montan las unidades de CD, DVD, discos duros y SticksUSB.|
|/root|anaconda-ks.cfg|Directorio hogar (casa) del administrador del sistema.|
|/sbin|nameif|Contiene programas esenciales del sistema, que son únicamente accesibles al administrador (root).|
|/tmp|yum.log|Archivos temporales del sistema.|
|/srv |...|Puede contener archivos que se sirven a otros sistemas|
|/sys |...|Archivos del sistema (system)|
|/usr |doc: Documentación general del sistema.|Éste es uno de los directorios más importantes del sistema puesto que contiene los datos, programas y librerías de uso común para todos los usuarios|
|/var |lock: Archivos para bloqueos.|Este directorio contiene información temporal de los programas (lo cual no implica que se pueda borrar su contenido)|

### 2.

 Comando   | Usuario | Descripción   |
|------|------|------|
| mv nombre_archivo nueva_ruta | root | Permite cortar el archivo hacia una nueve ruta del sistema.|
| reboot | root | permite reiniciar el sistema. |
|find / -name archivo|root|permite buscar un archivo especifico desde la raíz del sistema GNU/Linux.|
|tar -cxvf archivo.tar.tgz|user|permite empaquetar y comprimir un archivo.|
|uptime|user|permite mostrar el tiempo de funcionamiento, número de usuarios conectados, la carga media y  la hora del sistema.|
|kill nombre_proceso|user|permite matar un proceso del sistema|
|shutdown -h Hora|root|permite apagar el sistema a la hora que se indique. Sólo recordar si tú sistema se encuentra en horario militar, es decir, 1:00 PM = 13:00, etc.|
|mkdir -p nombre_directorio|root|permite crear un directorio oculto en el sistema.|
|hostname|user|permite conocer información del equipo anfitrión.|
|chkconfig|user|permite conocer información sobre los niveles de ejecución de los “scripts” ubicados en el directorio /etc/rc.d/init.d|

user: Cualquier usuario.

### 3.

El comando printenv nos permitie visualizar todas las variables de entorno con sus respectivos valores.

Para crear la variable utilizamos el comando export NOMBRE=VALOR. En mi caso hice el siguiente comando:

export VARIABLEOPERATIVOS=CENTOSLIFE



sed '$ a export nombreVariable=valor' /etc/profile  Con este comando la hacemos permanente.




## Referencias

http://docencia.udea.edu.co/cci/linux/dia4/directorio.htm
https://www.enlinux.org/comandos-basicos-en-gnulinux-centos/

