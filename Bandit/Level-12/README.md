# Bandit Level 12 → 13

## Objetivo

* Encontrar la contraseña que se encuentra en el archivo `data.txt`, que es un volcado hexadecimal de un archivo comprimido. Será necesario convertirlo a binario y descomprimirlo varias veces hasta obtener la contraseña.

## Inicio de sesión

Cada nivel requiere iniciar sesión con su usuario correspondiente y el puerto 2220. Para este nivel:

```bash
ssh bandit12@bandit.labs.overthewire.org -p 2220
```

## Pasos seguidos

### 1. Crear un directorio temporal seguro para trabajar

```bash
cd /tmp
mktemp -d
cd /tmp/tmp.C8zQssefau
```

### 2. Copiar el archivo `data.txt` al directorio de trabajo

```bash
cp ~/data.txt .
```

### 3. Convertir el volcado hexadecimal a binario

```bash
xxd -r data.txt > data.bin
```

### 4. Determinar el tipo de archivo

```bash
file data.bin
```

Esto indica el tipo de compresión o archivo que tenemos y nos permite decidir cómo descomprimirlo.

### 5. Descomprimir el archivo según su formato

Dependiendo del resultado del comando `file`:

* Si es `gzip`:

```bash
mv data.bin data.gz
gunzip data.gz
```

* Si es `bzip2`:

```bash
mv data.bin data.bz2
bzip2 -d data.bz2
```

* Si es `tar`:

```bash
mv data.bin data.tar
tar -xvf data.tar
```

### 6. Repetir el proceso de descompresión

Cada vez que se genere un nuevo archivo, verificamos nuevamente con:

```bash
file data
```

y descomprimimos según corresponda, hasta llegar a un archivo de texto plano.

### 7. Obtener la contraseña final

Cuando `file` indique que es **ASCII text**:

```bash
cat data
```

El contenido de este archivo es la contraseña para el nivel 13.

## Comandos útiles usados

* `mktemp -d` → crear directorio temporal seguro
* `cp`, `mv` → copiar y renombrar archivos
* `xxd -r` → convertir hexdump a binario
* `file` → identificar tipo de archivo
* `tar`, `gunzip`, `bzip2` → descompresión
* `cat` → mostrar contenido del archivo final
