# Bandit Level 2 → 3

## Objetivo
Aprender a manejar archivos con espacios y caracteres especiales en el nombre usando comillas y la ruta relativa.

## Inicio de sesión
Cada nivel requiere iniciar sesión con su usuario correspondiente y el puerto 2220.  
Para este nivel:

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

## Pasos seguidos
- Listar archivos de la carpeta actual con el comando `ls`.  
- Leer el contenido del archivo utilizando `cat ./"--spaces in this filename--"`.

## Comandos aprendidos
- `cat ./"archivo"` → Permite abrir archivos que contienen espacios en el nombre, se utilizan comillas para dicho nombre.

## Notas y observaciones  
- Este nivel enseña cómo manejar archivos con espacios en el nombre.
