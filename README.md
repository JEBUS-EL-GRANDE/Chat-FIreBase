# Chat en tiempo real

### Proyecto compilado
![video de proyecto ya compilado](readMeIMG/compilado.gif "video de mi proyecto ya compilado")

## Informacion directa
- [Instalacion](#Instalacion)
- [Configuracion con el Firebase](#Configuracion2)
- [Inte](#grupoIntegrande)


<h2 id="grupoIntegrande">Proyecto desarrollado por los estudiantes: </h2>
   -Cordero

   -Pedro

<h2 id="Configuracion2">Configuración Con el Firebase: <img src="readMeIMG/firebase.svg" width="20" height="20"></h2> 

ve a la web consolefirebase  y crea un proyecto
- En menu izquierdo> Databases & Storage> Realtime Database> Create Database> next> next
- En menu ezquierdo> security> authentication> next> sing-in method> Email/password> activa el 1er y guarda
- En menu izquierdo> settings> General> App web> (copia todo el const firebaseConfig = {cosas}) y sustituyelo por el que esta en el login.html
- En menu izquierdo> settings> Service accounts> Python> Generate new private key  (sustituye este archivo credenciales.json por lo que tenga el nuevo que se descargo)

- ve a login.html copia el (databaseURL: "link") del const firebaseconfig y pegalo en app.py (linea 11 aprox)

<h2 id="Instalacion">Instalación Y Configuración local en diferentes Sistemas Operativos:</h2>

<h3  style="color: blue; font-size: 50px">Instalación en Windows: <img src="readMeIMG/windows.svg" width="20" height="20"></h3> 

```bash
   pip install -r requirements.txt                          #Instala las dependencias requeridas
   venv\Scripts\activate

   python app.py                                            #Inicia servidor Flask:
```
<h3>instalacion en Arch linux: <img src="readMeIMG/arch-linux.svg" width="20" height="20"></h3>

```bash
sudo pacman -Syu
sudo pacman -S python python-pip
pip install -r requirements.txt                             # Dependencias del proyecto
python -m venv venv                                         # Entorno virtual
source venv/bin/activate

python app.py                                               # Ejecutar
```

<h3> Instalacion en debian: <img src="readMeIMG/debian.svg" width="20" height="20"></h3>

```bash
sudo apt update
sudo apt install python3 python3-pip python3-venv
pip install -r requirements.txt                             # Dependencias del proyecto
python3 -m venv venv                                        # Entorno virtual
source venv/bin/activate

python app.py                                               # Ejecutar
```