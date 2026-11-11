# UNAI–ALM | Dossier público para revisión académica (REF)

**Versión:** REF-PUBLICO-2026-11-11-v1.0  
**Fecha:** 11 de noviembre de 2026  
**Investigador y proponente:** Antonio López Martínez  
**Proyecto:** UNAI–ALM / Atomic Logical Method (ALM)  
**Estado:** material de consulta pública para crítica científica. **No es un manuscrito aceptado, una evaluación por pares realizada ni una reivindicación de resolución de los problemas del Milenio.**

## 1. Objetivo y límites

Este dossier es la **capa pública y no sensible** para facilitar a personas revisoras el examen de enunciados, supuestos, ejemplos reproducibles, contraejemplos y obligaciones todavía abiertas. No reproduce el expediente REF interno, anexos inéditos, código reservado ni documentación de otros desarrollos independientes. La existencia de un dossier público **no equivale al envío de una candidatura a una revista** o a una aceptación de revisión por parte de terceros.

ALM se presenta como un *programa de investigación* para explicitar relaciones entre estructuras matemáticas mediante hipótesis, dominios, invariantes, transformaciones, nociones de compatibilidad y condiciones de prueba. Una analogía entre modelos no prueba una transferencia de resultados ni una ley universal.

## 2. Estado de las principales líneas

| Línea | Qué se presenta públicamente | Qué NO se ha establecido |
| --- | --- | --- |
| ALM | Método de exploración estructural y protocolo de trazabilidad de afirmaciones | Una teoría universal validada |
| Navier–Stokes 3D (NS3D) | Programa de estudio de regularidad y estimaciones condicionadas | Existencia y regularidad globales del caso general |
| Hipótesis de Riemann (RH) | Línea de investigación de relaciones analíticas y espectrales | Una prueba de RH |
| Conjetura de Hodge | Línea de exploración geométrica/cohomológica | Una prueba de la conjetura |
| Álgebra / análisis elementales | Identidades delimitadas con demostraciones explícitas | Que los ejemplos sean descubrimientos originales o cierren los problemas anteriores |

Los problemas citados permanecen **abiertos** en el sentido de este expediente. Las comprobaciones en modelos o con herramientas informáticas no deben extrapolarse sin una demostración de transferencia al dominio correspondiente.

## 3. Tres pruebas elementales y sus límites

Estos ejemplos son matemática conocida y ya están descritos en [Ejemplos matemáticos públicos](03_EJEMPLOS_MATEMATICOS.md). Se incluyen para ilustrar el estándar de exposición, **no como demostraciones de los problemas abiertos**.

**P1 — Proyectores de una involución.** Sea \(V\) un espacio vectorial sobre un cuerpo de característica distinta de dos, y \(R:V\to V\) lineal tal que \(R^2=I\). Los operadores
\[
P_+=(I+R)/2,\qquad P_-=(I-R)/2
\]
cumplen \(P_\pm^2=P_\pm\), \(P_+P_-=P_-P_+=0\) y \(P_++P_-=I\). **Prueba:** desarrollar \((I\pm R)^2=2(I\pm R)\) y \((I+R)(I-R)=I-R^2=0\). No se presupone ortogonalidad sin hipótesis adicionales.

**P2 — Transporte Lipschitz de errores.** Si \(F,F_N:X\to Y\) verifican \(d_Y(F(x),F_N(x))\le\varepsilon_N(x)\) y \(\phi:Y\to Z\) es \(L\)-Lipschitz sobre las imágenes usadas, entonces \(d_Z(\phi(F(x)),\phi(F_N(x)))\le L\varepsilon_N(x)\). **Prueba:** aplicar directamente la definición de Lipschitz. La existencia de una \(L\) adecuada o de un error controlable en un caso físico es **otra obligación**, no una consecuencia de este lema.

**P3 — Igualdad espectral no determina observables en una base fija.** Para \(A=\operatorname{diag}(1,2)\) y \(B=\operatorname{diag}(2,1)\), los espectros coinciden, pero \(A_{11}=1\ne B_{11}=2\). **Conclusión:** los autovalores no bastan para inferir igualdad de todas las mediciones locales.

## 4. Tres contraejemplos / barreras de extrapolación

- **C1 — Sin involución no hay idempotencia garantizada.** Sobre \(\mathbb R\), con \(R=0\), se tiene \(P_+=I/2\) y \(P_+^2=I/4\ne P_+\); eliminar \(R^2=I\) invalida P1.
- **C2 — Sin cota Lipschitz no hay constante global fija.** Sobre \([0,1]\), con \(\phi(t)=\sqrt t\), \(F(x)=0\) y \(F_N(x)=\varepsilon\), el error de salida es \(\sqrt\varepsilon\) mientras el de entrada es \(\varepsilon\). Ninguna \(L\) independiente de \(\varepsilon\to0\) satisface la conclusión de P2.
- **C3 — Información incompleta no garantiza reconstrucción.** La observación \(O(x)=x^2\) cumple \(O(1)=O(-1)\); sin datos adicionales no existe una inversa bien definida sobre ambas entradas. Este ejemplo **no** demuestra una pérdida concreta en NS3D, RH o Hodge: solo identifica un control requerido antes de afirmarla o descartarla.

## 5. Obligaciones abiertas para que un «puente» sea matemáticamente evaluable

1. **Dominio y enunciado:** definir explícitamente los espacios y las clases de objetos de NS3D, RH y Hodge que se pretenda relacionar, sin confundir objetos físicos, analíticos y cohomológicos.
2. **Mapas y alcance:** construir mapas efectivos entre los espacios propuestos (o hacia un espacio común) y demostrar que están bien definidos; **no se declara aquí su existencia**.
3. **Invariantes y pérdida:** precisar qué propiedades conserva cada mapa; probar, cuando se afirme, inyectividad, reconstrucción con información auxiliar o una cota de error útil.
4. **Composición:** verificar que las compatibilidades exigidas son coherentes bajo composición; una coincidencia por pares o en un ejemplo finito no basta para una conclusión global.
5. **NS3D:** identificar un lema nuevo no circular que proporcione las estimaciones necesarias en el dominio original, sin asumir indirectamente la regularidad buscada.
6. **RH:** cualquier afirmación sobre ceros requiere un resultado válido para el objeto analítico original, no solo para aproximaciones matriciales o modelos numéricos.
7. **Hodge:** distinguir la descomposición de Hodge lineal/discreta de la conjetura sobre clases racionales y ciclos algebraicos.
8. **Reproducibilidad y procedencia:** exhibir hipótesis, pruebas, referencias, código/datos autorizados y resultados negativos; diferenciar inequívocamente demostración, prueba asistida, simulación y conjetura.

**Estado de cierre:** todas las obligaciones de transferencia general citadas se consideran **pendientes** hasta que exista evidencia específica reproducible y revisada.

## 6. Protocolo de revisión

Para una revisión útil se pide indicar la afirmación exacta, hipótesis, dominio, demostración o contraejemplo, posible circularidad y referencias pertinentes. No se atribuirá a ninguna persona o institución una validación por el simple hecho de leer o comentar el material. Véase [Protocolo de revisión externa](04_REVISION_EXTERNA.md).

La clasificación editorial aplicable es: **demostrado en dominio declarado / verificado en modelo / condicional / conjetural / no evaluado**. Las correcciones deben ser trazables. La ausencia de respuesta no implica aprobación.

## 7. Referencias, autoría y materiales reservados

- **DOI central indicado por el autor:** [10.5281/zenodo.24075954](https://doi.org/10.5281/zenodo.24075954). Su mención **no acredita** que este dossier concreto esté depositado en Zenodo ni que exista evaluación por pares. La correspondencia documental debe comprobarse independientemente.
- **DOI histórico relacionado declarado:** [10.5281/zenodo.18761284](https://doi.org/10.5281/zenodo.18761284). No se presupone equivalencia de versiones.
- [Estado científico público](02_ESTADO_CIENTIFICO.md), [Ejemplos](03_EJEMPLOS_MATEMATICOS.md), [Política de DOI](06_REFERENCIAS.md), [Autoría, procedencia y asistencia de IA](05_AUTORIA_Y_PROCEDENCIA.md).

**No incluye** repositorios privados, originales históricos, código/datos experimentales reservados ni documentación de desarrollos independientes. La evaluación de material reservado solo podrá tramitarse separadamente, con autorización y supervisión expresas. **Los originales no se han modificado.**

**Invitación:** se solicitan críticas científicas, errores verificables, contraejemplos y propuestas de cierre de obligaciones, sin presumir resultados ni aval institucional.