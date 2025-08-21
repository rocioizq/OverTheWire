# Bandit Level 11 → 12

## Objetivo
- Encontrar la contraseña que se ecuentra en el archivo `data.txt` donde todas las letras minúsculas y mayúsculas se giraron en 13 posiciones.


## Inicio de sesión
Cada nivel requiere iniciar sesión con su usuario correspondiente y el puerto 2220.  
Para este nivel:

```bash
ssh bandit11@bandit.labs.overthewire.org -p 2220
```

## Pasos seguidos
- Decodificar el archivo `data.txt` con el texto cifrado ROT13 con el comando:
```bash
cat data.txt | tr "A-Za-z" "N-ZA-Mn-za-m"
```

## Comandos aprendidos
- `tr` → Mapea posición por posición: el primer carácter del primer conjunto se convierte en el primer del segundo conjunto, el segundo en el segundo, y así sucesivamente.


