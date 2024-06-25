# Iteradores en Java

[[Java]] [[Iteradores]] 

## Resumen
Los iteradores en Java son una herramienta fundamental para recorrer colecciones de elementos de manera secuencial. Forman parte del marco de colecciones de Java y permiten iterar sobre listas, conjuntos, colas y otras estructuras de datos. La interfaz `Iterator` en el paquete `java.util` proporciona los métodos `hasNext()`, `next()`, y `remove()` para este propósito.
### Requisitos
Para usar un Iterador Para usar un iterador en Java, necesitas lo siguiente: 
1. **Importar el paquete `java.util`**: Asegúrate de importar `java.util.Iterator` y cualquier otra colección que planees utilizar. 
2. **Tener una colección que implemente `Iterable`**: La colección debe implementar la interfaz `Iterable`, que define el método `iterator()` y permite obtener un iterador para la colección.

## Métodos clave
- **hasNext()**: Este método devuelve `true` si hay más elementos en la colección al iterar, de lo contrario devuelve `false`. Permite verificar si se ha alcanzado el final de la colección.
- **next()**: Este método devuelve el siguiente elemento en la colección. Si no hay más elementos, lanza una `NoSuchElementException`. Es importante utilizar `hasNext()` antes de llamar a `next()` para evitar excepciones.
- **remove()**: Este método elimina el último elemento devuelto por el iterador de la colección subyacente. Solo puede ser llamado una vez por cada llamada a `next()` y lanza una `IllegalStateException` si se llama en un momento inapropiado.

## Ejemplo de uso
A continuación se muestra un ejemplo de cómo utilizar un iterador para recorrer una lista de elementos en Java:

```java
import java.util.ArrayList;
import java.util.Iterator;

public class IteradorEjemplo {
    public static void main(String[] args) {
        // Crear una lista de ejemplo
        ArrayList<String> lista = new ArrayList<>();
        lista.add("Elemento1");
        lista.add("Elemento2");
        lista.add("Elemento3");

        // Obtener el iterador
        Iterator<String> iterador = lista.iterator();

        // Usar el iterador para recorrer la lista
        while (iterador.hasNext()) {
            String elemento = iterador.next();
            System.out.println(elemento);
        }
    }
}
