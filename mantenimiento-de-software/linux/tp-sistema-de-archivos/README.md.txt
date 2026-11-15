## 1. Estructura del Árbol de Directorios

![Listado de la raíz](assets/01_raiz_ls.png)

| Directorio | Función según la guía |
| :--- | :--- |
| `/etc` | Contiene archivos de configuración del sistema y de los programas. |
| `/home` | Almacena las carpetas y archivos personales de los usuarios. |
| `/dev` | Contiene archivos especiales que representan dispositivos de hardware y virtuales. |
| `/var` | Almacena datos variables como registros (logs), cachés y otros archivos del sistema. |

---

## 2. Sensibilidad a Mayúsculas y Minúsculas

![Case Sensitivity](assets/02_case_sensitivity.png)

**Respuesta:**

Linux distingue entre mayúsculas y minúsculas en los nombres de archivos. Por eso, `Ejercicio.txt` y `ejercicio.txt` son considerados dos archivos diferentes y pueden existir en una misma carpeta. Esto se debe a que los sistemas de archivos utilizados habitualmente por Linux, como ext4, son sensibles a las mayúsculas y minúsculas. En Windows, en cambio, el comportamiento habitual es no distinguirlas.

---

## 3. Visualización y Gestión de Archivos Ocultos

![Archivos ocultos](assets/03_archivos_ocultos.png)

**Respuesta:**

Los archivos ocultos sirven principalmente para almacenar configuraciones y preferencias del usuario y de diferentes programas. Permiten mantener organizada la carpeta personal, evitando que los archivos de configuración aparezcan junto con los documentos habituales. Se identifican porque sus nombres comienzan con un punto. No significa que estén protegidos o sean inaccesibles.

---

## 4. Buenas Prácticas en Nombres de Archivos

![Creación de directorio](assets/04_creacion_directorio.png)

**Respuesta:**

El nombre `tp_sistema_ficheros_2026` cumple con las recomendaciones porque utiliza letras minúsculas, números y guiones bajos, sin espacios ni caracteres especiales. Esto facilita su utilización desde la terminal y evita problemas al ejecutar comandos.

En cambio, `TP Sistema de Ficheros (Año 2026)!.doc` contiene espacios, mayúsculas, paréntesis, una letra con tilde y un signo de exclamación. Estos caracteres pueden requerir un tratamiento especial al trabajar con archivos desde la terminal.

---

## 5. Exploración de Dispositivos y Procesos

![Directorios proc y dev](assets/05_proc_dev.png)

**Respuesta:**

El directorio `/proc` es un sistema de archivos virtual que almacena información sobre los procesos que se están ejecutando y el estado del sistema operativo. Permite consultar datos como los identificadores de procesos, el uso de memoria y la información del procesador. Sus archivos no son archivos convencionales almacenados en el disco, sino información generada dinámicamente por el kernel de Linux.
