# Bandit Level 9 → 10

## Objetivo
- Procesar un archivo binario para extraer la información legible por humanos.
- Filtrar la línea que contiene la contraseña, identificada porque comienza con varios `=`.


## Inicio de sesión
Cada nivel requiere iniciar sesión con su usuario correspondiente y el puerto 2220.  
Para este nivel:

```bash
ssh bandit9@bandit.labs.overthewire.org -p 2220
```

## Pasos seguidos
- Extraer todo el texto legible por humanos del archivo data.txt con el comando:
```bash
strings data.txt
```
- Filtrar la línea que contiene la contraseña, que empieza con =: 
```bash
grep "="
```

La combinación de ambos comandos quedaría así:
```bash
strings data.txt | grep "="
```

## Comandos aprendidos
- `strings` → Extrae todas las secuencias de caracteres legibles por humanos de un archivo binario
- `grep "="` → Filtra las líneas que comienzan con =.
- `|` → Permite combinar comandos, usando la salida de strings como entrada de grep.


