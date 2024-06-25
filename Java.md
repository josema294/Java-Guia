# Introducción a Java

Java es un lenguaje de programación de propósito general, concurrente, orientado a objetos y basado en clases. Fue diseñado para tener la menor cantidad de dependencias de implementación posibles, lo que lo hace ideal para aplicaciones que necesitan ser ejecutadas en múltiples plataformas.

## Sintaxis Básica de Java

### Tipos de Variables

En Java, existen varios tipos de variables que se pueden usar para almacenar datos. Estos se dividen en dos categorías principales: **tipos primitivos** y **tipos de referencia**.

#### Tipos Primitivos

1. **Enteros:**
   - `byte` (8 bits)
   - `short` (16 bits)
   - `int` (32 bits)
   - `long` (64 bits)

2. **Punto Flotante:**
   - `float` (32 bits)
   - `double` (64 bits)

3. **Caracteres:**
   - `char` (16 bits, basado en Unicode)

4. **Booleanos:**
   - `boolean` (true o false)

#### Tipos de Referencia

Estos incluyen cualquier instancia de una clase, arreglos, o interfaces.

### Estructuras de Control

Las estructuras de control en Java se utilizan para gestionar el flujo de ejecución del programa. Las más comunes son:

1. **Condicionales:**
   - `if`:
     ```java
     if (condición) {
         // Código a ejecutar si la condición es verdadera
     } else {
         // Código a ejecutar si la condición es falsa
     }
     ```


   - `switch`:
     ```java
     switch (variable) {
         case valor1:
             // Código a ejecutar si variable == valor1
             break;
         case valor2:
             // Código a ejecutar si variable == valor2
             break;
         default:
             // Código a ejecutar si ninguna de las condiciones anteriores se cumple
     }
     ```

	 `Operador Ternario`:

```java
variable = (condición) ? valorSiVerdadero : valorSiFalso;

```

2. **Bucles:**

- `for`:
```java
for (inicialización; condición; actualización) {
	// Código a ejecutar en cada iteración
 }
```

- `while`:
```java
while (condición) {
	// Código a ejecutar mientras la condición sea verdadera
}
```

- `do-while`:
```java
do {
	// Código a ejecutar al menos una vez y luego mientras la condición sea verdadera
} while (condición);
```

- `foreach`:
```java
int[] numeros = {1, 2, 3, 4, 5};
for (int numero : numeros) {
	System.out.println(numero);
}
	```
### Estructuras de Datos

Java proporciona varias estructuras de datos para almacenar y manipular conjuntos de datos.

1. **Arrays:** Los arrays en Java son estructuras de datos que almacenan una colección de elementos del mismo tipo.  Son inmutables
 
```java

// Declaración e inicialización de un arreglo de enteros
int[] numeros = {1, 2, 3, 4, 5}; // Acceso a elementos del arreglo
int primerNumero = numeros[0]; // 1
int segundoNumero = numeros[1]; // 2

```

 2. [[Colecciones]] (Lists)

Una lista es una colección ordenada que puede contener elementos duplicados. La implementación más común es `ArrayList`.

```java
`import java.util.ArrayList; import java.util.List;  // Creación de una ArrayList
List<String> nombres = new ArrayList<>();  // Agregar elementos a la lista 
nombres.add("Juan"); nombres.add("María"); nombres.add("Pedro");  // Acceso a elementos de la lista
String primerNombre = nombres.get(0); // "Juan"`
```
