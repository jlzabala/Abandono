Experimentos No Determinísticos
================

## <span style="color:black">*1. Ejercicios de Experimentos No Determinísticos* </span>

### <span style="color:black">*1.1. Simulaciones* </span>

### En está práctica de simulaciones se utiliza principalmente las siguientes funciones:

- **set.seed**, para fijar una semilla y contar siempre con el mismo
  resultado
- **sample**, en este caso se utiliza para generar una muestra de
  números aleatorios
- **size**, determina el tamaño de la muestra
- **replace**, True si queremos que exista reemplazamiento, caso
  contrario False
- **table**, que crea una tabla de frecuencias
- **freq**, muestra una tabal de frecuencias completa
- **plot**, o hist para graficar
- **cbind**, para unir dos vectores en columnas
- **pnorm**, permite calcular la función de distribución acumulada de la
  distribución normal

Nota: Previamente se deben tener cargadas las librerias que permiten
llamar a las funciones.

### <span style="color:black">*1.1.1 Lanzamiento de moneda 1285 veces* </span>

``` r
set.seed(1234)
resul1 <- sample(c("cara", "sello"),
                 size = 1285, replace=T)
print(resul1)
```

    ##    [1] "sello" "sello" "sello" "sello" "cara"  "sello" "cara"  "cara"  "cara" 
    ##   [10] "sello" "sello" "sello" "sello" "cara"  "sello" "sello" "sello" "cara" 
    ##   [19] "sello" "sello" "sello" "sello" "sello" "sello" "sello" "sello" "cara" 
    ##   [28] "sello" "sello" "sello" "cara"  "sello" "cara"  "cara"  "cara"  "sello"
    ##   [37] "cara"  "sello" "sello" "cara"  "sello" "cara"  "sello" "sello" "sello"
    ##   [46] "cara"  "cara"  "cara"  "cara"  "sello" "sello" "sello" "sello" "sello"
    ##   [55] "cara"  "sello" "cara"  "cara"  "sello" "cara"  "sello" "sello" "cara" 
    ##   [64] "sello" "cara"  "cara"  "sello" "cara"  "cara"  "sello" "sello" "cara" 
    ##   [73] "cara"  "cara"  "sello" "sello" "sello" "cara"  "sello" "cara"  "cara" 
    ##   [82] "sello" "cara"  "sello" "cara"  "sello" "cara"  "sello" "sello" "cara" 
    ##   [91] "cara"  "cara"  "cara"  "sello" "cara"  "sello" "sello" "cara"  "sello"
    ##  [100] "sello" "sello" "cara"  "cara"  "cara"  "cara"  "sello" "cara"  "sello"
    ##  [109] "cara"  "cara"  "cara"  "sello" "sello" "sello" "sello" "cara"  "sello"
    ##  [118] "cara"  "sello" "cara"  "cara"  "sello" "sello" "cara"  "sello" "cara" 
    ##  [127] "sello" "sello" "sello" "sello" "cara"  "cara"  "sello" "cara"  "cara" 
    ##  [136] "sello" "sello" "sello" "sello" "sello" "cara"  "sello" "cara"  "sello"
    ##  [145] "sello" "cara"  "sello" "sello" "cara"  "sello" "sello" "sello" "cara" 
    ##  [154] "cara"  "cara"  "cara"  "sello" "sello" "sello" "cara"  "cara"  "cara" 
    ##  [163] "cara"  "sello" "sello" "sello" "sello" "sello" "cara"  "sello" "sello"
    ##  [172] "cara"  "cara"  "cara"  "cara"  "sello" "sello" "cara"  "sello" "cara" 
    ##  [181] "cara"  "cara"  "cara"  "cara"  "sello" "sello" "cara"  "sello" "cara" 
    ##  [190] "sello" "sello" "sello" "cara"  "sello" "sello" "cara"  "sello" "cara" 
    ##  [199] "cara"  "cara"  "sello" "cara"  "sello" "cara"  "cara"  "cara"  "sello"
    ##  [208] "sello" "sello" "cara"  "sello" "cara"  "sello" "cara"  "cara"  "cara" 
    ##  [217] "sello" "cara"  "cara"  "cara"  "sello" "sello" "sello" "cara"  "cara" 
    ##  [226] "cara"  "cara"  "sello" "cara"  "sello" "sello" "cara"  "cara"  "cara" 
    ##  [235] "cara"  "sello" "cara"  "sello" "sello" "sello" "cara"  "sello" "cara" 
    ##  [244] "cara"  "sello" "cara"  "sello" "cara"  "sello" "sello" "cara"  "cara" 
    ##  [253] "cara"  "cara"  "cara"  "cara"  "sello" "sello" "cara"  "cara"  "sello"
    ##  [262] "sello" "cara"  "sello" "cara"  "sello" "sello" "sello" "sello" "cara" 
    ##  [271] "sello" "sello" "cara"  "sello" "sello" "cara"  "cara"  "sello" "sello"
    ##  [280] "cara"  "cara"  "sello" "sello" "cara"  "cara"  "cara"  "cara"  "cara" 
    ##  [289] "cara"  "sello" "cara"  "sello" "sello" "cara"  "cara"  "sello" "cara" 
    ##  [298] "cara"  "sello" "cara"  "cara"  "cara"  "cara"  "cara"  "sello" "sello"
    ##  [307] "cara"  "cara"  "sello" "sello" "cara"  "cara"  "sello" "sello" "sello"
    ##  [316] "cara"  "cara"  "sello" "sello" "cara"  "cara"  "sello" "sello" "sello"
    ##  [325] "sello" "sello" "cara"  "sello" "sello" "cara"  "cara"  "sello" "cara" 
    ##  [334] "sello" "sello" "cara"  "sello" "sello" "cara"  "cara"  "sello" "sello"
    ##  [343] "cara"  "cara"  "cara"  "cara"  "sello" "sello" "sello" "cara"  "sello"
    ##  [352] "cara"  "cara"  "sello" "sello" "cara"  "cara"  "cara"  "cara"  "sello"
    ##  [361] "cara"  "sello" "sello" "cara"  "sello" "cara"  "sello" "sello" "sello"
    ##  [370] "cara"  "cara"  "cara"  "cara"  "cara"  "sello" "sello" "cara"  "cara" 
    ##  [379] "cara"  "sello" "cara"  "sello" "cara"  "sello" "sello" "cara"  "sello"
    ##  [388] "cara"  "sello" "sello" "sello" "sello" "sello" "cara"  "sello" "sello"
    ##  [397] "sello" "sello" "cara"  "cara"  "sello" "cara"  "cara"  "cara"  "cara" 
    ##  [406] "cara"  "sello" "cara"  "cara"  "sello" "sello" "cara"  "cara"  "sello"
    ##  [415] "cara"  "sello" "sello" "cara"  "cara"  "cara"  "sello" "cara"  "cara" 
    ##  [424] "sello" "cara"  "cara"  "cara"  "sello" "sello" "sello" "cara"  "sello"
    ##  [433] "cara"  "sello" "sello" "cara"  "cara"  "sello" "sello" "cara"  "sello"
    ##  [442] "sello" "sello" "sello" "cara"  "cara"  "cara"  "cara"  "sello" "cara" 
    ##  [451] "cara"  "sello" "cara"  "cara"  "cara"  "sello" "sello" "sello" "sello"
    ##  [460] "cara"  "sello" "sello" "sello" "cara"  "sello" "cara"  "sello" "sello"
    ##  [469] "cara"  "cara"  "sello" "sello" "cara"  "cara"  "sello" "cara"  "sello"
    ##  [478] "sello" "sello" "cara"  "sello" "sello" "cara"  "cara"  "cara"  "sello"
    ##  [487] "cara"  "cara"  "cara"  "cara"  "cara"  "cara"  "sello" "cara"  "sello"
    ##  [496] "cara"  "cara"  "cara"  "sello" "sello" "cara"  "sello" "sello" "sello"
    ##  [505] "sello" "cara"  "sello" "cara"  "cara"  "cara"  "cara"  "sello" "cara" 
    ##  [514] "cara"  "sello" "sello" "sello" "sello" "cara"  "sello" "cara"  "cara" 
    ##  [523] "cara"  "sello" "sello" "cara"  "sello" "sello" "cara"  "cara"  "sello"
    ##  [532] "sello" "sello" "cara"  "cara"  "sello" "sello" "cara"  "cara"  "sello"
    ##  [541] "sello" "cara"  "sello" "cara"  "cara"  "cara"  "cara"  "cara"  "sello"
    ##  [550] "sello" "cara"  "sello" "cara"  "sello" "cara"  "sello" "cara"  "cara" 
    ##  [559] "cara"  "cara"  "sello" "sello" "cara"  "cara"  "sello" "sello" "cara" 
    ##  [568] "sello" "cara"  "sello" "cara"  "cara"  "sello" "cara"  "cara"  "sello"
    ##  [577] "sello" "sello" "cara"  "cara"  "sello" "cara"  "cara"  "cara"  "cara" 
    ##  [586] "sello" "sello" "sello" "cara"  "cara"  "sello" "cara"  "sello" "cara" 
    ##  [595] "sello" "sello" "cara"  "sello" "cara"  "sello" "sello" "sello" "sello"
    ##  [604] "sello" "sello" "sello" "sello" "sello" "sello" "cara"  "cara"  "cara" 
    ##  [613] "sello" "cara"  "cara"  "cara"  "sello" "cara"  "cara"  "sello" "cara" 
    ##  [622] "sello" "cara"  "cara"  "cara"  "cara"  "cara"  "cara"  "cara"  "sello"
    ##  [631] "sello" "cara"  "cara"  "cara"  "cara"  "cara"  "sello" "sello" "sello"
    ##  [640] "cara"  "sello" "cara"  "cara"  "cara"  "sello" "sello" "cara"  "sello"
    ##  [649] "sello" "sello" "cara"  "cara"  "cara"  "sello" "sello" "sello" "sello"
    ##  [658] "cara"  "cara"  "cara"  "sello" "sello" "cara"  "sello" "sello" "sello"
    ##  [667] "cara"  "sello" "cara"  "sello" "sello" "sello" "sello" "cara"  "cara" 
    ##  [676] "cara"  "cara"  "cara"  "cara"  "cara"  "cara"  "sello" "sello" "cara" 
    ##  [685] "cara"  "sello" "sello" "cara"  "sello" "sello" "cara"  "cara"  "cara" 
    ##  [694] "sello" "cara"  "sello" "cara"  "sello" "sello" "sello" "sello" "cara" 
    ##  [703] "sello" "sello" "cara"  "cara"  "sello" "sello" "cara"  "sello" "cara" 
    ##  [712] "sello" "sello" "cara"  "cara"  "cara"  "sello" "cara"  "cara"  "cara" 
    ##  [721] "cara"  "cara"  "sello" "sello" "sello" "cara"  "cara"  "sello" "cara" 
    ##  [730] "sello" "cara"  "cara"  "cara"  "cara"  "cara"  "cara"  "sello" "cara" 
    ##  [739] "cara"  "sello" "cara"  "cara"  "sello" "cara"  "sello" "cara"  "sello"
    ##  [748] "cara"  "sello" "cara"  "cara"  "cara"  "cara"  "sello" "sello" "cara" 
    ##  [757] "cara"  "cara"  "sello" "sello" "sello" "cara"  "cara"  "cara"  "sello"
    ##  [766] "sello" "sello" "cara"  "cara"  "sello" "cara"  "cara"  "cara"  "sello"
    ##  [775] "cara"  "sello" "cara"  "sello" "sello" "cara"  "cara"  "cara"  "cara" 
    ##  [784] "cara"  "cara"  "cara"  "cara"  "sello" "cara"  "sello" "sello" "cara" 
    ##  [793] "sello" "cara"  "cara"  "cara"  "cara"  "cara"  "sello" "sello" "sello"
    ##  [802] "cara"  "sello" "sello" "cara"  "cara"  "sello" "cara"  "sello" "sello"
    ##  [811] "cara"  "cara"  "sello" "sello" "sello" "sello" "sello" "sello" "cara" 
    ##  [820] "cara"  "cara"  "cara"  "sello" "cara"  "cara"  "cara"  "cara"  "sello"
    ##  [829] "sello" "sello" "cara"  "cara"  "sello" "sello" "cara"  "sello" "sello"
    ##  [838] "sello" "cara"  "cara"  "cara"  "cara"  "cara"  "cara"  "sello" "cara" 
    ##  [847] "sello" "cara"  "sello" "cara"  "sello" "sello" "sello" "cara"  "cara" 
    ##  [856] "sello" "cara"  "sello" "cara"  "cara"  "sello" "sello" "cara"  "sello"
    ##  [865] "cara"  "sello" "sello" "sello" "sello" "cara"  "sello" "cara"  "cara" 
    ##  [874] "sello" "sello" "sello" "cara"  "sello" "sello" "cara"  "sello" "cara" 
    ##  [883] "cara"  "cara"  "cara"  "cara"  "sello" "cara"  "cara"  "cara"  "sello"
    ##  [892] "sello" "cara"  "cara"  "sello" "sello" "cara"  "cara"  "cara"  "cara" 
    ##  [901] "cara"  "cara"  "cara"  "cara"  "sello" "sello" "sello" "cara"  "cara" 
    ##  [910] "cara"  "cara"  "sello" "cara"  "cara"  "cara"  "sello" "sello" "cara" 
    ##  [919] "cara"  "sello" "sello" "sello" "cara"  "sello" "cara"  "sello" "sello"
    ##  [928] "cara"  "sello" "sello" "cara"  "sello" "sello" "cara"  "cara"  "sello"
    ##  [937] "cara"  "sello" "cara"  "cara"  "sello" "cara"  "cara"  "sello" "sello"
    ##  [946] "sello" "sello" "cara"  "sello" "sello" "cara"  "sello" "sello" "sello"
    ##  [955] "sello" "cara"  "cara"  "cara"  "cara"  "cara"  "sello" "sello" "cara" 
    ##  [964] "sello" "cara"  "cara"  "sello" "sello" "sello" "cara"  "cara"  "sello"
    ##  [973] "sello" "sello" "cara"  "sello" "cara"  "sello" "sello" "cara"  "sello"
    ##  [982] "cara"  "sello" "sello" "cara"  "cara"  "cara"  "sello" "cara"  "cara" 
    ##  [991] "cara"  "cara"  "cara"  "sello" "sello" "sello" "cara"  "cara"  "cara" 
    ## [1000] "sello" "sello" "cara"  "sello" "cara"  "sello" "sello" "cara"  "cara" 
    ## [1009] "sello" "sello" "sello" "sello" "cara"  "cara"  "cara"  "cara"  "sello"
    ## [1018] "cara"  "sello" "cara"  "cara"  "sello" "cara"  "sello" "sello" "sello"
    ## [1027] "sello" "cara"  "cara"  "cara"  "cara"  "sello" "cara"  "sello" "cara" 
    ## [1036] "cara"  "sello" "cara"  "cara"  "sello" "cara"  "sello" "cara"  "cara" 
    ## [1045] "sello" "cara"  "cara"  "sello" "cara"  "sello" "cara"  "sello" "sello"
    ## [1054] "sello" "cara"  "cara"  "sello" "cara"  "cara"  "sello" "sello" "cara" 
    ## [1063] "sello" "cara"  "sello" "sello" "cara"  "cara"  "cara"  "sello" "sello"
    ## [1072] "cara"  "cara"  "cara"  "cara"  "sello" "cara"  "sello" "cara"  "cara" 
    ## [1081] "cara"  "sello" "sello" "sello" "cara"  "cara"  "cara"  "cara"  "sello"
    ## [1090] "sello" "sello" "cara"  "cara"  "sello" "sello" "cara"  "cara"  "cara" 
    ## [1099] "sello" "cara"  "sello" "sello" "cara"  "sello" "cara"  "cara"  "cara" 
    ## [1108] "cara"  "cara"  "cara"  "sello" "cara"  "cara"  "cara"  "cara"  "sello"
    ## [1117] "sello" "cara"  "cara"  "cara"  "sello" "cara"  "cara"  "sello" "cara" 
    ## [1126] "sello" "cara"  "cara"  "sello" "cara"  "sello" "sello" "cara"  "cara" 
    ## [1135] "sello" "sello" "sello" "sello" "sello" "sello" "sello" "cara"  "cara" 
    ## [1144] "cara"  "cara"  "cara"  "sello" "sello" "cara"  "sello" "sello" "cara" 
    ## [1153] "sello" "cara"  "cara"  "cara"  "sello" "sello" "sello" "sello" "sello"
    ## [1162] "sello" "cara"  "cara"  "cara"  "cara"  "sello" "cara"  "sello" "cara" 
    ## [1171] "sello" "sello" "cara"  "sello" "cara"  "sello" "sello" "sello" "cara" 
    ## [1180] "sello" "sello" "cara"  "cara"  "cara"  "sello" "cara"  "sello" "sello"
    ## [1189] "sello" "sello" "sello" "cara"  "sello" "cara"  "cara"  "sello" "sello"
    ## [1198] "sello" "cara"  "cara"  "sello" "sello" "sello" "sello" "cara"  "cara" 
    ## [1207] "sello" "sello" "sello" "cara"  "cara"  "sello" "sello" "sello" "cara" 
    ## [1216] "sello" "sello" "cara"  "cara"  "sello" "sello" "cara"  "cara"  "cara" 
    ## [1225] "sello" "cara"  "sello" "cara"  "cara"  "sello" "cara"  "sello" "cara" 
    ## [1234] "sello" "sello" "cara"  "sello" "sello" "cara"  "sello" "cara"  "cara" 
    ## [1243] "cara"  "sello" "sello" "sello" "sello" "sello" "sello" "cara"  "sello"
    ## [1252] "cara"  "sello" "sello" "cara"  "cara"  "cara"  "cara"  "cara"  "sello"
    ## [1261] "cara"  "sello" "sello" "sello" "cara"  "cara"  "sello" "sello" "cara" 
    ## [1270] "sello" "sello" "cara"  "sello" "cara"  "sello" "cara"  "cara"  "sello"
    ## [1279] "sello" "sello" "cara"  "sello" "sello" "sello" "sello"

``` r
freq1 <- table(resul1)
freq1
```

    ## resul1
    ##  cara sello 
    ##   655   630

``` r
plot(freq1,main="Gráfico 1: Histograma del experimento lanzamiento de una moneda")
```

![](Experimentos_files/figure-gfm/unnamed-chunk-1-1.png)<!-- -->

``` r
resul2 <- ifelse(resul1=="cara",0,1)
resul2
```

    ##    [1] 1 1 1 1 0 1 0 0 0 1 1 1 1 0 1 1 1 0 1 1 1 1 1 1 1 1 0 1 1 1 0 1 0 0 0 1 0
    ##   [38] 1 1 0 1 0 1 1 1 0 0 0 0 1 1 1 1 1 0 1 0 0 1 0 1 1 0 1 0 0 1 0 0 1 1 0 0 0
    ##   [75] 1 1 1 0 1 0 0 1 0 1 0 1 0 1 1 0 0 0 0 1 0 1 1 0 1 1 1 0 0 0 0 1 0 1 0 0 0
    ##  [112] 1 1 1 1 0 1 0 1 0 0 1 1 0 1 0 1 1 1 1 0 0 1 0 0 1 1 1 1 1 0 1 0 1 1 0 1 1
    ##  [149] 0 1 1 1 0 0 0 0 1 1 1 0 0 0 0 1 1 1 1 1 0 1 1 0 0 0 0 1 1 0 1 0 0 0 0 0 1
    ##  [186] 1 0 1 0 1 1 1 0 1 1 0 1 0 0 0 1 0 1 0 0 0 1 1 1 0 1 0 1 0 0 0 1 0 0 0 1 1
    ##  [223] 1 0 0 0 0 1 0 1 1 0 0 0 0 1 0 1 1 1 0 1 0 0 1 0 1 0 1 1 0 0 0 0 0 0 1 1 0
    ##  [260] 0 1 1 0 1 0 1 1 1 1 0 1 1 0 1 1 0 0 1 1 0 0 1 1 0 0 0 0 0 0 1 0 1 1 0 0 1
    ##  [297] 0 0 1 0 0 0 0 0 1 1 0 0 1 1 0 0 1 1 1 0 0 1 1 0 0 1 1 1 1 1 0 1 1 0 0 1 0
    ##  [334] 1 1 0 1 1 0 0 1 1 0 0 0 0 1 1 1 0 1 0 0 1 1 0 0 0 0 1 0 1 1 0 1 0 1 1 1 0
    ##  [371] 0 0 0 0 1 1 0 0 0 1 0 1 0 1 1 0 1 0 1 1 1 1 1 0 1 1 1 1 0 0 1 0 0 0 0 0 1
    ##  [408] 0 0 1 1 0 0 1 0 1 1 0 0 0 1 0 0 1 0 0 0 1 1 1 0 1 0 1 1 0 0 1 1 0 1 1 1 1
    ##  [445] 0 0 0 0 1 0 0 1 0 0 0 1 1 1 1 0 1 1 1 0 1 0 1 1 0 0 1 1 0 0 1 0 1 1 1 0 1
    ##  [482] 1 0 0 0 1 0 0 0 0 0 0 1 0 1 0 0 0 1 1 0 1 1 1 1 0 1 0 0 0 0 1 0 0 1 1 1 1
    ##  [519] 0 1 0 0 0 1 1 0 1 1 0 0 1 1 1 0 0 1 1 0 0 1 1 0 1 0 0 0 0 0 1 1 0 1 0 1 0
    ##  [556] 1 0 0 0 0 1 1 0 0 1 1 0 1 0 1 0 0 1 0 0 1 1 1 0 0 1 0 0 0 0 1 1 1 0 0 1 0
    ##  [593] 1 0 1 1 0 1 0 1 1 1 1 1 1 1 1 1 1 0 0 0 1 0 0 0 1 0 0 1 0 1 0 0 0 0 0 0 0
    ##  [630] 1 1 0 0 0 0 0 1 1 1 0 1 0 0 0 1 1 0 1 1 1 0 0 0 1 1 1 1 0 0 0 1 1 0 1 1 1
    ##  [667] 0 1 0 1 1 1 1 0 0 0 0 0 0 0 0 1 1 0 0 1 1 0 1 1 0 0 0 1 0 1 0 1 1 1 1 0 1
    ##  [704] 1 0 0 1 1 0 1 0 1 1 0 0 0 1 0 0 0 0 0 1 1 1 0 0 1 0 1 0 0 0 0 0 0 1 0 0 1
    ##  [741] 0 0 1 0 1 0 1 0 1 0 0 0 0 1 1 0 0 0 1 1 1 0 0 0 1 1 1 0 0 1 0 0 0 1 0 1 0
    ##  [778] 1 1 0 0 0 0 0 0 0 0 1 0 1 1 0 1 0 0 0 0 0 1 1 1 0 1 1 0 0 1 0 1 1 0 0 1 1
    ##  [815] 1 1 1 1 0 0 0 0 1 0 0 0 0 1 1 1 0 0 1 1 0 1 1 1 0 0 0 0 0 0 1 0 1 0 1 0 1
    ##  [852] 1 1 0 0 1 0 1 0 0 1 1 0 1 0 1 1 1 1 0 1 0 0 1 1 1 0 1 1 0 1 0 0 0 0 0 1 0
    ##  [889] 0 0 1 1 0 0 1 1 0 0 0 0 0 0 0 0 1 1 1 0 0 0 0 1 0 0 0 1 1 0 0 1 1 1 0 1 0
    ##  [926] 1 1 0 1 1 0 1 1 0 0 1 0 1 0 0 1 0 0 1 1 1 1 0 1 1 0 1 1 1 1 0 0 0 0 0 1 1
    ##  [963] 0 1 0 0 1 1 1 0 0 1 1 1 0 1 0 1 1 0 1 0 1 1 0 0 0 1 0 0 0 0 0 1 1 1 0 0 0
    ## [1000] 1 1 0 1 0 1 1 0 0 1 1 1 1 0 0 0 0 1 0 1 0 0 1 0 1 1 1 1 0 0 0 0 1 0 1 0 0
    ## [1037] 1 0 0 1 0 1 0 0 1 0 0 1 0 1 0 1 1 1 0 0 1 0 0 1 1 0 1 0 1 1 0 0 0 1 1 0 0
    ## [1074] 0 0 1 0 1 0 0 0 1 1 1 0 0 0 0 1 1 1 0 0 1 1 0 0 0 1 0 1 1 0 1 0 0 0 0 0 0
    ## [1111] 1 0 0 0 0 1 1 0 0 0 1 0 0 1 0 1 0 0 1 0 1 1 0 0 1 1 1 1 1 1 1 0 0 0 0 0 1
    ## [1148] 1 0 1 1 0 1 0 0 0 1 1 1 1 1 1 0 0 0 0 1 0 1 0 1 1 0 1 0 1 1 1 0 1 1 0 0 0
    ## [1185] 1 0 1 1 1 1 1 0 1 0 0 1 1 1 0 0 1 1 1 1 0 0 1 1 1 0 0 1 1 1 0 1 1 0 0 1 1
    ## [1222] 0 0 0 1 0 1 0 0 1 0 1 0 1 1 0 1 1 0 1 0 0 0 1 1 1 1 1 1 0 1 0 1 1 0 0 0 0
    ## [1259] 0 1 0 1 1 1 0 0 1 1 0 1 1 0 1 0 1 0 0 1 1 1 0 1 1 1 1

``` r
hist(resul2,main="Gráfico 2: Histograma del experimento lanzamiento de una moneda", 
     ylab="Frecuencias",
     col=c("green","yellow"))
```

![](Experimentos_files/figure-gfm/unnamed-chunk-1-2.png)<!-- -->

``` r
library("descr")
freq2 <- freq(resul1, 
              main = "Gráfico 3: Frecuencias del experimento lanzamiento de una moneda",
              col=c("green","yellow"))
```

![](Experimentos_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->

``` r
freq2
```

    ## resul1 
    ##       Frequency Percent
    ## cara        655   50.97
    ## sello       630   49.03
    ## Total      1285  100.00

``` r
tab <- freq2
dim(tab)
```

    ## [1] 3 2

``` r
fx <- tab[,2]/100
fx
```

    ##      cara     sello     Total 
    ## 0.5097276 0.4902724 1.0000000

``` r
tab <- cbind(tab,fx)
print(tab)
```

    ##       Frequency   Percent        fx
    ## cara        655  50.97276 0.5097276
    ## sello       630  49.02724 0.4902724
    ## Total      1285 100.00000 1.0000000

### <span style="color:black">*1.1.2 Lanzamiento de un dado 1100 veces* </span>

``` r
dado <- c(1,2,3,4,5,6)
simuld <- NULL
nd <- 1100
simuld <- sample(dado, nd, replace = TRUE)
simuld
```

    ##    [1] 6 2 1 5 6 2 2 1 6 6 3 5 3 2 4 2 3 5 6 4 6 2 1 3 4 1 5 5 6 1 6 4 2 3 4 4 5
    ##   [38] 3 2 4 2 2 3 2 1 6 5 2 4 5 1 3 4 1 6 3 2 2 2 2 4 3 5 5 4 5 6 3 4 2 2 1 6 1
    ##   [75] 4 6 1 2 4 6 4 5 1 5 6 1 5 1 4 1 3 3 5 4 1 3 3 6 4 2 1 1 5 3 5 6 4 5 4 4 6
    ##  [112] 5 3 3 4 2 2 4 3 3 4 5 6 3 5 3 1 1 4 6 1 3 4 1 5 5 3 4 4 6 5 4 2 3 2 3 5 2
    ##  [149] 3 6 6 5 1 3 6 3 5 4 2 5 5 3 3 6 6 5 1 2 3 2 6 1 5 5 4 3 6 3 4 6 4 2 5 4 3
    ##  [186] 6 3 1 2 6 5 6 1 1 6 4 5 4 5 1 2 3 1 3 5 1 1 2 3 1 1 5 2 6 3 5 2 6 4 3 6 1
    ##  [223] 5 6 5 4 1 5 6 4 1 4 6 1 2 6 4 6 6 2 3 6 3 3 6 6 6 5 2 3 3 1 5 3 2 5 3 6 4
    ##  [260] 5 4 6 4 4 3 1 6 3 2 4 2 5 6 6 4 4 4 4 4 3 3 4 4 6 3 3 5 6 1 6 5 1 1 4 4 5
    ##  [297] 3 3 5 4 1 5 4 6 6 5 3 1 1 2 1 5 1 6 2 1 1 3 3 2 5 3 6 4 3 6 6 6 4 3 5 1 1
    ##  [334] 2 1 1 3 2 2 3 5 6 3 6 5 5 2 3 1 2 1 5 4 6 4 4 3 2 6 4 5 6 2 2 5 3 3 2 4 4
    ##  [371] 4 4 5 3 1 5 1 3 4 3 1 1 5 4 3 2 6 5 2 3 5 5 2 1 5 6 4 1 4 2 1 6 2 3 5 6 6
    ##  [408] 3 5 1 5 4 4 5 2 5 4 6 3 2 4 6 2 1 5 5 4 4 6 3 4 2 6 2 1 3 4 2 4 3 5 4 6 3
    ##  [445] 6 2 4 6 3 2 3 6 2 1 3 2 6 2 4 6 4 1 2 2 4 5 2 4 3 5 6 6 2 6 5 1 3 3 6 5 2
    ##  [482] 6 4 5 3 5 1 4 2 5 1 4 5 2 6 2 3 5 3 2 5 2 3 2 3 2 6 1 4 4 1 6 4 2 1 4 1 4
    ##  [519] 4 6 1 2 1 6 6 4 6 5 4 2 4 3 3 3 5 5 5 5 2 4 3 4 1 5 3 1 2 5 5 4 3 5 4 1 2
    ##  [556] 5 3 4 1 1 1 4 5 5 6 5 5 6 5 3 2 2 5 5 2 3 3 6 5 5 5 6 6 4 2 1 4 6 2 5 1 5
    ##  [593] 3 1 1 5 5 4 3 4 5 5 2 6 5 1 1 4 2 5 1 4 3 5 6 6 1 6 4 2 2 4 4 2 6 4 2 1 3
    ##  [630] 1 1 5 5 4 1 3 6 3 4 2 2 4 6 4 5 6 1 4 4 5 5 3 2 5 4 6 5 4 5 6 1 4 5 3 5 4
    ##  [667] 4 5 6 6 2 4 2 3 6 4 5 2 6 5 5 3 1 2 2 1 4 5 2 6 2 3 4 1 2 2 4 3 3 3 2 5 1
    ##  [704] 2 3 6 2 4 6 6 5 4 2 1 5 1 2 4 4 3 6 2 1 5 2 6 1 2 5 2 4 1 2 5 3 5 3 1 5 4
    ##  [741] 3 5 6 6 5 6 6 2 2 3 5 5 5 4 3 1 5 1 2 4 3 2 6 1 6 3 5 6 6 6 5 2 1 3 5 4 1
    ##  [778] 4 3 2 3 5 2 3 2 6 6 6 5 4 4 3 2 1 5 2 3 6 6 6 2 1 5 1 6 6 2 1 1 5 3 5 1 5
    ##  [815] 1 6 2 3 6 1 4 1 4 6 4 4 4 1 4 1 3 6 5 6 4 5 6 4 2 6 3 6 3 4 4 2 2 2 5 4 4
    ##  [852] 5 5 1 5 3 1 3 1 6 5 3 1 5 6 6 2 6 3 4 6 1 6 3 4 6 2 5 5 3 4 5 4 1 2 6 2 3
    ##  [889] 6 5 1 5 2 6 3 6 1 1 3 4 6 2 1 3 3 3 3 3 2 4 6 6 5 2 5 3 4 6 4 2 5 5 5 3 3
    ##  [926] 3 6 3 4 3 4 6 6 3 6 6 1 6 3 2 3 6 1 4 1 4 6 3 1 3 2 4 5 3 2 2 4 1 2 1 3 1
    ##  [963] 2 2 5 3 1 4 5 4 2 4 5 3 1 6 2 5 6 6 4 2 6 6 3 5 1 1 5 3 1 1 5 4 1 6 1 4 1
    ## [1000] 6 6 4 2 1 5 6 3 2 2 6 1 5 6 1 3 3 4 4 1 6 1 4 4 5 6 6 1 5 3 1 2 2 1 3 1 6
    ## [1037] 6 5 2 4 1 2 1 4 3 4 1 4 5 6 2 1 2 3 2 2 2 5 6 5 3 5 5 6 1 2 6 3 4 3 5 3 3
    ## [1074] 2 5 5 6 5 2 4 1 5 6 1 1 3 3 1 5 5 2 1 4 2 1 1 4 1 3 2

``` r
t2 <- table(simuld)
t2
```

    ## simuld
    ##   1   2   3   4   5   6 
    ## 171 173 182 187 198 189

``` r
t2p <- prop.table(t2)
addmargins(t2p)
```

    ## simuld
    ##         1         2         3         4         5         6       Sum 
    ## 0.1554545 0.1572727 0.1654545 0.1700000 0.1800000 0.1718182 1.0000000

``` r
### Ahora realizaremos un gráfico de la distribución de las frecuencias relativas utilizando la librería ggplot

library (ggplot2)
t2p <- as.data.frame(t2p)
ggplot(t2p, aes(x=simuld, y=Freq, label=Freq)) + 
  geom_point(stat='identity', fill="green", size=8)  +
  geom_segment(aes(x = simuld, 
                   xend = simuld, 
                   y = 0, 
                   yend = Freq), 
               color = "green") +
  geom_text(color="red", size=2) +
  labs(title="Gráfico 4: Distribución de frecuencias lanzamiento de un dado 1100 veces",
       x = "Cara del dado",y = "Frecuencias") 
```

![](Experimentos_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

### <span style="color:black">*1.1.3 Selección de los estudiantes con edades en el rango de 17 A 50 años* </span>

``` r
set.seed(1234)
ed_u <- sample(17:50, size=320,replace=T)
freq4 <-freq(ed_u,plot=T, col=rainbow(5), main="Gráfico 5: Distribución de Frecuencias edades")
```

![](Experimentos_files/figure-gfm/unnamed-chunk-4-1.png)<!-- -->

``` r
tab <- freq4
fx <- tab[,2]/100
tb <- cbind(tab,fx)

colnames(tb) <- c("Frecuencia","%","fx")
print(tb)
```

    ##       Frecuencia        %       fx
    ## 17             2   0.6250 0.006250
    ## 18            12   3.7500 0.037500
    ## 19            10   3.1250 0.031250
    ## 20            10   3.1250 0.031250
    ## 21             4   1.2500 0.012500
    ## 22            12   3.7500 0.037500
    ## 23             6   1.8750 0.018750
    ## 24             9   2.8125 0.028125
    ## 25             6   1.8750 0.018750
    ## 26            11   3.4375 0.034375
    ## 27             8   2.5000 0.025000
    ## 28             7   2.1875 0.021875
    ## 29            14   4.3750 0.043750
    ## 30            10   3.1250 0.031250
    ## 31            14   4.3750 0.043750
    ## 32            10   3.1250 0.031250
    ## 33             9   2.8125 0.028125
    ## 34             7   2.1875 0.021875
    ## 35            15   4.6875 0.046875
    ## 36            10   3.1250 0.031250
    ## 37            11   3.4375 0.034375
    ## 38            18   5.6250 0.056250
    ## 39            11   3.4375 0.034375
    ## 40             9   2.8125 0.028125
    ## 41             6   1.8750 0.018750
    ## 42             8   2.5000 0.025000
    ## 43            10   3.1250 0.031250
    ## 44             7   2.1875 0.021875
    ## 45             7   2.1875 0.021875
    ## 46            10   3.1250 0.031250
    ## 47            12   3.7500 0.037500
    ## 48            10   3.1250 0.031250
    ## 49            10   3.1250 0.031250
    ## 50             5   1.5625 0.015625
    ## Total        320 100.0000 1.000000

### <span style="color:black">*2. Gráficas de las funciones de probabilidad y de las distribuciones de la función de variables aleatorias* </span>

### <span style="color:black">*2.1. Simulaciones* </span>

### <span style="color:black">*2.1.1 Variables aletorias discretas* </span>

``` r
rm(list=ls())
set.seed(1234)
edad <- sample (17:50, 200, replace=T)
freq5 <- freq(edad,plot=F) 
plot(freq5, main="Gráfico 6: Histograma de la Edad",
     xlab="Edades",
     ylab="Frecuencias",
     col=rainbow(10))
```

![](Experimentos_files/figure-gfm/unnamed-chunk-5-1.png)<!-- -->

``` r
tab5 <- freq5
fx <- tab5[,2]/100
Fx <- cumsum(fx)
tab5 <- cbind(tab5,fx,Fx)
tab5
```

    ##       Frequency Percent    fx    Fx
    ## 17            2     1.0 0.010 0.010
    ## 18            9     4.5 0.045 0.055
    ## 19            7     3.5 0.035 0.090
    ## 20            5     2.5 0.025 0.115
    ## 21            4     2.0 0.020 0.135
    ## 22           10     5.0 0.050 0.185
    ## 23            4     2.0 0.020 0.205
    ## 24            8     4.0 0.040 0.245
    ## 25            6     3.0 0.030 0.275
    ## 26            5     2.5 0.025 0.300
    ## 27            5     2.5 0.025 0.325
    ## 28            5     2.5 0.025 0.350
    ## 29            3     1.5 0.015 0.365
    ## 30            4     2.0 0.020 0.385
    ## 31            6     3.0 0.030 0.415
    ## 32            7     3.5 0.035 0.450
    ## 33            6     3.0 0.030 0.480
    ## 34            4     2.0 0.020 0.500
    ## 35           10     5.0 0.050 0.550
    ## 36            7     3.5 0.035 0.585
    ## 37            7     3.5 0.035 0.620
    ## 38           14     7.0 0.070 0.690
    ## 39            7     3.5 0.035 0.725
    ## 40            4     2.0 0.020 0.745
    ## 41            5     2.5 0.025 0.770
    ## 42            5     2.5 0.025 0.795
    ## 43            3     1.5 0.015 0.810
    ## 44            5     2.5 0.025 0.835
    ## 45            5     2.5 0.025 0.860
    ## 46            6     3.0 0.030 0.890
    ## 47            4     2.0 0.020 0.910
    ## 48            8     4.0 0.040 0.950
    ## 49            6     3.0 0.030 0.980
    ## 50            4     2.0 0.020 1.000
    ## Total       200   100.0 1.000 2.000

``` r
n <- length(tab5[,1])
tab5[n,3:4] <- NA
edad1 <- seq(17,51)
## Gráfico
plot(tab5[,3],  main="Gráfico 7:Función Densidad Edad")
```

![](Experimentos_files/figure-gfm/unnamed-chunk-6-1.png)<!-- -->

``` r
par(mfrow=c(1,2))
plot(edad1,tab5[,3], type = "b", main="Gráfico 8:\nFunción Densidad Edad",
     xlab="Edades",
     ylab="f(x)",
     xlim=c(17,50))

plot(edad1,tab5[,4], type = "b", main="Gráfico 9: \nFunción Dist, Acumulada Edad",
     xlab="Edades",
     ylab="F(x)")
```

![](Experimentos_files/figure-gfm/unnamed-chunk-6-2.png)<!-- -->

### <span style="color:black">*2.1.1 Variables aletorias continuas* </span>

``` r
par(mfrow=c(1,2))
z <- seq(-5,5,0.5)
fz <-(1/sqrt(2*pi))*exp(-(z^2/2))
Fz <- pnorm(z,0,1)
plot(z,fz,main="Gráfico  10: \nDist. normal estandarizada - fz",
     type="l",
     xlab="Valores Z",
     ylab="f(z)")

abline(v=0,col="red",lty=3)

plot(z,Fz,main="Gráfico 11: \nDist. normal estandarizada - Fz",
     type="l",
     xlab="Valores Z",
     ylab="F(z)")
```

![](Experimentos_files/figure-gfm/unnamed-chunk-7-1.png)<!-- -->
