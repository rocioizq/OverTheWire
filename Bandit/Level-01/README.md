# Bandit Level 1 → 2

## Objetivo
Aprender a leer un archivo cuyo nombre comienza con un guion (-).

## Inicio de sesión
Cada nivel requiere iniciar sesión con su usuario correspondiente y el puerto 2220.  
Para este nivel:

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

## Pasos seguidos
- Listar archivos de la carpeta actual con el comando `ls`.  
- Leer el contenido del archivo utilizando `cat ./-`, ya que al usar `cat -` el sistema lo interpreta como una opción en lugar de un archivo.

## Comandos aprendidos
- `cat ./-` → Permite abrir archivos que comienzan con guion, evitando que se confundan con opciones del comando.
- `./` → Significa “en el directorio actual” y se usa para referirse a archivos que están en el mismo directorio desde donde estás ejecutando el comando.

## Notas y observaciones  
- Este nivel enseña cómo manejar archivos con nombres poco comunes.
- La contraseña para el siguiente nivel se obtiene leyendo el archivo `-`.
