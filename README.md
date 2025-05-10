# _*Apunte de clases*_

## *Introduccion a Git*
#### -----------------------------------------------------------------------------------
### Control de versiones
Es el sistema que se encarga de organizar cada version que se va realiza en el codigo principal.
Asi tenemos un historial de todo lo que vamos progresando en el codigo principal.

Esto nos permite tener mejor seguridad y flexibilidad, porque todo lo que hagamos va a ser monitoreado por el control de versiones asi evitamos tener percances con el proyecto.
  
![alt text](https://codideep.com/img/blogpost/imagenportada/201811200000001.png)

#### -----------------------------------------------------------------------------------
### ¿Que es git?
Es un sistema de control de versiones que nos permite tener una conexion remota y local, al tener estas conexiones se debe tener en cada máquina la conexión con el repositorio para tenerlo en la parte local.
Cada máquina que se conecta aloja todos los archivos que tienen el repositorio.
  
 ![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e0/Git-logo.svg/800px-Git-logo.svg.png)

#### -----------------------------------------------------------------------------------
### ¿Que es un repositorio?
Un repositorio es la carpeta donde se va a almacenar todos los ficheros que se vayan creando, aqui tambien se va observando el control de versiones que se realizo a lo largo del proyecto.
Pueden ser tanto locales como remotos, la diferencia es que el local se encuentra alojado en tu computadora y el remoto ya fue subido en nuestro caso al GitHub
![alt text](https://blogs.iadb.org/conocimiento-abierto/wp-content/uploads/sites/10/2014/06/New-Picture.png)

#### -----------------------------------------------------------------------------------
### Instalación del Git

Primero debemos descargar de la pagina web de Git "[text](https://git-scm.com/downloads)" 
Abrimos el archivo descargado y en los primeros paneles debemos poner "Next"
 
![alt text](https://www.mclibre.org/consultar/informatica/img/git/git-instalacion-01.png)
 
Llegamos al panel que preguntara con que editor de codigo queremos utilizar y seleccionamos el editor de nuestra preferencia y que tengamos instalado 
 
![alt text](https://www.solvetic.com/uploads/monthly_11_2021/tutorials-9832-0-34695800-1635843407.png)
 
En nuestro caso utilizaremos Visual Studio Code
En el siguiente panel tendremos dos opciones y seleccionamos el segundo que es el mas actualizado y por defecto en el cuadro de texto tendremos main, si no tuviera ponemos main.
 
En el siguiente panel seleccionamos el que esta recomendado para nosotros 
 
![alt text](https://www.ionos.com/es-us/digitalguide/fileadmin/DigitalGuide/Screenshots_2022/screenshot-of-path-environment-options-during-git-bash-installation.jpg)
 
Luego tenemos un panel que tendremos que elegir para usar bundled SSH
Luego en el siguiente panel seleccionamos openSSL
En el siguiente panel tenemos multiples opciones, si somos windows debemos elegir la opcion de Windows-style. La otra opcion es para sistemas operativos Linux.
 
![alt text](https://kinsta.com/wp-content/uploads/2023/04/line-ending-conversions.png)
 
En el nuevo panel que aparecera tenemos lo que seria MinTTY que es simplemente como vera la terminal de git.
Luego en el siguiente panel tenemos que elegir "fast-forward or merge"
De aqui en adelante simplemente le damos a "next" hasta llegar a "Install"
 
![alt text](https://miro.medium.com/v2/resize:fit:990/1*XYMyRItzk_HQVSoeFXmLkw.png)

### Iniciar un proyecto de Git

Para iniciar un nuevo proyecto debemos tener creado una carpeta en donde se almacenara todos los archivos que subiremos luego a GitHub.
Lo que debemos hacer es con "git init" en el Git bash para ya iniciar el proyecto de ahi debemos empezar creando README.md, que es recomendable para la poner como la sinopsis de lo que trata nuestro proyecto.
         
![alt text](https://media.geeksforgeeks.org/wp-content/uploads/20220915184539/GitInit1.jpg)

#### ***********************************************************************************
## *States y Commits*
### Los 3 estados de Git
    -Modified
    Son los cambios en los archivos que aun no han sido confirmados 
    -Staged
    El archivo ya fue confirmado pero aun no se grabo en el repositorio local
    -Commited
    Los cambios ya fueron aceptados y el archivo se guardo en el repositorio local

![alt text](https://i.ytimg.com/vi/dEBWNvY8dY4/maxresdefault.jpg)

#### -----------------------------------------------------------------------------------
### ¿Que es un commit?
Es el estado actual o en el que se encontro en algun momento un archivo o varios archivos que llega a tener el autor, fecha, localización.
El commit podemos verlo como el punto de guardado que se va almacenando en el repositorio

Se puede realizar de manera muy sencilla, al ser un mensaje de confirmacion podemos hacerlo de varias maneras pero la que a mi gusto es la mejor seria " git commit -m "(Lo que se guardo en el archivo)" "

![alt text](https://i.imgur.com/ogoyi2W.png)

#### -----------------------------------------------------------------------------------
### ¿Que es el HEAD?

Es la ubicacion en donde te encuentras, en otras palabras es la rama donde te encuentras.
Es como el pin que hace referencia a donde te encuentras actualmente el repositorio.

![alt text](https://media.geeksforgeeks.org/wp-content/uploads/20230504180513/git-head-architecture.webp)

#### -----------------------------------------------------------------------------------
### ¿Que es una rama?

Es una version copia de la rama actual, por ejemplo cuando iniciamos un proyecto git, tenemos lo que seria la rama main.
La primera rama que creemos partira de la rama main pero de ahi ya se creara ramas a partir de la nueva rama creada y asi sucesivamente, por eso se llama ramas, ya que todas van enlazadas de una rama principal.

![alt text](https://media.datacamp.com/cms/google/ad_4nxf_maaumizik2_rv90hfm0msw-ugg4h1qqw6ccptxgswvukyg5uvusuw8e71ier7hcxugept-skyaf81nvxocgyfafrfsemrobon-gkpalhosbgbrxtwdple928ngt6tvxrecb9hz7eiwvpb6rh-ifqy18.png)

#### -----------------------------------------------------------------------------------
### ¿Para que sirve una rama?

Para realizar trabajos de manera no lineal, por ejemplo al trabajar en equipo cada uno puede tener su rama y asi al aplicar cambios, no afectar a la rama principal, esto nos permite poder realizar multiples cambios y al final con los diferentes colaboradores unir nuestras partes del proyecto.
![alt text](https://www.unir.net/wp-content/uploads/2023/03/git2.jpg)