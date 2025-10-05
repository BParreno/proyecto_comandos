# Informe - Práctica No 1: Comandos de Linux

## 1. Introducción
**Objetivo:** El objetivo de esta práctica fue familiarizarse con los comandos fundamentales del sistema operativo Linux para la gestión del sistema de archivos. Se cubrió la creación, manipulación, redirección y eliminación de directorios y archivos, utilizando el entorno de línea de comandos de **Git Bash**.

## 2. Desarrollo de la Práctica (Comandos Utilizados)
Se ejecutaron los siguientes comandos en secuencia. El registro completo de los comandos (incluidos los errores de prueba) se encuentra en el archivo de historial adjunto.

### 2.1 Creación de Estructura de Carpetas
| Tarea | Comando(s) | Función |
| :--- | :--- | :--- |
| Creación de Estructura | `mkdir proyecto_comandos`, `cd proyecto_comandos` | Creación del directorio principal y navegación a este. |
| Subcarpetas | `mkdir documentos`, `mkdir imagenes`, `mkdir scripts` | Creación de los tres subdirectorios requeridos. |

### 2.2 Manipulación de Archivos
| Tarea | Comando(s) | Función |
| :--- | :--- | :--- |
| Creación y Contenido | `cd documentos` | Navega al directorio de trabajo para archivos de texto. |
| | `echo "Primera linea de la tarea autónoma." > notas.txt` | Crea `notas.txt` y escribe la primera línea. |
| | `echo "Segunda linea para cumplir con el requisito." >> notas.txt` | Añade la segunda línea de texto. |
| | `echo "Tercera linea sobre los comandos básicos." >> notas.txt` | Añade la tercera línea de texto. |
| Copia y Renombre | `cp notas.txt ../scripts/backup_notas.txt` | Copia el archivo `notas.txt` al directorio `scripts` renombrándolo. |
| Mover Archivo | `mv ../scripts/backup_notas.txt ../imagenes/` | Mueve el archivo a la carpeta `imagenes`. |
| Regreso a Principal | `cd ..` | Vuelve al directorio raíz del proyecto (`proyecto_comandos`). |

### 2.3 Redirección y Concatenación
| Tarea | Comando(s) | Función |
| :--- | :--- | :--- |
| Creación de `resumen.txt` | `touch documentos/resumen.txt` | Crea el archivo de destino. |
| Redirección (Sobrescribir) | `cat documentos/notas.txt > documentos/resumen.txt` | Vuelca el contenido de `notas.txt` a `resumen.txt`. |
| Concatenación (Añadir) | `echo "Este texto se añade al final de resumen.txt." >> documentos/resumen.txt` | Añade una línea adicional sin sobrescribir el contenido previo. |

### 2.4 Eliminación de Archivos y Carpetas
| Tarea | Comando(s) | Función |
| :--- | :--- | :--- |
| Eliminación de Archivo | `rm imagenes/backup_notas.txt` | Elimina el archivo `backup_notas.txt`. |
| Eliminación de Directorio | `rmdir imagenes` | Elimina el directorio `imagenes`, al estar vacío. |
| Volcado de Historial | `history > tarea-s1-BRYAN_PARRENO.txt` | Genera el archivo final de entrega con el historial de comandos. |

## 3. Conclusiones y Aprendizaje
La práctica demostró la funcionalidad y la sintaxis básica de los comandos de Linux, confirmando que herramientas como **`mkdir`**, **`cp`**, **`mv`**, **`rm`**, y el uso eficiente de los operadores de redirección **`>`** y **`>>`** son esenciales para la administración de archivos en la línea de comandos.

## 4. Entrega
Los siguientes tres archivos se adjuntan al repositorio de GitHub:
1.  `informe.md` (Este documento).
2.  `tarea-s1-BRYAN_PARRENO.txt` (Volcado del historial de comandos).
3.  `audio_reflexion.mp3` (Archivo de audio de 60 segundos con la reflexión solicitada).