# LinkedList
 La idea básica consiste en construir una lista cuyos elementos, llamados nodos, se componen de dos partes:  
 * la primera parte contiene la información y es un valor de un tipo genérico  
 * la segunda parte es una referencia o enlace que apunta al siguiente elemento de la lista.
 ![Texto alternativo]( https://sites.google.com/a/espe.edu.ec/programacion-ii/home/listas-enlazadas/lista.png?attredirects=0)
 ## ¿Cual es la diferencia entre LinkedList y ArrayList?
La principal diferencia de las listas enlazadas es que el orden de los elementos enlazados puede ser diferente al orden de almacenamiento.  
Una Linkedlist se puede usar como pila mientras que una ArrayList no.
 ![Texto alternativo](https://www.codenuclear.com/wp-content/uploads/2017/11/ArrayList_LinkedList.jpg)
## Algunos métodos usados de LinkedList
https://prezi.com/5k4gs1vdwz_s/metodos-de-linkedlist/
## Ejemplo de uso de LinkedList
```java
import java.util.ArrayList;
import java.util.Collection;
import java.util.LinkedList;

class Scratch {

  public static void main(String[] args) {
    LinkedList<String> listaEnlazada = new LinkedList<>();
    listaEnlazada.add("Kawasaki");
    listaEnlazada.add("Ducati");
    listaEnlazada.addFirst("Honda");
    listaEnlazada.addLast("KTM");
    // Tambien se pueden añadir otras colecciones
    Collection<String> coleccion = new ArrayList<String>();
    coleccion.add("1");
    coleccion.add("2");
    coleccion.add("3");
    coleccion.add("4");
    coleccion.add("5");
    listaEnlazada.addAll(coleccion);
    //Imprimiendo con foreach
    System.out.println("Lista Enlazada");
    for (String s : listaEnlazada) {
      System.out.println(s);
    }
  }
}
```
### Enlace al javadoc
https://docs.oracle.com/javase/8/docs/api/java/util/LinkedList.html
