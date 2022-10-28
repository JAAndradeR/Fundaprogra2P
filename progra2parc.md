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
Almacene en un array el numero n leido del teclado (Do While)
#### 3.2.2 Analsis
Se abre un array de diez digitos, se declara una variable i que empieza en 0, luego se captura un numero N despues A de la posicion C=0 se declara como N y se agrega +1 a i, despues una condicion nos hace repetir el ciclo y capturar datos mientras c<=9, cuando la condicion se cumple se imprime el array.
#### 3.2.3 Diagrama de flujo de datos
![Array10Dowhile](https://user-images.githubusercontent.com/113397997/198505136-b4be42db-6fed-41b3-8fdf-f78f9c5576b5.png)
#### 3.2.4 Prueba de escritorio 
| n|i|A[i]=n|i++|i<=9|Pantalla|
|--|-|------|---|----|--------|
| 2|0|0<=9|0+1|A[0]=2|        |
| 2|1|1<=9|1+1|A[1]=2|        |
| 2|2|2<=9|2+1|A[2]=2|        |
| 2|3|3<=9|3+1|A[3]=2|        |
| 2|4|4<=9|4+1|A[4]=2|        |
| 2|5|5<=9|5+1|A[5]=2|        |
| 2|6|6<=9|6+1|A[6]=2|        |
| 2|7|7<=9|7+1|A[7]=2|        |
| 2| 8|8<=9|8+1|A[8]=2|        |
| 2| 9|9<=9|9+1|A[9]=2|2,2,2,2,2,2,2,2,2,2|
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
#### 3.2.6 Entradas 
2,2,2,2,2,2,2,2,2,2
#### 3.2.7 Salidas 
2,2,2,2,2,2,2,2,2,2
### Ejercicio 4
Almacene en un array un contador regresivo del 10 al 0 (For)
#### 4.1 Analisis abrir un array de 11 espacios, luego recorrerlos con un ciclo for que cuente del 11 hasta el 0 y almacenar los numeros obtenidos en el array 
![Regrefor](https://user-images.githubusercontent.com/113397997/198507960-38960c4b-3e9f-4e03-b765-d97d6c50ab52.png)
DFD
#### 4.2 Prueba de escritorio
|i|i>=0|A[10-i]=i|i--|pantalla
|-|-|-|-|-|
|10|10>=0|A[10-10]=0|10-1||
|9|9>=0|A[10-9]=1|9-1||
|8|8>=0|A[10-8]=2|8-1||
|7|7>=0|A[10-7]=3|7-1||
|6|6>=0|A[10-6]=4|6-1||
|5|5>=0|A[10-5]=5|5-1||
|4|4>=0|A[10-4]=6|4-1||
|3|3>=0|A[10-3]=7|3-1||
|2|2>=0|A[10-2]=8|2-1||
|1|1>=0|A[10-1]=9|1-1||
|0|0>=0|A[10-0]=10||10,9,8,7,6,5,4,3,2,1,0|
#### 4.3 Codigo 
```
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  for (var i = 10; i >= 0; i--) {
    arr[10 - i] = i;
  }
  print(arr);
}
```
#### 4.4 Entradas 
Ninguna
#### 4.5 Salidas 
10,9,8,7,6,5,4,3,2,1,0
### Ejercicio 4.1.1
Almacene en un array la ceunta regresiva del 10 al 0 (While)
#### Analisis 4.1.2
![RegreWhile](https://user-images.githubusercontent.com/113397997/198509548-2d84499a-4192-4d61-8cb9-847a3b6314c5.png)
DFD
#### 4.1.3 Prueba de escritorio 
|i|i>=0|A[10-i]=i|i--|pantalla
|-|-|-|-|-|
|10|10>=0|A[10-10]=0|10-1||
|9|9>=0|A[10-9]=1|9-1||
|8|8>=0|A[10-8]=2|8-1||
|7|7>=0|A[10-7]=3|7-1||
|6|6>=0|A[10-6]=4|6-1||
|5|5>=0|A[10-5]=5|5-1||
|4|4>=0|A[10-4]=6|4-1||
|3|3>=0|A[10-3]=7|3-1||
|2|2>=0|A[10-2]=8|2-1||
|1|1>=0|A[10-1]=9|1-1||
|0|0>=0|A[10-0]=10||10,9,8,7,6,5,4,3,2,1,0|
#### 4.1.4 Codigo 
```
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  while (c >= 0) {
    arr[10 - c] = c;
    c = c - 1;
  }
  print(arr);
} //dart
```
#### 4.1.5 Entradas
Ninguna 
#### 4.1.6 Salidas 
10,9,8,7,6,5,4,3,2,1,0
### Ejercicio 4.2.1 (Do While)
Almacene en un array la ceunta regresiva del 10 al 0
#### 4.1.2 Analisis 
Se abre un array de 11 espacios, luego se inicializa una variable i en 10, para despues con una condicion repetir i-1 y almacenarlo en A en reversa restandole a 10 i, que inicia en 10, y luego decrementar i hasta que llegue a 0 para que finalice el programa e imprimir A
#### 4.1.3 Diagrama de flujo de datos 
![RegreDoWhile](https://user-images.githubusercontent.com/113397997/198510533-d949b690-8e1d-4c10-b1e2-151254847d99.png)
DFD 
#### 4.1.4 Prueba de escritorio 
|i|A[10-i]=i|i--|i>=0|Pantalla|
|-|-|-|-|-|
|10|A[10-10]=0|10-1|10>=0||
|9|A[10-9]=1|9-1|9>=0||
|8|A[10-8]=2|8-1|8>=0||
|7|A[10-7]=3|7-1|7>=0||
|6|A[10-6]=4|6-1|6>=0||
|5|A[10-5]=5|5-1|5>=0||
|4|A[10-4]=6|4-1|4>=0||
|3|A[10-3]=7|3-1|3>=0||
|2|A[10-2]=8|2-1|2>=0||
|1|A[10-1]=9|1-1|1>=0||
|0|A[10-0]=10||0>=0|10,9,8,7,6,5,4,3,2,1,0|
#### 4.1.5 Codigo 
```
//dart
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  do {
    arr[10 - c] = c;
    c = c - 1;
  } while (c >= 0);
  print(arr);
}
```
#### 4.1.6 Entradas 
Ninguna 
#### 4.1.7 Salidas 
10,9,8,7,6,5,4,3,2,1,0
### Ejercicio 5 Almacene en un vector de tamaño 10, todos los numeros pares capturados hasta completar todos. (for)
#### 5.1 Analisis Se inicialia un array de 10 espacios, para luego recorrer todo el indice con un ciclo for, y con una entrada de teclado almacenarlos, discriminando los no pares.
#### 5.2 Diagrama de flujo de datos 
![ParesUsfor](https://user-images.githubusercontent.com/113397997/198512856-ca97d447-fe41-4760-af37-ae73445217ff.png)
#### 5.3 Prueba de escritorio 
|i|i<=9|n|n%2==0|A[i]=n|i+1|pantalla|
|-|-|-|-|-|-|-|
|0|0<=9|8|8%2==0|A[0]=8|0+1||
|1|1<=9|8|4%2==0|A[1]=8|1+1||
|2|2<=9|6|2%2==0|A[2]=6|2+1||
|3|3<=9|8|8%2==0|A[3]=8|3+1||
|4|4<=9|4|4%2==0|A[4]=4|4+1||
|5|5<=9|6|6%2==0|A[5]=6|5+1||
|6|6<=9|6|6%2==0|A[6]=6|6+1||
|7|7<=9|2|2%2==0|A[7]=2|7+1||
|8|8<=9|4|4%2==0|A[8]=4|8+1||
|9|9<=9|4|4%2==0|A[9]=4|9+1|8,8,6,8,4,6,6,2,4,4|
#### 5.4 Codigo 
```
numeros = [2, 4, 6, 8, 10, 12, 14, 16, 18, 20]
def extraer_pares(lista):
    pares = []
    for n in lista:
        if n % 2 == 0:
            pares.append(n)
    return pares
print()
resultado = extraer_pares(numeros)
print("Contenido de la variable`resultado`:", resultado)
print("Cantidad de elementos en la lista `resultado`:", len(resultado))
```
### Ejercicio 5.1.1 Almacene en un vector de tamaño 10, todos los numeros pares capturados hasta completar todos. (while)
#### 5.1.2 Analisis
Se inicializa un array en 10 para luego llenarlo dentro de un ciclo while, mientras la condicion i<=10 se cumpla, luego se llena de los numeros pares validados
#### 5.1.3 Diagrama de flujo de datos 
![ParesUsWhile](https://user-images.githubusercontent.com/113397997/198515434-5db101df-a879-491c-aaee-dea8a1e3846e.png)
#### 5.1.4 Prueba de escritorio 
|i|i<=9|N|n%2==0|A[i]=n|i+1|pantalla|
|-|-|-|-|-|-|-|
|0|0<=9|2|8%2==0|A[0]=2|0+1||
|1|1<=9|4|4%2==0|A[1]=4|1+1||
|2|2<=9|6|2%2==0|A[2]=6|2+1||
|3|3<=9|8|8%2==0|A[3]=8|3+1||
|4|4<=9|2|4%2==0|A[4]=2|4+1||
|5|5<=9|4|6%2==0|A[5]=4|5+1||
|6|6<=9|6|6%2==0|A[6]=6|6+1||
|7|7<=9|8|2%2==0|A[7]=8|7+1||
|8|8<=9|2|4%2==0|A[8]=2|8+1||
|9|9<=9|8|4%2==0|A[9]=8|9+1|2,4,6,8,2,4,6,8,2,8|
#### 5.1.5 Codigo
```
\\py
numeros = [2, 4, 6, 8, 10, 12, 14, 16, 18, 20]
def extraer_pares(lista):
    pares = []
    for n in lista:
        if n % 2 == 0:
            pares.append(n)
    return pares
print()
resultado = extraer_pares(numeros)
print("Contenido de la variable`resultado`:", resultado)
print("Cantidad de elementos en la lista `resultado`:", len(resultado))
```
#### 5.1.6 Entradas 
2,4,6,8,2,4,6,8,2,8
#### 5.1.7 Salidas 
2,4,6,8,2,4,6,8,2,8
### 5.2.1 Ejercicio Almacene en un vector de tamaño 10, todos los numeros pares capturados hasta completar todos. (Do While)
#### 5.2.2 Analisis 
Se inicializa un array en diez y una variable i en 0, luego con una entrada se valida que sea par, si lo es entonces se declara A[i] como n Y, se incrementa i en 1 y luego se dirige al ciclo que repite esta accion hasta que todos los espacios del array se hayan llenado, si el numero no es par manda un error que pide un numero par y el programa regresa a la entrada de datos 
#### 5.2.3 Diagrama de flujo de datos 
![ParUsDoWhile](https://user-images.githubusercontent.com/113397997/198517329-95a1d91d-290b-4682-bffd-565213c9bab6.png)
#### 5.2.4 Prueba de escritorio
|i|n|n%2==0|A[i]=n|i+1|i<=9|Pantalla|
|-|-|-|-|-|-||
|0|2|8%2==0|A[0]=2|0+1|0<=9||
|1|2|4%2==0|A[1]=2|1+1|1<=9||
|2|4|2%2==0|A[2]=4|2+1|2<=9||
|3|4|8%2==0|A[3]=4|3+1|3<=9||
|4|6|4%2==0|A[4]=6|4+1|4<=9||
|5|6|6%2==0|A[5]=6|5+1|5<=9||
|6|8|6%2==0|A[6]=8|6+1|6<=9||
|7|8|2%2==0|A[7]=8|7+1|7<=9||
|8|2|4%2==0|A[8]=2|8+1|8<=9||
|9|2|4%2==0|A[9]=2|9+1|9<=9|2,2,4,4,6,6,8,8,2,2|
#### 5.2.5 Codigo 
```dart
import 'dart:io';
import 'dart:async';
void main() {
  var array = [];
  var c = 0;
  do {
    int n = int.parse(stdin.readLineSync()!);
    if (n % 2 == 0) {
      array.add(n);
      c = c + 1;
    }
  } while (c <= 9);
  print(array);
}
```
#### 5.2.6 Entradas
2,2,4,4,6,6,8,8,2,2
#### 5.2.7 Salidas 
2,2,4,4,6,6,8,8,2,2
### Ejercicio 6 Obtener el promedio de las calificaciones aprobatorias y la cantidad de alumnos reprobados. La calificación entre 0 y 10 y el maximo de alumnos es de 15. (FOR)
#### 6.1 Analisis
Se ingresan las variables y se validan que esten dentro del rango, luego con un ciclo for se recorren todos lugares del indice y se asignan los valores de las variables para calificaciones y luego se clasifican como aprobatorias o reprobatorias con una condicion que revisa si son menores a 6
#### 6.2 Diagrama de flujo de datos 
![fofof](https://user-images.githubusercontent.com/113397997/198523739-10156bab-6d0a-4df6-87a3-0cf4ca2a5431.png)
6.3 Prueba de escritorio 
|C_Almn|C_Almn<=14|Cal|Cal>=LI|Cal<=LS|A[i]=Cal|i+1|Cal<5|S_A=S_A+Cal|C_A=C_A+1|C_R++|P_A=S_A/C_A|P_A|C_R|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|0|0<=14|6|6>=0|6<=10|A[0]=6|0+1|6<5|0+6|0+1|||||
|1|1<=14|6|6>=0|6<=10|A[1]=6|1+1|6<5|7+6|1+1|||||
|2|2<=14|2|2>=0|2<=10|A[2]=2|2+1||||0+1||||
|3|3<=14|4|4>=0|4<=10|A[3]=4|3+1||||1+1||||
|4|4<=14|9|9>=0|9<=10|A[4]=9|4+1|9<5|22+9|3+1|||||
|5|5<=14|10|10>=0|10<=10|A[5]=10|5+1|10<5|31+10|4+1|||||
|6|6<=14|5|5>=0|5<=10|A[6]=5|6+1||||1+1||||
|7|7<=14|3|3>=0|3<=10|A[7]=3|7+1||||2+1||||
|8|8<=14|8|8>=0|8<=10|A[8]=8|8+1|8<5|51+8|6+1|||||
|9|9<=14|7|7>=0|7<=10|A[9]=7|9+1|7<5|59+7|7+1|||||
|10|10<=14|9|9>=0|9<=10|A[10]=9|10+1|9<5|66+9|8+1|||||
|11|11<=14|4|4>=0|4<=10|A[11]=4|11+1||||2+1||||
|12|12<=14|10|10>=0|10<=10|A[12]=10|12+1|10<5|75+10|9+1|||||
|13|13<=14|9|9>=0|9<=10|A[13]=9|13+1|9<5|85+9|10+1|||||
|14|14<=14|8|8>=0|8<=10|A[14]=8|14+1|8<5|94+8|11+1||P_A=102/12|8.5|3|
#### 6.4 Codigo 
```
alumnos = list(range(15))
p_aprobados = 0
j = 0

for i in alumnos: 
    while(True):
        calificacion = int(input("Ingresa la calificación >>"))
        if (calificacion >= 0 and calificacion <= 10):
            break
        else:
            print("Calificación fuera de rango. Intenta de nuevo")
 
    if (calificacion < 6):
     alumnos[i] = "R"
    else:
     p_aprobados = calificacion + p_aprobados
     j = j + 1
     alumnos[i] = "A"

print("\033[33;1m",alumnos,"\033[39m")
print("El promedio de calificación de los aprobados es de >>",round(p_aprobados/j,2))
print("El total de aprobados fueron >> ",j)
print("El total de reprobados fueron >> ",(len(alumnos)-j))
```
#### 6.5 Entradas 
7,6,3,9,9,10,5,10,8,7,9,4,10,9,8
#### 6.6 Salidas 
El promedio de los aprobados 8.5 y la cantidad de reprobados 3
### 6.1.1 Ejercicio  Obtener el promedio de las calificaciones aprobatorias y la cantidad de alumnos reprobados. La calificación entre 0 y 10 y el maximo de alumnos es de 15. (While)
#### 6.1.2 Analisis 

















