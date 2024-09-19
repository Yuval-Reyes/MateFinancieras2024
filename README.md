# Copilacion de funciones en matematicas financieras 

En este repositorio, se agrupan las funciones y actividades informaticas realizadas en la materia de matematicas financieras de la licenciatura de Actuaria y Ciencias de Datos de la UMSNH

## Funciones de interes simple

Con el siguiente codigo, puede usted cargar las funciones relativas a los calculos de interes simple:

```{r}
source("https://raw.githubusercontent.com/Yuval-Reyes/MateFinancieras2024/refs/heads/main/VF%20(1)")
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


###Calculo del valor Actual


para ilustrar el ejemplo se tiene el siguiente ejercicio:
$VF$=$1,140.00
$i$=24% anualizado
$r$=2.00% mensual
$t$=7 meses

Se realizan los calculos:
```(r)
#creamos objetos con valores de entrada:
valorFinal=1140
tasaPeriodo=0.02
nPeriodos=7
#Calculamos el valor futuro
valorActual=VA(VF=valorFinal,r=tasaPeriodo,t=nPeriodos)
#Imprimimos el resultado
valorActual
```


###Calculo de la tasa de interes mensual


para ilustrar el ejemplo se tiene el siguiente ejercicio:
$VA$=$1,000.00
$VF$=1140
$r$=20.00%
$t$=7 meses

Se realizan los calculos:
```(r)
#creamos objetos con valores de entrada:
VA=1,000.00
valorFinal=1140
nPeriodos=7
#Calculamos el valor futuro
interes=r(VA=valorActual,VF=valorFinal,t=nPeriodos)
#Imprimimos el resultado
interes
```


###Calculo del tiempo


para ilustrar el ejemplo se tiene el siguiente ejercicio:
$VA$=$1,000.00
$VF$=1140
$r$=2.00% mensual
$i$=24% anualizado

Se realizan los calculos:
```(r)
#creamos objetos con valores de entrada:
VA=$1,000.00
tasaPeriodo=0.02
valorFinal=1140
#Calculamos el valor futuro
tiempo=t(VA=valorActual,r=tasaPeriodo,VF=valorFinal)
#Imprimimos el resultado
tiempo
```
