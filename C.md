# Lenguaje c
###  ***Indice***
1. [Memoria en tiempo de Ejecucion](https://github.com/MatiaCornejo/cheat-sheets/blob/master/C.md#memoria-en-tiempo-de-ejecucion)
2. [Tipo de Datos](https://github.com/MatiaCornejo/cheat-sheets/blob/master/C.md#tipos-de-datos)
3. [Operadores](https://github.com/MatiaCornejo/cheat-sheets/blob/master/C.md#operadores)
4. [Arreglos](https://github.com/MatiaCornejo/cheat-sheets/blob/master/C.md#arreglos)
5.[Structs](#structs)
______
## Memoria en tiempo de Ejecucion
|Tipo|Caracteristica|
|:--:|:--|
|***_Stack_***|***Segmento de datos variables locales***, crece dinamicamente|
|***_Heap_***|***Segmento de memoria dinámica***,crece dinamicamente|
|***_Data_***|***Variables globales y estáticas***|
|***_Text_***|***Segmento de código*** código del programa compilado, es cargado a memoria cuando se ejecuta el programa|

## Tipos de Datos
|Tipo|Ej|calificadores|
|:--:|:--:|:--:|
|int|1| short, long, unsigned|
|float|1.1|
|double|1.1|
|char| c|

## Operadores
|Operador| Significado|
|:--:|:--|
|<|Menor que|
|<=|Menor o igual que|
|>|Mayor que|
|>=|Mayor o igual que|
|==|Igual que|
|!=|Distinto de|
|***Operadores Logicos***| ***Significado***|
|&&| and|
|!|not|
|II| or |

## Arreglos
* Almacenan conjunto de datos en memoria ***principal***.
* ***Todos*** los datos almacenados son del mismo tipo.
* Ej:
```c
int A[10];
//RESULTADO   |0|1|2|3|4|5|6|7|8|9| 
```
## Structs
* Conjunto de variables de uno o mas tipos bajo un *unico nombre*
```c
typedef struct{
  tipo1 x;
  tipo2 x;
} nombreStruct;
```
* Declaracion
```c
struct nombreStruct variable;
```
* Acceder a campos
```c
 nombreStruct.tipo1=<valor1>;
 nombreStruct->tipo2=<valor2>;
```
## Punteros
* Variable que almacena la direccion de otra variable.
* Declaracion
```C
 int* ptrint;
 float *ptrfloat;
 char *ptrchar;
 // etc...
```
### Aritmetica de Punteros
|***Operadores***| ***Significado***|
|:---:|:---:|
|++| Aumenta en 1 el la varible apuntada por ptr|
|--| Disminuye en 1 el la varible apuntada por ptr|
|=| Iguala el ptr a otro |
## Ciclos
### For
```c
for(contador;condicion;incremento){
	 //Codigo
}
```
### While
```c
while ( condicion )
{
 //Codigo
}
```
### DoWhile
```c
do {
  //Codigo
} while (condicion);
```
## Condiciones
### If-Else
```c
if (condicion){
  //Codigo
}
else{
  //Codigo
}
```
### Switch
```c
switch(int):
    case 1 :
        //Codigo
	break;
    case 2 :
        //Codigo
        break;
    case ... :
        //Codigo
	break;
    default :
        //Codigo
}
return 0;
```
## Archivos
* Secuencias de bytes para almacenar grandes volumenes de informacion

