# Copilacion de funciones en matematicas financieras 

En este repositorio, se agrupan las funciones y actividades informaticas realizadas en la materia de matematicas financieras de la licenciatura de Actuaria y Ciencias de Datos de la UMSNH

## Funciones de interes simple

Con el siguiente codigo, puede usted cargar las funciones relativas a los calculos de interes simple:

```{r}
source("https://raw.githubusercontent.com/Yuval-Reyes/MateFinancieras2024/refs/heads/main/formulasInteresSimple.R")
```
A continuacion se dan ejemplos del uso de las formulas correspondientes
###Calculo del valor futuro


para ilustrar el ejemplo se tiene el siguiente ejercicio:
$VA$=$1,000.00
$i$=24% anualizado
$r$=2.00% mensual
$t$=7 meses

Se realizan los calculos:
```(r)
#creamos objetos con valores de entrada:
valorActual=1000
tasaPeriodo=0.02
nPeriodos=7
#Calculamos el valor futuro
valorFuturo=valorfinalsimple(VA=valorActual,r=tasaPeriodo,t=nPeriodos)
#Imprimimos el resultado
valorFuturo
```
