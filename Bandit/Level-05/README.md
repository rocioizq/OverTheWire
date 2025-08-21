# Bandit Level 5 → 6

## Objetivo
- Este nivel enseña cómo localizar archivos desde el root con propiedades específicas, como usuario, grupo y tamaño.

## Inicio de sesión
Cada nivel requiere iniciar sesión con su usuario correspondiente y el puerto 2220.  
Para este nivel:

```bash
ssh bandit5@bandit.labs.overthewire.org -p 2220
```

## Pasos seguidos
- Buscar archivo desde el root con el comando:
 ```bash
    find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
```
- Leer el archivo que nos entrega utilizando el comando:
```bash
cat /var/lib/dpkg/info/bandit7.password
```

## Comandos aprendidos
- `find` Se utiliza para buscar archivos por muchas propiedades, como tamaño, tipo, permisos, nombre, etc. 
- `-type f` Especifica que solo busca archivos (no directorios), `f` hace referencia `file`.
- `-size 33c` Hace refencia al tamaño exacto del archivo, (`c` hace referencia a los `bytes` que tiene de tamaño).
- `2>/dev/null` Ignora los mensajes de "Permission denied" para que la búsqueda sea más limpia.

