Mario C velez G
que nombre 

un metodo, para que un metodo?
metodos para resolver problemas?
que problemas
el metodo permite abordar un modelo

descripcion del curso
contenido
pacto pedagogico
plan de trabajo
comunicacion con el profe

por que es importante en el curriculo:

reconocer sistuaciones donde puedo usar ingenieria par resolver un problema
modelar , traducir problemas a modelos matematicos
interpretar  las salidas del software
resolver 

essentially,all models are wrong but some are useful
george E. P Box

1 identificar el problema
2 desarrollare un modelo formal del problema
3 traducir el modelo formal en un modelo computacional

Tipos de modelos

determinista
Mismo punto de partida + Mismas reglas = Exactamente el mismo resultado.

estocastico (tiene condiciones aleatorias)
Mismo punto de partida + Mismas reglas = Diferentes resultados posibles con distintas probabilidades.

descriptivo: (que pasa si)(que paso)

> **Qué pasó? o ¿Qué está pasando?**

Un modelo descriptivo se encarga de **reunir, organizar y resumir datos históricos o en tiempo real** para identificar patrones, tendencias y anomalías. Su objetivo principal es brindar visibilidad y comprensión del estado actual o de eventos pasados.

- **Enfoque:** Reactivo e histórico.
    
- **Qué hace:** Consolida grandes volúmenes de datos en métricas digeribles. No intenta adivinar el futuro ni decirte qué hacer; solo te muestra la foto exacta de la realidad.

prescriptivo

> **¿Qué es probable que pase?**

Antes de llegar a la prescripción, necesitamos estimar el futuro. Los modelos predictivos utilizan los datos históricos (del modelo descriptivo) y algoritmos estadísticos o de _Machine Learning_ para **estimar la probabilidad de eventos futuros**.

- **Enfoque:** Proactivo y probabilístico.
    
- **Ejemplos prácticos:** Pronósticos de demanda de inventario, detección de transacciones fraudulentas o modelos de fuga de clientes (_churn_).
construccion

los modelos de analitica tienen 4 estados

Analítica Descriptiva (¿Qué pasó?)
Analítica Diagnóstica (¿Por qué pasó?)
Analítica Predictiva (¿Qué pasará?)
Analítica Prescriptiva (¿Cómo podemos hacer que pase? / ¿Qué debemos hacer?)

no hay forma de saber si todos los problemas tienen solucion

| **Clasificación**         | **Modelos deterministas**                  | **Modelos estocásticos**                          |
| ------------------------- | ------------------------------------------ | ------------------------------------------------- |
| **Modelos descriptivos**  | Hojas de cálculo, Dinámica de sistemas     | Teoría de colas, Simulación                       |
| **Modelos prescriptivos** | Programación lineal, Programación dinámica | Programación estocástica, Simulación-optimización |
## Construccion

### Modelo descriptivo

- **Entradas:** Parámetros.
- **Proceso:** Representación o simulación del sistema.
- **Salida:** Medidas de desempeño.

### Modelo prescriptivo

- **Entradas:** Parámetros y variables de decisión.
- **Proceso:** Optimización bajo restricciones.
- **Salida:** Decisión óptima y medidas de desempeño.


tenemos que programar 

reconozer los problemas
desarrollar habilidades de solicion
dar soluciones
analizar

## pensum
### programacion lineal
- introducción a la Investigación de Operaciones y sus campos de aplicación.
- El problema de optimización y características de los problemas de programación lineal.
- Formulación de modelos de programación lineal.
- Solución gráfica.
- Introducción al Método Simplex.
- Solución utilizando software e interpretación de las salidas.

### simulacion
- Introducción a la simulación y conceptos básicos.
- Proceso de simulación.
- Generación de números y variables aleatorias.
- Uso de software para el análisis de datos de entrada.
- Simulación con hojas de cálculo (Monte Carlo).
- Análisis de resultados.
- Modelación continua y ejemplos.

Notas
Teoria de colas, 
La **teoría de colas** es una rama de las matemáticas y la investigación de operaciones que estudia cómo se forman las filas o colas de espera y cómo diseñar sistemas para atender a los usuarios de la manera más eficiente posible.

La **dinámica de sistemas** es una metodología de modelado y simulación que permite comprender cómo evolucionan sistemas complejos a lo largo del tiempo.

evaluaciones a la vieja escuela no tech

|Semana|Fecha|Evaluación|Valor|
|---|---|---|---|
|6|Agosto 19|Taller 1|**15%**|
|8|Septiembre 2|Parcial 1|**25%**|
|13|Octubre 16|Taller 2|**15%**|
|17|Noviembre 13|Parcial 2|**25%**|
|1-17|—|Seguimiento|**20%**|

la programacion lineal nacio durante la segunda guerra mundial , para optimizar recusos
que hace? convierte un problema real de asignacion de recurosos

ejemplos de la clase,va  ser manufactura y transporte

### problema
info , silla , mesa
utilidad, 12 000, 8 000
metros lineales de madera ,4,2
tiempo de ensamble , 1 ,1
tiempo de pintura 1,1

recursos
operario ensamblando sillas 2
operario ensamblando mesas 3
operaios de pintura 4
metros lienales de madera 90


Preguntas
segun la diapositiva 4  que software usariamos
Cual seria el nuevo nombre del curso?

# Clase 2

Lo que esta dentro del area total es posible
lo que esta fuera no es posible o tiene limitantes
donde se interceptan las lineas es el punto optimo

el total se saca multiplicando los valores

sillas a 8 y mesas a 12 , pero las sillas consumen el doble de madera de las  mesas
osea T=12S1+8M2

partes del problema
**variables de decicion** (sobre que desidimos)
**problema de optimizacion**(la medida para maximizaor o minimar)
**Restricciones** Limitantes del problema

en programacion lineal hay muchas soluciones optimas, 
Como uno sabe uno la cantidad de soluciones optimas

tambien hay programacion no lineal

Los modelos de programacion lineal se pueden usar para cuadrar horarios  y es rapido

cual desicion es mejor que otra , mediante algo cuantitativo

Pasos para solucionar un problema de programacion lineal

hallar 
variables
combistibles A y B
2000 de A
4000 de B

objetivo
minimizar costo

restriccion
la mescla debe tener un minimo de 80%
min(3.000)
max(4.000)

con fracciones es valido matematicamente pero un programa de pc no lo va resolver

metodo simplex

generar  la idea buscar en los vertices

la frontera es el conjunto de soluciones, cumple en igualdad
punto interiror, soluciones las cuales todas la restricciones se cumplen en desigualdad
(sobra de todo)
busca punto extremo vertice, en la frontera se consumen 2 recursos o mas , osea la solucion optima


dame un vertice y solucionare el problema, 

# Clase 3

Hay proble,mas que no tienen solucion

Pyomo

PulP

Google-OR-Tools 

algoritmo para esto
punto inmterrior
brnach and cut

hay 2 modeladores y solvers
modeladores  no implementan simplex method


Trayectos medellin bogota
12 camiones
bogota 3 dias de camion y genera 4 200 utilidades, minimo 6 viajes semanales
cali 2 dias de camion y genera 2800 utilidades, a cali maximo 10 viajes semanales

variables de decision

trayecto, 
cuantos viajes a medellin bogota = Vb
cuantos viajes a medellin cali = Vc

objetivo
maximisar utilidades
max(z)=4.2Vb +2.8Vc

Limitantes
12 camiones* 6 dias de la semana
3Vb+2Vc <= 72 

viajes cali < 10 , cada semana
viajes bogota > 6  , cada semana
semana 6 dias

Ejercicio 2

Variables de desicion
cual porcion cocinar

bandeja paisa = Cb
sopa de dia = Cs
pasta vegetaria = Cp

Funcion objetivo

max(z)= 9000Cb+ 5500Cs+ 7500Cp

Restricciones

600 minutos de cocina
600 mins <= 12Cb+6Cs+8Cp

700 000 presupuesto diario ingredientes
700 000$  <= 9000Cb + 4500Cs+ 5500Cp

0<Cb<=50
0<Cs<=80
0<Cp<=60

# Clase 4

### variables
variables, al inicio del ano

cdt  bianual w1,w2,w3,w4
cdt trianual x1,x2,x3
fondo semilla y2
pagare R z5
no invertir r1,r2,r3,r4,r5

objetivo

maximisar rendimiento 
max(z) = R5+1.35w4+1.55x3+175y2+1.2

restricciones
ano 1
 60 <= w1+x1+r1

ano 2
r1 = w2+x2+y2+r2

ano 3
1.35w1+r2 = w3+x3+r3

ano 4 
1.55x1+1.35w1+r3 = w4+x4+r4

ano 5
1.55x2+1.35w3+ry = z5+r4

dinero a invertir < 60 000 
tiempo < 5 anos
Tcdt1
Tcdt2
Tcdt3
Tcdt4


Rcdt1 =1.35
Rcdt2 =1.55
Rcdt3 =1.75
Rcdt4 =1.2


ejemplos de problemas
Production Planning
Resource Allocation
Transportation and Logistics
Scheduling
Business and Finance
Agriculture
Supply Chain Management
Healthcare
Telecommunications and Networks
Military and Defense

RHS right hand side

Sadow Price
es una tasa de cambio
**Shadow Price (Precio Sombra)** Es la tasa de cambio instantánea en el valor de la función objetivo óptima ($Z$) por cada unidad de incremento en el lado derecho ($RHS$) de una restricción. Indica cuánto está dispuesto a pagar el modelo por obtener una unidad adicional de un recurso limitante.

$\frac{\text{Unidades de } Z}{\text{Unidades del recurso}}$

olgura
**Holgura y Exceso (Slack & Surplus)**

- **Holgura (_Slack_):** Cantidad de recurso que queda sin utilizar en una restricción de tipo menor o igual ($\le$).
$$\text{Holgura } (s) = RHS - \text{Recurso Consumido}$$
- **Exceso (_Surplus_):** Cantidad en la que se sobrepasa el requerimiento mínimo en una restricción de tipo mayor o igual ($\ge$).

# Clase 5

una formula para infinitos problemas

Taller parejas
formulacion de problemas

Se puede imprimir notas

describir un modelo de miles de variables
toca desacopar los datos del modelo

por que albegraico
modelo algebraico
max z = sum (cj)

conjuntos e indices el vocabulario de la generalidad

Conjuntos letras mayusculas

Conjuntos
parametros
variable de decicion
funcion objetivo
restriciones
resolver

conjunto
I recursos
J productos
Prametros

cj utilidad por unidad vendida de j en J
bi cantidad disponible del recurso I en I
aiJ Cantidad nesesaria del recurso i en I
para fabricar  una  unidad del producto j en J

Variables de desicion

Xj litros a producir

Funcion objetivo

Max z = sum (cj,xj)  jeJ

Restricciones
sum jEJ sum (aij,xj) < bi
```python
import  pulp as pl

#insanciar modelo

prob =pl.LpProblem("Maximizar utilidad",pl.LpMaximize)

J =["Natural","premium"]
I = ["Fruta","maquina","empaque"]
c = {"Natural":3500,"Premium":5000}
b={"Fruta":90,"maquina":40,"empaque":30}
a={"Fruta":{"Natural":2.0,"premium":3.0},"maquina":{"Natural":0.5,"premium":1.0},"empaque":{"Natural":1.0,"premium":0.5}}

x = {"x"+j:pl.LpVariable("x_"+j,lowBound=0) for j in J}
x = {j: pl.LpVariable('x_'+j,LowBound=0) for j in J}

#funcion objetivo

prob+= pl.lpSum(c[j]*x[j] for j in J)

#restricciones
for i in I:
	prob+= pl.lpSum(c[j]*x[j] for j in J) <=b[i],"restriccion_"+i
prob.solve()
#imprimir solucion optima
print("utilidad", prob.objetive.value())
print("litros natural", x["Natural"].varValue())
print("litros natural", x["Premium"].varValue())	
```
## Revision quiz



4.4 estubo bien

nos equivocamos en la segunda restriccion de   politicas de marca

no era S+I = 100%; I>=40%,

era I/(A+I) >= 0.4 ,I>=0.4(S+I)

Cual es el precio sombra de las horas del taller? justifique

El precio sombra es cero por que no cambio, No indefinido, por que no cambio

## Clase 6

Modelo algrebraico

antes se veia con numeros ya no, se utilizan elementos, simbolizados por letras mayusculas, para producir estos productos nesesitamos recursos, tengo que usar todos los elementos en terminos de los conjuntos

Aij coenficiente tecnologivo
cuanto es el consumo del recurso i por cada una unidad de producto j que voy a producir

Cuales son las variables de decicion

Modelo canonico de mescla de productos

$Maximizar z \sum_{j\in J} j$


es el mismo modelo para todo

para todo

## Clase 7
3 patrones que resuelva cientos de problema

el modelo algebraico describe la estructura de un tipo de problema en la practica esa estructura se repite una y otra vez con distintos datos

Familias de problema 

mesclas,
min costo
cuanto producir de cada producto

blending
en que proporcion mesclar 

transporte
min costo

multi periodo
min costo

Mescla de ingredientes

ingredientes,proteina,grasa,costo ($/KG)
maiz,9%,4%,800
soya 44%,2%,2 200
sorgo 8% ,3% ,600

proteina minimo 18%
grasa maximo 6%

La empresa quiere el concentrado mas barato por kilogramo que compla las 2 especificaciones

Defina
Conjuntos
Parametros
y variables de decicion

Conjunto
IngredientesI,i
Nutirentes:N,j

Parametros
$g_i$ Fraccion de grasa $i \in I$
$p_i$ Fraccion de Proteina $i \in I$ 

Realment es
$f_{ij}$ Fraccion en el ingrediente de  $i \in I$ del nutriente  $j\in N$

$c_i$ Fraccion de Kg $i \in I$

$l_i$ Fraccion minimo del  nutriete $j \in N$ en la mezcla
$u_i$ Fraccion Maximo del  nutriete $j \in N$ en la mezcla

$x_i$ Kilos del ingrediente $i\in I$ en un Kg de mescla
Objetivo
min Z = $\sum_{i \in I}{c_i,x_i}$
Restricciones
 $l_j\leq \sum_{i\in I}f_{ij}x_i \leq u_j \forall j \in N$ 


Modelo 2 Problema del transporte

Origen, oferta (Ton)
Medellin 300
Bogota 500

Destino demanda (Ton)
Cali 200
Barranquilla 350
Bucaramanga 150

Costo de transporte ($/ton), cali,barranquilla, bucaramanga
Medellin,850,1200,920
Bogota,1100,980,760

La oferta total 800 ton supera la demanda total 700 ton de modo que no todas las plantas tendran  que despachar todo lo que pueden

Debemos hayar

Conjuntos
Parametros
Variables de desicion

Conjuntos
CiudadOrigen , O,o
CiudadDestino ,D ,o

Parametros
$a_o$ Ofererta disponible en el origen o
$b_d$ Demanda del destino d
$x_{od}$ Toneladas enviadas desde el origen al destiono