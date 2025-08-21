# Bandit Level 0 → 1

## Objetivo
Aprender a conectarse a un servidor Linux remoto vía SSH y explorar los archivos básicos de una carpeta.

## Inicio de sesión
Cada nivel requiere iniciar sesión con su usuario correspondiente y el puerto 2220.  
Para este nivel:

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
# Contraseña: bandit0
```

## Pasos seguidos
- Listar archivos de la carpeta actual con el comando `ls`.  
- Leer el archivo `readme` encontrado utilizando el comando `cat readme`.

## Comandos aprendidos
- `ssh usuario@host -p puerto` → Conectarse a un servidor remoto vía SSH.  
- `ls` → Listar archivos y carpetas en el directorio actual.  
- `cat archivo` → Mostrar el contenido de un archivo en la terminal.

## Notas y observaciones  
- Este nivel sirve para familiarizarse con la conexión SSH y la navegación básica en Linux.
