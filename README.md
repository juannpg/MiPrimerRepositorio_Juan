# Documentación trabajo git y github RA5
## Por Juan Pasamar - 1º DAW D

### Git

- 1.1. Instalación y configuración de git:

Debido a que ya tengo Git y GitHub configurados en mi dispositivo desde tiempos anteriores, no puedo instalarlo de nuevo.

Hubiera instalado git con:
```bash
choco install git
```
Tras ello, configurado mi usuario con:
```bash
git config --global user.name "FIRST_NAME LAST_NAME"
git config --global user.email "MY_NAME@example.com
```
Y añadido a mi cuenta de GitHub con una clave `SSH`
<img src='https://drive.google.com/uc?export&id=1GSCZk1Q1hX30IVJgl0cY1nCrg3dz073V' alt='captura ejercicio 1.1' width='100%'/>

- 1.2. Documentación:

Este documento.

<hr>

- 2.1. Inicializa un repositorio:

Creo el repositorio y el archivo `README.md` en el que escribo esta documentación.
<img src='https://drive.google.com/uc?export&id=1mfBaGOZdxBn_DaRds_hImlud7pTEv3xY' alt='captura ejercicio 2.1' width='100%'/>

- 2.2. Añadir y confirmar cambios:

Añado y confirmo.
<img src='https://drive.google.com/uc?export&id=1iQBWVRcRgYgyJwfi2AQ6NsHPjYadwpgN' alt='captura ejercicio 2.2' width='100%'/>

- 2.3. Añadir comandos utilizados:
  - `git init` inicia un repositorio en el directorio
  - `git add` añade los archivos especificados a la fase de stage
  - `git commit -m [message]` confirma los cambios en stage con un mensaje
  

### GitHub

- 3.1. Crear un repositorio remoto:

Creo el repositorio en mi perfil.
<img src='https://drive.google.com/uc?export&id=1NQL536nfNOCmh71a8WO0GPn9VyY63DOI' alt='captura ejercicio 3.1' width='100%'/>

- 3.2. Vincular el repositorio local con GitHub.

Copio los últimos dos comandos del repositorio remoto:
<img src='https://drive.google.com/uc?export&id=13p23Tc-KhswZEpxbNP4CunZFje5p-vCG' alt='captura ejercicio 3.2' width='100%'/>

Los pego en el repositorio local:
<img src='https://drive.google.com/uc?export&id=1P3EQc7c7vhRk7J1kdAjiRT_JsA49GVce' alt='captura ejercicio 3.2' width='100%'/>

Compruebo el repositorio remoto:
<img src='https://drive.google.com/uc?export&id=1be-DINnMTwd5gvl95pAE9ASe2Kl1LstX' alt='captura ejercicio 3.2' width='100%'/>

- 3.3. Explicación:

Para vincular un repositorio, debes crear uno nuevo en GitHub. Tras ello, se te proporcionará la clave del repositorio, en mi caso SSH.

Con dicha clave, ejecutas:
```bash
git remote add origin [clave]
```
y, tras añadirlo, haces `push`a main, estableciendo el nombre de la rama principal del repositorio remoto con:
```bash
git push -u origin main
```

### Ramas

- 4.1. Crear y cambiar de rama:

<img src='https://drive.google.com/uc?export&id=1veQqJCIwzwzhWmay5G3tXwh1IF5R9Mf-' alt='captura ejercicio 4.1' width='100%'/>

- 4.2. Cambios en la rama dev:

<img src='https://drive.google.com/uc?export&id=1EH4N-wdSrHQk1CqFcj8amkGGPBjc4KmS' alt='captura ejercicio 4.2' width='100%'/>

- 4.3. Fusionar ramas:

<img src='https://drive.google.com/uc?export&id=1h4ZH92GqBCCJ6Z1JahfgkEyP5pornIEn' alt='captura ejercicio 4.3' width='100%'/>

- 4.4. Explicación:

Para crear una rama utilizamos:
```bash
git branch [nombre_nueva_rama]
```
Esto, crea una nueva rama a partir del estado de la rama de la que partimos.

Para viajar a otra rama, simplemente hacemos:
```bash
git switch [nombre_destino]
```

Si realizamos cambios en ella, podemos luego viajara a otra rama, y traer esos cambios usando:
```bash
git merge [nombre_rama_con_cambios]
```

### Descargar cambios
