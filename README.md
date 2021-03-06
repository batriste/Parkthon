# Parkthon

## Guía de instalación

### Linux/MacOS

Abrimos una terminal (Ctrl+T en Linux) y ejecutamos lo siguiente:

#### Con Github

```bash
git clone https://github.com/superpep/Parkthon.git

cd Parkthon

pip3 install -r requirements.txt
```

#### Sin Github

Accederemos a la página [https://github.com/superpep/Parkthon.git](https://github.com/superpep/Parkthon.git) y puslsamos el botón "**Code**" y luego hacemos clic en la opción "**Download ZIP**"\
Una vez descargado, lo extraemos en el escritorio y ahí tendremos el proyecto.\
Ahora sí que neceistaremos acceder a la terminal y ejecutaremos lo siguiente:

```console
cd Desktop

python -m pip install -r Parkthon/requirements.txt
```

En caso de error al ejecutar el último comando, probamos las siguientes alternativas (En cuanto funcione una de ellas, dejamos de probar):

- `$ python3 -m pip install -r requirements.txt`
- `$ pip install -r requirements.txt`
- `$ python -m pip install -r requirements.txt`

Una vez instaladas las dependencias, ejecutaremos el programa de la siguiente forma (Suponiendo que estamos dentro del repositorio clonado):

`$ python3 cli.py`

Y listo.

### Windows

Abrimos una powershell o línea de comandos y ejecutamos lo siguiente (Teniendo en cuenta que ya debemos tener instalado Python3):

#### Con GitHub

```cmd
cd Desktop

git clone https://github.com/superpep/Parkthon.git

python -m pip install -r Parkthon\requirements.txt
```

#### Sin Github

Accederemos a la página [https://github.com/superpep/Parkthon.git](https://github.com/superpep/Parkthon.git) y puslsamos el botón "**Code**" y luego hacemos clic en la opción "**Download ZIP**"\
Una vez descargado, lo extraemos y ahí tendremos el proyecto.\
Ahora sí que neceistaremos acceder a la terminal y ejecutaremos lo siguiente:

```cmd
cd Desktop

python -m pip install -r Parkthon\requirements.txt
```

Abrimos la carpeta de Parkthon que se habrá descargado en nuestro escritorio y hacemos doble click en el archivo `cli.py`

## Dependencias

- PyQt5
- passlib
- stopwatch.py
- pyqtgraph

## Problemas en Windows

Windows tiene un bug con la versión `1.19.4` de `numpy` así que hay que degradarlo. Para ello, abrir una terminal y utilizar el mismo comando para instalar las dependencias que se ha utilizado antes (`pip` o `pip3`) y ejecutar:\
`pip install --upgrade numpy==1.19.3`\
o\
`pip3 install --upgrade numpy==1.19.3`
