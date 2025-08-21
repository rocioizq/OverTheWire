# Bandit Level 6 → 7

## Objetivo
Este nivel enseña cómo localizar archivos desde el root con propiedades específicas, como usuario, grupo y tamaño.

## Inicio de sesión
Cada nivel requiere iniciar sesión con su usuario correspondiente y el puerto 2220.  
Para este nivel:

```bash
ssh bandit6@bandit.labs.overthewire.org -p 2220
```

## Pasos seguidos
- Buscar el archivo desde el root con el comando:
  ```bash
  find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
  ```
- Leer el contenido del archivo encontrado con el comando:
  ```bash
  cat /var/lib/dpkg/info/bandit7.password
  ```

## Comandos aprendidos
- `find` → Se utiliza para buscar archivos por muchas propiedades: tamaño, tipo, usuario, grupo, permisos, nombre, etc.
- `-type f` → Especifica que solo se buscan archivos (no directorios).
- `-user bandit7` → Buscar archivos que pertenezcan al usuario `bandit7`.
- `-group bandit6` → Buscar archivos que pertenezcan al grupo `bandit6`.
- `-size 33c` → Buscar archivos de **exactamente 33 bytes** (`c` indica bytes).
- `2>/dev/null` → Ignora los mensajes de “Permission denied” para limpiar la salida.

