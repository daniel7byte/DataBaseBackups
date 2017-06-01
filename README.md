# DataBaseBackups
Backups de bases de datos MySQL programadas

## Archivos
Cuando hagas `$ git clone https://github.com/daniel7byte/DataBaseBackups.git`, encontrarás los siguientes archivos:

- :package: DatabaseBackups.exe
- :page_facing_up: config_database.txt
- :page_facing_up: config_database_login.txt
- :page_facing_up: config_path_mysqldump.txt
- :open_file_folder: BuckupsProgramados
  - :page_facing_up: readme.txt

## Instalación:
Para que el programa funcione correctamente debes seguir los siguientes pasos.

1. Descarga el repositorio, o ejecuta `$ git clone https://github.com/daniel7byte/DataBaseBackups.git` en tu consola
2. Copia la carpeta `DataBaseBackups` en la particion `D:\`, quedando así: `D:\DataBaseBackups\`

## Configuración:
Despues de habér copiado la carpeta, deben configurar los archivos

### `config_database.txt`
Este archivo contiene el nombre de las bases de datos a las cuales se les realizará las copias de seguridad.
Este tiene la siguiente sitaxis:
```
baseDeDatos1, baseDeDatos2, baseDeDatos3
```
Donde baseDeDatos**N**, corresponde a el nombre de una base de datos
y las **,** (comas) cumplen el papel de separadores

### `config_database_login.txt`
Este archivo es muy importante porque en él debes configurar los datos del usuario que realizará los backups.
Tiene la siguiente sitaxis:
```
usuario:contrasenia
```
Donde usuario y contraseña corresponde a los datos de inicio de sesion

### `config_path_mysqldump.txt`
Este archivo debe contener en su interior la ruta del archivo `mysqldump.exe` que por lo general en XAMPP se encuentra en: `"C:\xampp\mysql\bin\mysqldump.exe"`.
**Muy Importante!** La ruta debe tener la siguente sitaxis `"ruta"` con las **"comillas"**
