# Bandit Level 4 → 5

## Objetivo
Aprender a manejar archivos ocultos en Linux y navegar dentro de subdirectorios para encontrarlos.

## Inicio de sesión
Cada nivel requiere iniciar sesión con su usuario correspondiente y el puerto 2220.  
Para este nivel:

```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
```

## Pasos seguidos
- Listar archivos de la carpeta actual con el comando `ls`.  
- Entrar en el archivo `inhere` con el comando `cd inhere`.
- Listar todos los archivos incluso los escondidos con el comando `ls -a`.
- Buscar archivos legibles para los humanos con el comando `file ./*`.
- Leer el archivo de tipo `ASCII text` llamado `./-file07` con el comando `cat ./-file07`.

## Comandos aprendidos
- `file ./*` → Detectar el tipo de cada archivo en el directorio actual. 
    - Examina el contenido de cada archivo y muestra su tipo real.
    - Puede identificar si un archivo es: texto plano, ejecutable, binario, comprimido, imagen, etc.

## Notas y observaciones  
- Este nivel enseña cómo manejar archivos por su tipo.
