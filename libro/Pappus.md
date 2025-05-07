# Aplicaciones

## Segundo teorema de Pappus

:::{prf:theorem} Segundo teorema de Pappus 
El volumen de un cuerpo generado por revolución es igual al área de la sección multiplicado por la longitud de circunferencia que recorre el baricentro de la sección.
:::

Es decir

$$
V = 2\pi d A
$$

donde $d$ es la distancia del centroide de la sección al eje de revolución.

Vamos a demostrarlo. Supongamos que el eje de revolución es el eje $Oz$ en ese caso se tiene que el volumen se puede calcular en cilíndricas como:

$$
V = \iiint_\mathcal{B} dV= \int_0^{2\pi} \iint_\mathcal{S} r dA \,\mathrm{d}\theta  = 2\pi \iint_\mathcal{S} r dA
$$

Por otra parte, las coordenadas del baricentro de la sección vienen dadas por:

$$
r_{\mathrm{BC}} = \frac{1}{A}\iint_{\mathcal{S}} r dA
$$

$$
z_{\mathrm{BC}} = \frac{1}{A}\iint_{\mathcal{S}} z dA
$$

Con lo cual podemos reescribir el volumen como

$$
V = \iiint_\mathcal{B} dV= {2\pi} A r_\mathrm{BC} = 2\pi r_\mathrm{BC} A
$$
