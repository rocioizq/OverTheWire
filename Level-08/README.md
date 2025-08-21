# Bandit Level 8 → 9

## Objetivo
- Procesar un archivo de texto donde algunas líneas están repetidas muchas veces.

- Encontrar la única línea que aparece solo una vez, que normalmente es la contraseña del siguiente nivel..

## Inicio de sesión
Cada nivel requiere iniciar sesión con su usuario correspondiente y el puerto 2220.  
Para este nivel:

```bash
ssh bandit8@bandit.labs.overthewire.org -p 2220
```

## Pasos seguidos
- Listar los archivos de la carpeta con `ls`.
- Ordenar todas las líneas alfabéticamente del archivo data.txt con el comando `sort`.
- Filtrar las líneas que no se repiten con el comando `uniq -u`.
- Se combinan ambos comandos 
```bash
sort data.txt | uniq -u 
```

## Comandos aprendidos
- `sort` → Ordenar líneas de un archivo alfabéticamente o numéricamente.
- `uniq -u` → Mostrar solo las líneas que no se repiten consecutivamente.

