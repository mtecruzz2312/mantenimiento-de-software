1. Creación de Grupos y Usuarios



Explicación del parámetro -m:

El parámetro -m del comando useradd permite crear automáticamente el directorio personal del usuario. Si se omite, la cuenta se crea sin generar dicho directorio, aunque se haya establecido una ruta con -d.

2. Gestión de Grupos Secundarios



Comando para quitar un usuario de un grupo:

Se utiliza sudo deluser usuario grupo, que permite eliminar la pertenencia de un usuario a un grupo secundario sin eliminar su cuenta.

3. Modificación de Usuarios



Diferencia entre useradd y usermod:

El comando useradd permite crear nuevas cuentas de usuario, mientras que usermod se utiliza para modificar los parámetros y características de cuentas existentes.

4. Ficheros de Configuración



Fichero

Contenido / Función

/etc/passwd

Almacena información de los usuarios, como nombre, UID, GID, directorio personal y shell.

/etc/group

Almacena información de los grupos del sistema y los usuarios que pertenecen a ellos.

/etc/shadow

Almacena información protegida sobre las contraseñas de los usuarios, sus hashes y vencimientos.

5. Eliminación de Usuarios y Grupos



Uso del parámetro -r en userdel:

El parámetro -r permite eliminar la cuenta del usuario junto con su directorio personal y los archivos asociados.

Condición para borrar un grupo con groupdel:

Para eliminar un grupo, este no debe ser el grupo principal de ningún usuario existente en el sistema.