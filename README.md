# Uso_GitFlow
  Ejemplo del uso de GitKraken
# POO (Programación Orientada a objetos)
  Ejemplo aplicando la Programación orientada a objetos en Java
##Ejemplo
Creamos una clase llamada **Telefono** la cual contiene dos caracteristicas principales:
 * Marca
 * Version
 
Esta clase va a presentar dos metodos **Constructores**
 * Constructor No.1 **Telefono**
  - Marca
  - Version
 * Constructor No.2 **Telefono**
 
El **Objeto Telefono** debe tener metodos especiales para realizar ciertas funciones tales como:
 * Llamar
 * infoTelefono

Al final nuestra clase **Telefono** queda de la siguiente manrea:

###Clase Telefono

```java
public class Telefono {

    private String marca,version;
    
    public Telefono(String marca,String version){
        this.marca = marca;
        this.version = version;
    }

    public Telefono(){}

    public void llamar(){
        System.out.println("Llamando de "+ marca +" Version: "+ version);
    }

    public void infoTelefono(Telefono telefono){
        System.out.println("-----------------------------------------------------------");
        System.out.println("Marca: " + telefono.marca + "\nVersión:  " + telefono.version );
        System.out.println("-----------------------------------------------------------");
    }
    
}
```

###Clase Main
```java
public class Main {

    public static void main(String[] args) {

        Telefono telefono1 = new Telefono("Samsung","J12 Prime"); //Declaracion de telefono1
        telefono1.llamar();

        Telefono telefono2 = new Telefono("Readmi"," 12C"); //Declaracion de telefono2
        telefono2.llamar();

        Telefono infoTelefono = new Telefono(); //Mostrando detalle de objeto telefono creado

        infoTelefono.infoTelefono(telefono2);
    }
}
