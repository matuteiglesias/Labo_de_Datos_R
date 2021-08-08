# Laboratorio de Datos (en R)

Material para la materia Laboratorio de Datos, Fac. Cs. Exactas de la UBA. 

## Instalacion

Para instalacion de R seguir instrucciones en https://cloud.r-project.org/

### En Ubuntu linux

#### Instalar Rstudio

Luego de instalar R, instalar rstudio. Bajar el binary de http://www.rstudio.com/download y correr:

`sudo dpkg -i rstudio-1.4.1717-amd64.deb`

Si falla con error del tipo: 

```
...
dpkg: dependency problems prevent configuration of rstudio:
 rstudio depends on libclang-dev; however:
  Package libclang-dev is not installed.
 rstudio depends on libpq5; however:
  Package libpq5 is not installed.
...
  ```
  
correr: `$ sudo apt --fix-broken install`

#### Instalar Packages

Si bien se podrian instalar desde la consola de Rstudio, pueden haber problemas. Es recomendable tener anaconda instalado, y crear un environment de R.

`conda create -n myenv r`

luego activarlo

`$ conda activate myenv`

deberia estar actualizado

`$ conda update --all`

y aca se pueden instalar los modulos sin problemas

`$ conda install r-tidyverse`

y podemos ir al directorio de nuestra eleccion y abrir rstudio:

`$ rstudio`

