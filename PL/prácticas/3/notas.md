# Tarea 2
## 1� parte: an�lisis de la productividad en punto nominal y tiempo de respuesta
5 mediciones: en el punto nominal, 5 minutos 1 arranque
1 medici�n: 5 usuarios 20 minutos 1 arranque


### F�rmulas
- n = 5
- alpha = 0,95 -> 1-alpha = 0,05

- intervalo de confianza: $\overline x\pm t_{\alpha/2;n-1}\times{s\over \sqrt{n}}$
- t: `=DISTR.T.INV(1-alpha; n-1)`
- error: $e={t_{\alpha/2;n-1}\times{s\over\sqrt{n}}\over\overline x}\times 100$
$$n=({t_{\alpha/2;n-1}\times s\times 100\over\overline x\times e})^2$$

## 2� parte: histograma

1. Hacer un rango entre los extremos del tiempo de respuesta.
2. Histograma: `datos > an�lisis de datos > histograma`
3. Columna separada para frecuencia relativa.
4. Crear gr�fico del histograma con las frecuencias relativas.

# Tarea 3
Hacer una estad�stica descriptiva para los tiempos de respuesta de cinco usuarios.

**Objetivo:** sugerir una de las familias de distribuciones del PDF de distribuciones continuas.
Hay que argumentar.

## OPCIONAL: an�lisis de distribuciones
1. Valores normales
2. Hacer una gr�fica con los valores normales.
3. Hacer un histograma con los valores normales y los valores del histograma obtenidos.
4. Valorar si ambas gr�ficas se parecen y si se ha escogido la familia de distribuciones correcta.


---
**ENTREGA: 30 octubre**