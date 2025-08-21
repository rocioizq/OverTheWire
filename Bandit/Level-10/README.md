# Bandit Level 9 → 10

## Objetivo
- Decodificar un archivo que está codificado en Base64 para obtener la contraseña del siguiente nivel.


## Inicio de sesión
Cada nivel requiere iniciar sesión con su usuario correspondiente y el puerto 2220.  
Para este nivel:

```bash
ssh bandit10@bandit.labs.overthewire.org -p 2220
```

## Pasos seguidos
- Decodificar el archivo `data.txt` con el comando:
```bash
base64 -d data.txt
```

## Comandos aprendidos
- `base64 -d archivo` → Decodifica un archivo que está codificado en Base64.


