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
### Ejercicio 1.1 Sumar los valores del 1 al 10 (while)
#### Analisis 1.1.2 
Se asigna una variable que inicia en 0 "s" y otra que inice en 1 "c" luego con una se asigna la condicion de termino y en la otra se almacena la suma.
#### 1.1.3 Diagrama de flujo de datos
![SumaWhile](https://user-images.githubusercontent.com/113397997/198421393-eae5b96a-3afb-4428-b267-5a8b45f820e3.png)
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
 ### Ejercicio 1.2 Suma de los numeros del 1 al 10 (Do while)
 #### 1.2.1 Analisis 
 Se asignan dos variables Suma y Cont inicializadas en 0 y 1 respectivamente, luego se inicia el proceso donde se le suman a las variables cont y +1 respectivamente, hasta que la condicion encontrada al final se cumpla
 #### 1.2.2 Diagrama de flujo de datos 
![SumaDoWhile](https://user-images.githubusercontent.com/113397997/198421584-c05dce79-f7d8-4cdc-bc7b-92fe6e59fa16.png)
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
### 2 Ejercicio Obtenga la suma de los 5 primeros numeros pares (for)
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
#### 2.1.1 Ejercicio Obtenga la suma de los 5 primeros numeros pares (While)
#### 2.1.2 Analisis
Se asigna una variable que inicia en 0 "s" y otra que inice en 1 "c" luego con una se asigna la condicion de termino y en la otra se almacena la suma del contador multiplicado por 2.
#### 2.1.3 Diagrama de flujo de datos 
![SumaParWhile](https://user-images.githubusercontent.com/113397997/198422269-276c7021-6c66-481c-b077-5c7321456f1f.png)
#### 2.1.4 Prueba de escritorio 
|s|c|c<=5|s=s+ i * 2|c++|salida|
|-|-|-|-|-|-|
|0|1|1<=5|0+ 1 * 2|1+1||
|2|2|2<=5|2+ 2 * 2|2+1||
|6|3|3<=5|6+ 3 * 2|3+1||
|12|4|4<=5|12+ 4 * 2|4+1||
|20|5|5<=5|20+ 5 * 2|5+1|3|
#### 2.1.5 Entradas
Ninguna
#### 2.1.6 Salidas 
30
#### 2.1.7 Codigo 
```
void main() {
  int s = 0, c = 1;
  while (c <= 5) {
    s = s + c * 2;
    c = c + 1;
  }
  print("resultado de la suma de numeros pares:$s");
} //While
```
### Ejercicio 2.2.1 Suma los primeros 5 numeros pares
#### 2.2.3 Analisis
Se crean dos variables con, sum y son iniciadas en 0, para despues crear sumarle 1 a con y a sum le agregamos con
hasta que la condicion que se encuentra al final se cumpla
#### 2.2.4 Diagrama de flujo de datos 
![Sumapardowhile](https://user-images.githubusercontent.com/113397997/198417061-fb07bc48-4878-432a-aa5c-5da60070d035.png)
DFD
#### 2.2.5 Prueba de escritorio 
|Sun|Con|Con<=5|pantalla|
|-|-|-|-|
|2|1|1<=5|  |
|6|2|2<=5|  |
|12|3|3<=5| |
|20|4|4<=5| |
|30|5|5<=5|30|
#### 2.2.6 Codigo
```
void main() {
  int s = 0, c = 1;

  do {
    s = s + c * 2;
    c = c + 1;
  } while (c <= 5);
  print("La suma de tus pares es:$s");
} //Do While
```
#### 2.2.7 Entradas
Ninguna
#### 2.2.8 
30
### Ejercicio 3 (for)
Almacene en un array el numero n leido del teclado 
#### 3.1 Analisis
Usando una lista se generan diez numeros 0, luego usando un ciclo for se recorren todas las posiciones de la lista
Se usa una entrada de teclado simple convirtiendo un String a Int y luego verificando que la entrada no sea null para luego asignarla a la posicion que genera el for.
#### 3.2 Diagrama de flujo de datos 
![SumaparDowhile](https://user-images.githubusercontent.com/113397997/198422521-72bae51f-eb4d-474e-bcdd-cd10619468b8.png)
DFD
#### 3.3 Prueba de escritorio 
|N|i|A[i]|A|
|-|-|-|-|
|4|0|A[0]||
|5|1|A[1]||
|7|2|A[2]||
|5|3|A[3]||
|5|4|A[4]||
|3|5|A[5]||
|3|6|A[6]||
|5|7|A[7]||
|1|8|A[8]||
|-8|9|A[9]|4,5,7,55,3,3,5,1,-8|
#### 3.4 Codigo 
```
import 'dart:io';

//Leer 10 numeros del teclado y ponerlos en una lista.
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  for (var i = 0; i <= 9; i++) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
    }
  }
  stdout.write("aqui esta la lista, $arra");
}
``` 
#### 3.5 Entradas 
4,5,7,5,5,3,3,5,1,-8
#### 3.6 Salidas 
4,5,7,5,5,3,3,5,1,-8
### 3.1.1 Ejercicio 
Almacene en un array el numero n leido del teclado (While)
#### 3.1.2 Analisis 
Se declara la variable i = 0, luego se entra en un ciclo while donde mientras se cumpla la conidicon i <= 9 el usuario ingresa un numero en el teclado, luego de la primera corrida i aumenta en 1. el ciclo se repite hasta que se tengan los 10 numeros del teclado
#### 3.1.3 Diagrama de flujo de datos 
![Array10while](https://user-images.githubusercontent.com/113397997/198423714-6929f933-afbc-4568-a3e8-edf5af4cae37.png)
DFD
#### 3.1.4 Prueba de escritorio 
|n|c|c<=9|A[c]=n|c++|pantalla|
|-|-|-|-|-|-|
|9|0|0<=9|A[0]=9|0+1||
|9|1|1<=9|A[1]=9|1+1||
|9|2|2<=9|A[2]=9|2+1||
|9|3|3<=9|A[3]=9|3+1||
|9|4|4<=9|A[4]=9|4+1||
|9|5|5<=9|A[5]=9|5+1||
|9|6|6<=9|A[6]=9|6+1||
|9|7|7<=9|A[7]=9|7+1||
|9|8|8<=9|A[8]=9|8+1||
|9|9|9<=9|A[9]=9|9+1|9,9,9,9,9,9,9,9,9,9|
#### 3.1.5 Codigo
```
import 'dart:io';

//Leer 10 numeros del teclado y ponerlos en una lista.
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  while (i <= 9) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int ner = int.parse(s);
      arra[i] = ner;
    }
    i++;
  }
  stdout.write("Tu lista es, $arra ");
}
```
#### 3.1.6 Entradas
9,9,9,9,9,9,9,9,9,9
#### 3.1.7 Salidas 
A[9,9,9,9,9,9,9,9,9,9]
###  3.2.1 Ejercicio
Almacene en un array el numero n leido del teclado 
#### 3.2.2 Analsis
Se abre un array de diez digitos, se declara una variable i que empieza en 0, luego se captura un numero N despues A de la posicion C=0 se declara como N y se agrega +1 a i, despues una condicion nos hace repetir el ciclo y capturar datos mientras c<=9, cuando la condicion se cumple se imprime el array.
#### 3.2.3 Diagrama de flujo de datos
![Array10Dowhile](https://user-images.githubusercontent.com/113397997/198505136-b4be42db-6fed-41b3-8fdf-f78f9c5576b5.png)
#### 3.2.4 Prueba de escritorio 
|n|i|A[i]=n|i++|i<=9|Pantalla|
|2|0|0<=9|0+1|A[0]=2||
|2|1|1<=9|1+1|A[1]=2||
|2|2|2<=9|2+1|A[2]=2||
|2|3|3<=9|3+1|A[3]=2||
|2|4|4<=9|4+1|A[4]=2||
|2|5|5<=9|5+1|A[5]=2||
|2|6|6<=9|6+1|A[6]=2||
|2|7|7<=9|7+1|A[7]=2||
|2|8|8<=9|8+1|A[8]=2||
|2|9|9<=9|9+1|A[9]=2|A[2,2,2,2,2,2,2,2,2,2]|
#### 3.2.5 Codigo

```
import 'dart:io';

void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  do {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
      i++;
    }
  } while (i <= 9);
  stdout.write("Tu lista es $arra ");
}
```

















