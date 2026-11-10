# Ejemplos matemáticos públicos y acotados

Estos ejemplos ilustran cómo escribir hipótesis, demostrar un resultado y marcar sus límites. Son **resultados clásicos**; no constituyen pruebas de originalidad de ALM ni de problemas abiertos.

## Ejemplo A: descomposición mediante una involución

Sea \(V\) un espacio vectorial sobre un cuerpo de característica distinta de 2 y sea \(R:V\to V\) lineal con \(R^2=I\).

Definimos
\[
P_+=\frac{I+R}{2},\qquad P_-=\frac{I-R}{2}.
\]

**Proposición.** Se cumple
\[
P_+^2=P_+,\quad P_-^2=P_-,\quad P_+P_-=P_-P_+=0,\quad P_++P_-=I.
\]

**Prueba.** Como \(R^2=I\),
\[
(I\pm R)^2=I\pm 2R+R^2=2(I\pm R).
\]
Dividiendo por 4 se obtienen las identidades de idempotencia. Además,
\((I+R)(I-R)=I-R^2=0\), y la suma de ambos proyectores es \(I\). \(\square\)

**Límite:** esta proposición de álgebra lineal no acredita por sí misma cotas analíticas, regularidad de ecuaciones diferenciales ni un resultado físico nuevo. Para llamarlos *proyectores ortogonales* en un espacio con producto interno hay que exigir además propiedades como \(R^*=R\).

## Ejemplo B: transportar una cota de aproximación

Sean \((Y,d_Y)\) y \((Z,d_Z)\) espacios métricos, \(F,F_N:X\to Y\), y \(\phi:Y\to Z\) una función \(L\)-Lipschitz sobre las imágenes consideradas. Supongamos que para cada \(x\) del dominio analizado
\[
d_Y(F(x),F_N(x))\le\varepsilon_N(x).
\]

**Proposición.** Entonces
\[
d_Z(\phi(F(x)),\phi(F_N(x)))\le L\varepsilon_N(x).
\]

**Prueba.** Aplicar la definición de función \(L\)-Lipschitz a los puntos \(F(x)\) y \(F_N(x)\), y usar la cota asumida. \(\square\)

**Límite:** esta conclusión no demuestra que exista una cota pequeña \(\varepsilon_N\) en un problema concreto, ni proporciona por sí sola una constante válida \(L\). Ambos datos son obligaciones independientes.

## Ejemplo C: mismo espectro no implica misma medición local

Sean \(A=\operatorname{diag}(1,2)\) y \(B=\operatorname{diag}(2,1)\). Tienen los mismos autovalores \(\{1,2\}\), pero \(A_{11}=1\) y \(B_{11}=2\).

**Conclusión acotada:** la igualdad del multiconjunto de autovalores no garantiza igualdad de una observación ligada a una base fijada. No se infiere de ello una nueva teoría de geometría espectral.

---

**Criterio editorial:** cualquier generalización futura deberá publicar las hipótesis extra que permiten pasar de estos ejemplos a un resultado más amplio.
