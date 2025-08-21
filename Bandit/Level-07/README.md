# Bandit Level 7 → 8

## Objetivo
Este nivel enseña cómo buscar dentro de archivos por contenido específico.

## Inicio de sesión
Cada nivel requiere iniciar sesión con su usuario correspondiente y el puerto 2220.  
Para este nivel:

```bash
ssh bandit7@bandit.labs.overthewire.org -p 2220
```

## Pasos seguidos
- Buscar la línea que contiene la palabra clave `millionth` con el comando:
  ```bash
  grep "millionth" data.txt
  ```

## Comandos aprendidos
- `grep` Se utiliza para buscar líneas que coincidan con un patrón o palabra clave dentro de uno o varios archivos. En este caso se busca una palabra específica dentro del archivo `data.txt`.

