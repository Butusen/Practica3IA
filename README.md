# PRÁCTICA 3: APRENDIZAJE AUTOMÁTICO


## 1. Elegir el problema

En nuestro caso hemos escogido los datos de los partidos de la ATP 

## 2.Identificar la fuente de datos

Hemos escogido los partidos de la ATP de 2018 localizados en: 

[datos](https://github.com/JeffSackmann/tennis_atp/blob/master/atp_matches_2018.csv)

## 3.Identificar las características relevantes de los hechos

En el fichero original había muchos más atributos de los cuales nos quedamos con los que hemos considerado más relevantes: surface, ranking y ganador.
<br />
surface: Como la superficie donde se juega el partido de tenis del `{Hard,Clay, Grass}`
<br />
ranking: Como el ranking del primer jugador y del segundo jugador como datos enteros: `{123,68}`
<br />
winner: Como el ganador del partido a analizar: `{0rank ó 1rank}`
<br />
Los jugadores están definidos como `0rank` el `jugador0` y `1rank` el `jugador1`.

## 4.Obtener un fichero .arff

Mediante el programa de Weka, introduciendo los datos del .csv generamos el fichero `atp_matches.arff` y posteriormente el `test.arff` para analizar un caso concreto.

## 5.Evaluación de los distintos algoritmos de aprendizaje automático con los datos

Una vez evaluados los algoritmos en la pestaña de classify, nos quedamos con el algoritmo MultiLayerPerceptron ya que es el que mayor ROC Area nos da a la hora de hacer el análsis. Esto se sabe que es correcto ya que el ROC está por debajo de 1.

![image](https://user-images.githubusercontent.com/65571317/146685976-82251ce9-c548-48e9-af59-23593880878c.png)
## 6.Generar un Java un objeto persistente con el algoritmo obtenido en el paso 

El objeto se genera al ejecutar el `java -jar ejecutable.jar`.
<br />
![image](https://user-images.githubusercontent.com/65571317/146686389-c52b29a0-047c-47af-a8e5-c493650a9274.png)


## 7.Implementar un prototipo de aplicación que consulte el objeto persistente generado en el paso 6

Al hacer el `make jar` se genera el `ejecutable.jar` con el que se comprobarán los resultados.
<br />
![image](https://user-images.githubusercontent.com/65571317/146686632-74c77542-2f5e-4d36-b704-633a7e47f09e.png)



Al hacer el `java -jar ejecutable.jar` comprobaremos que se ejecuta el resultado y que se genera el modelo.
<br /> 
![image](https://user-images.githubusercontent.com/65571317/146686389-c52b29a0-047c-47af-a8e5-c493650a9274.png)

## Autores ✒️

* **José Morán Nebot** - [Butusen](https://github.com/Butusen)
* **Miguel Melero Bernal** -[mikimb99](https://github.com/mikimb99)

## Licencias 

Copyright [2021] [José Morán Nebot y Miguel Melero Bernal]
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at
[apache](http://www.apache.org/licenses/LICENSE-2.0)
Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

