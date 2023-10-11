# Patrones de diseño

## Singleton 

El patrón Singleton es un patrón de diseño creacional que asegura que una clase solo tenga una instancia. Esto se puede utilizar para garantizar que un recurso compartido, como una base de datos o un servicio, solo se acceda a través de un punto de acceso.

**Ejemplo:**

```java
public class Singleton {

    private static Singleton instance;

    private Singleton() {
        // Constructor privado para evitar la instanciación directa
    }

    public static Singleton getInstance() {
        if (instance == null) {
            instance = new Singleton();
        }
        return instance;
    }
}

```
**Ventajas:**

* Asegura que solo haya una instancia de una clase.
* Facilita el acceso a un recurso compartido.
* Puede mejorar el rendimiento al evitar la creación de instancias innecesarias.

**Desventajas:**

* Puede ser difícil de probar.
* Puede ser difícil de escalar.

## Template

El patrón Template es un patrón de diseño estructural que define un marco para una operación, dejando que las subclases implementen algunos o todos los pasos de la operación. Esto permite que las subclases compartan un código común, mientras que todavía pueden proporcionar una implementación específica para sus necesidades.

**Ejemplo:**

```java
public abstract class TemplateMethod {

    public void doSomething() {
        // Pasos comunes
        step1();
        step2();

        // Pasos específicos de la subclase
        step3();
    }

    protected abstract void step3();

    private void step1() {
        // Código común
    }

    private void step2() {
        // Código común
    }
}

public class ConcreteClass extends TemplateMethod {

    @Override
    protected void step3() {
        // Implementación específica del paso 3
    }
}

```
**Ventajas:**

* Reduce la duplicación de código.
* Facilita la extensión de clases.
* Puede mejorar la mantenibilidad del código.

**Desventajas:**

* Puede ser difícil de probar.
* Puede ser difícil de escalar.

## Strategy

El patrón Strategy es un patrón de diseño comportamental que permite que un algoritmo se intercambie de forma independiente de los clientes que lo usan. Esto permite que los clientes cambien el comportamiento de un sistema sin modificar el código del cliente.

**Ejemplo:**

```java
public interface Strategy {

    void doSomething();
}

public class ConcreteStrategy1 implements Strategy {

    @Override
    public void doSomething() {
        // Implementación del algoritmo 1
    }
}

public class ConcreteStrategy2 implements Strategy {

    @Override
    public void doSomething() {
        // Implementación del algoritmo 2
    }
}

public class Context {

    private Strategy strategy;

    public Context(Strategy strategy) {
        this.strategy = strategy;
    }

    public void doSomething() {
        strategy.doSomething();
    }
}
```

**Ventajas:**

* Permite que los clientes cambien el comportamiento de un sistema sin modificar el código del cliente.
* Puede mejorar la flexibilidad y la adaptabilidad de un sistema.
* Puede facilitar la prueba de un sistema.

**Desventajas:**

* Puede ser difícil de implementar correctamente.
* Puede ser difícil de escalar.
