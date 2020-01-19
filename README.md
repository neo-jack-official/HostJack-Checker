![alt text](https://raw.githubusercontent.com/neo-jack-official/HostJack-Checker/master/img/vista01.png)
# hostjack-checker.py - HostJack-Checker herramienta de estado para Host-Web por Neo-Jack ENE/2020

## ¿Qué es HostJack-Checker?
Es una simple herramienta de comprobacion de estado de sitios web.
evita tener que estar corroborando el estado de un sitio miediante un navegador, y cuenta con conexion Tor.
HostJack-Checher es rapido simple y seguro.


## ¿Como funciona?
1. Realiza peticiones al sitio cada 9.5 Segundos.
2. Como respuesta obtendras: Operativo, No Disponible o TImeOUT
3. El tiempo de espera de 9.5 segundos puede ser ampliado en 5 segundos si la respuesta es TimeOUT. y modifica el tiempo de la respuesta segun su lag.
4. Cuenta con acceso a Tor Network mediante el argumento (-T).


## Como Instalar y correr PYTHON?

HostJack-Checker es un archivo con extencion "Py", solo requiere tener pre instalado Python.

## Preparamos la instalacion para python

* `sudo apt-get update`
* `sudo apt-get install build-essential checkinstall`
* `sudo apt-get install libreadline-gplv2-dev libncursesw5-dev libssl-dev libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev`
* `sudo apt-get install python2.7`
* `sudo apt-get install python3.6`

## Revisamos que python esta instalado correctamente

* `python -V | python3 -V`


### Soporte para proxy SOCKS5

Si planea usar la opción `-x` para usar un proxy SOCKS5 para conectarse en lugar de una conexión directa a través de su dirección IP, deberá instalar la biblioteca` PySocks`.
 [`PySocks`] (https://github.com/Anorov/PySocks)
 [` SocksiPy`] (http://socksipy.sourceforge.net/) by GitHub @Anorov y puede ser instalado fácilmente por comando ` pip` 

* `sudo pip3 install PySocks`

Luego puede usar la opción `-x` para activar el soporte SOCKS5 y las opciones` --proxy-host` y `--proxy-port` para especificar el host proxy SOCKS5 y su puerto, si son diferentes del estándar` 127.0.0.1: 8080`.

## Opciones de Configuracion

* `-h = Ayuda`
* `-T = Habilitar el enrutamiento TOR, por defecto: Desactivado`
* `-F = Des-habilitar el enrutamiento TOR`

## Como lo utiliso?

Si `hostjack-checker.py` esta en Escritorio
1) Abra terminal, Escriba `cd Escritorio`
2) Ejecute bajo Python `python hostjack-checker.py www.ejemplo.com`

## Ejemplos de comandos.

  Sin TOR:
* `python hostjack-checker.py www.ejemplo.com`
* `python hostjack-checker.py www.ejemplo.com -F`
  Con TOR:
* `python hostjack-checker.py www.ejemplo.com -T`


