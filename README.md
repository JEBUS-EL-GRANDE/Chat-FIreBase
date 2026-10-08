# Chat en tiempo real

### Proyecto compilado
![imagen de mis practicas](readMeIMG/img1.jpeg "imagen de mi mis practicas en postgreSQL")

## Integrantes
proyecto desarrollado por los estudiantes 
  
   -Cordero

   -Pedro

## Informacion directa
- [instalacion Y configuracion en distintos Sistemas](#Instalacion)
- [Configuracion Con el Firebase](#Configuracion2)
- [Uso](#uso)


## Configuracion Con el Firebase <img src="readMeIMG/firebase.svg" width="20" height="20">
ve a la web consolefirebase  y crea un proyecto
- En menu izquierdo> Databases & Storage> Realtime Database> Create Database> next> next
- En menu ezquierdo> security> authentication> next> sing-in method> Email/password> activa el 1er y guarda
- En menu izquierdo> settings> General> App web> (copia todo el const firebaseConfig = {cosas}) y sustituyelo por el que esta en el login.html
- En menu izquierdo> settings> Service accounts> Python> Generate new private key  (sustituye este archivo credenciales.json por lo que tenga el nuevo que se descargo)

-ve a login.html copia el (databaseURL: "link") del const firebaseconfig y pegalo en app.py (linea 11 aprox)

## Instalacion Y configuracion local en diferentes Sistemas Operativos

<span style="color: white">instalacion en windows</span><img src="readMeIMG/windows.png" width="20" height="20">

```bash
   venv\Scripts\activate
```
### Instala las dependencias requeridas:
```bash
   - **pip install -r requirements.txt
```
### inicia servidor Flask:
```bash
   python app.py
```
<span style="color: white">instalacion en Arch linux</span><img src="readMeIMG/arch.png" width="20" height="20">

```bash
sudo pacman -S python python-pip
```
### Dependencias del proyecto
```bash
pip install -r requirements.txt
```
### Entorno virtual
```bash
python -m venv venv
source venv/bin/activate
```
### Ejecutar
```bash
python app.py
```

<span style="color: yellow" style="font-size: 100px">instalacion en Debian</span><img src="readMeIMG/debian.png" width="20" height="20">

```bash
sudo apt update
sudo apt install python3 python3-pip python3-venv
```
### Dependencias del proyecto
```bash
pip install -r requirements.txt
```
### Entorno virtual
```bash
python3 -m venv venv
source venv/bin/activate
```
### Ejecutar
```bash
python app.py
```
