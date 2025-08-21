# Bandit Level 3 → 4

## Objetivo
Aprender a manejar archivos ocultos en Linux y navegar dentro de subdirectorios para encontrarlos.

## Inicio de sesión
Cada nivel requiere iniciar sesión con su usuario correspondiente y el puerto 2220.  
Para este nivel:

```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
```

## Pasos seguidos
- Listar archivos de la carpeta actual con el comando `ls`.  
- Entrar en el archivo `inhere` con el comando `cd inhere`.
- Listar todos los archivos incluso los escondidos con el comando `ls -a`.
- Leer el archivo oculto `...Hiding-From-You` con el comando `cat ...Hiding-From-You`.

## Comandos aprendidos
- `ls -a` → Permite ver todos los archivos que contiene el directorio incluso los que están ocultos.
- `cd directorio` → Entrar a un subdirectorio.

## Notas y observaciones  
- Este nivel enseña cómo manejar archivos encondidos.
