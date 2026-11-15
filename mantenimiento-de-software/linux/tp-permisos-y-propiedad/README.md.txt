1. Lectura e Interpretación de Permisos (ls -l)



Posición

Representación

Significado / Permiso

Tipo

- / d / l

Indica si es un archivo normal, directorio o enlace simbólico.

Propietario (u)

rwx

Representa los permisos de lectura, escritura y ejecución del propietario.

Grupo (g)

rwx

Representa los permisos de los usuarios pertenecientes al grupo del archivo.

Otros (o)

rwx

Representa los permisos de los demás usuarios del sistema.

Los caracteres r, w y x representan lectura, escritura y ejecución, respectivamente. Cuando aparece un guion (-), significa que ese permiso no está habilitado.

2. Permisos en Modo Octal



Desglose numérico 640:

Propietario: 4 + 2 = 6 (lectura y escritura).

Grupo: 4 (lectura).

Otros: 0 (sin permisos).

Desglose numérico 755:

Propietario: 4 + 2 + 1 = 7 (lectura, escritura y ejecución).

Grupo: 4 + 1 = 5 (lectura y ejecución).

Otros: 4 + 1 = 5 (lectura y ejecución).

3. Modo Simbólico



Ventaja del modo simbólico:

La principal ventaja es que permite modificar permisos específicos sin reemplazar los demás. Por ejemplo, con chmod go-x se quita únicamente el permiso de ejecución al grupo y a otros, manteniendo los permisos restantes.

4. Cambio de Propietario y Grupo



¿Por qué se requiere privilegio de superusuario para chown?

Porque cambiar el propietario de un archivo modifica la propiedad de un recurso del sistema. Esta operación requiere permisos administrativos, por lo que se utiliza sudo o se ejecuta como usuario root.

5. Permisos Recursivos en Directorios



Importancia del permiso x en un directorio:

El permiso de ejecución permite acceder y recorrer un directorio. Si se quita este permiso, los usuarios afectados no podrán ingresar ni acceder normalmente a los archivos que contiene.

La opción -R del comando chmod permite aplicar los permisos de manera recursiva al directorio principal, sus subdirectorios y los archivos contenidos en ellos.
