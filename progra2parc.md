![LOGO COMPLETO](https://user-images.githubusercontent.com/113397997/190875735-0e9ea8a0-161e-49d4-8b1d-de55ac5f2877.png)
# Presentación
## Jose Armando Andrade Ramos 
## Primer Semestre
## Facultad de Ingeniería Mecánica y Electrica
## Problemas resueltos en clase con Diagramas de Flujo de Datos
### Ejercicio 1. Suma de los numeros 1 al 10 (for)
#### 1.1 Análisis
Se hace un ciclo for para generar los numeros y un acumulador para sumarlos.
#### 1.2 Diagrama de flujo de datos
![Suma for](https://user-images.githubusercontent.com/113397997/197898365-e39a8294-329d-4bac-b391-37be0915f4cc.png)
### DFD
#### 1.3 Prueba de escritorio 
|Suma|i|i<=10|s=s+i|i++|Salida|
|-|-|-|-|-|-|
|0|1|1<=10|0+1|1+1||
|1|2|2<=10|1+2|2+1||
|3|3|3<=10|3+3|3+1||
|6|4|4<=10|6+4|4+1||
|10|5|5<=10|10+5|5+1||
|15|6|6<=10|15+6|6+1||
|21|7|7<=10|21+7|7+1||
|28|8|8<=10|28+8|8+1||
|36|9|9<=10|36+9|9+1||
|45|10|10<=10|45+10|10+1|55|
#### 1.4 Entradas de datos
### Ninguna
#### 1.5 Salidas
55 
```
#### Codigo 
// Contar del 1 hasta el 10 y sumar los valores.
void main() {
  int s = 0;
  for (var i = 1; i <= 10; i++) {
    s += i;
  }
  print("La suma de los valores es: $s"); }
  //for
  ```
### Ejercicio 1.1 (while) Sumar los valores del 1 al 10
#### Analisis 1.1.2 
Se asigna una variable que inicia en 0 "s" y otra que inice en 1 "c" luego con una se asigna la condicion de termino y en la otra se almacena la suma.
#### 1.1.3 Diagrama de flujo de datos
![SumaWhile](https://user-images.githubusercontent.com/113397997/197900095-36784cca-3425-44a8-99ca-456e451b34fa.png)
####DFD
#### 1.1.4 Prueba de Escritorio 
|Suma|Cont|Cont<=10|Suma=Suma+Cont|Cont=Cont++|Salida|
|-|-|-|-|-|-|
|0|1|1<=10|0+1|1+1||
|1|2|2<=10|1+2|2+1||
|3|3|3<=10|3+3|3+1||
|6|4|4<=10|6+4|4+1||
|10|5|5<=10|10+5|5+1||
|15|6|6<=10|15+6|6+1||
|21|7|7<=10|21+7|7+1||
|28|8|8<=10|28+8|8+1||
|36|9|9<=10|36+9|9+1||
|45|10|10<=10|45+10|10+1|55|
#### 1.1.5 Entradas
No hay
#### 1.1.6 Salidas
55
#### 1.1.7 Codigo
```
// Contar del 1 hasta el 10 y sumar los valores.
void main(List<String> args) {
  int s = 0, c = 1;

  while (c <= 10) {
    s += c;
    c++;
  }
  print("El resultado de la suma de los valores es:$s");
} //while
 ```
 ### Ejercicio 1.2 Suma de los numeros del 1 al 10
 #### 1.2.1 Analisis 
 Se asignan dos variables Suma y Cont inicializadas en 0 y 1 respectivamente, luego se inicia el proceso donde se le suman a las variables cont y +1 respectivamente, hasta que la condicion encontrada al final se cumpla
 #### 1.2.2 Diagrama de flujo de datos 
 ![SumaDowhile](https://user-images.githubusercontent.com/113397997/197901109-a075bfe3-cabd-4842-91f1-83f1054474b8.png)
 ####DFD
 #### 1.2.3 Prueba de escritorio 
|Suma|Cont|Suma=Suma+Cont|Cont=Cont++|Cont<=10|Salida|
|-|-|-|-|-|-|
|0|1|0+1|1+1|2<=10||
|1|2|1+2|2+1|3<=10||
|3|3|3+3|3+1|4<=10||
|6|4|6+4|4+1|5<=10||
|10|5|10+5|5+1|6<=10||
|15|6|15+6|6+1|7<=10||
|21|7|21+7|7+1|8<=10||
|28|8|28+8|8+1|9<=10||
|36|9|36+9|9+1|10<=10||
|45|10|45+10|10+1||55|
#### 1.2.4 Entradas 
Ninguna 
#### 1.2.5 Salidas
55 
#### 1.2.6 Codigo 
```
void main(List<String> args) {
  int s = 0, c = 1;
  do {
    s += c;
    c++;
  } while (c <= 10);
  print("El resultado de la suma de los valores es:$s");
}
```
### 2 Ejercicio Obtenga la suma de los 5 primeros numeros pares 
#### 2.1 Analisis 
Se crea un contador del 1 al 5 y en una variable se acumula el contador multiplicado por 2 por cada numero del 1 al 5
#### 2.2 Diagrama de flujo de datos
 ![SumaparFor](https://user-images.githubusercontent.com/113397997/197903943-0f6c7ded-5f6b-4afa-bf28-a621290f0d58.png)
#### DFD
#### 2.3 Prueba de escritorio 
|s|i|i<=5|s=s+ i * 2|i++|salida|
|-|-|-|-|-|-|
|0|1|1<=5|0+ 1 * 2|1+1||
|2|2|2<=5|2+ 2 * 2|2+1||
|6|3|3<=5|6+ 3 * 2|3+1||
|12|4|4<=5|12+ 4 * 2|4+1||
|20|5|5<=5|20+ 5 * 2|5+1|30|
#### 2.4 Entradas 
Ninguna
#### 2.5 Salidas
30 
#### 2.6 Codigo 
```
dart
void main(List<String> args) {
  int s = 0;
  for (var i = 2; i <= 10; i = i + 2) {
    s = s + i;
  }
  print("resultado de la suma de numeros pares es:$s");
}
```
#### 2.1.1 Ejercicio Obtenga la suma de los 5 primeros numeros pares 
#### 2.1.2 Analisis
Se asigna una variable que inicia en 0 "s" y otra que inice en 1 "c" luego con una se asigna la condicion de termino y en la otra se almacena la suma del contador multiplicado por 2.
#### 2.1.3 Diagrama de flujo de datos 
![Sumaparwhile](https://user-images.githubusercontent.com/113397997/197905652-656ce027-0a6a-4902-b29f-b378723ab119.png)
#### 2.1.4 Prueba de escritorio 
|s|c|c<=5|s=s+ i * 2|c++|salida|
|-|-|-|-|-|-|
|0|1|1<=5|0+ 1 * 2|1+1||
|2|2|2<=5|2+ 2 * 2|2+1||
|6|3|3<=5|6+ 3 * 2|3+1||
|12|4|4<=5|12+ 4 * 2|4+1||
|20|5|5<=5|20+ 5 * 2|5+1|30|
#### 2.1.5 Entradas
Ninguna
#### 2.1.6 Salidas 
30
#### Codigo 
```
void main(List<String> args) {
  int s = 0, c = 1;
  while (c <= 5) {
    s = s + c * 2;
    c = c + 1;
  }
  print("resultado de la suma de numeros pares:$s");
} //While
```










