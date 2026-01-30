# LabReport_3.1
package pack1;

public class Parent {
    protected int value = 10;

    protected void show() {
        System.out.println("Value: " + value);
    }
}
package pack1;

public class Child extends Parent {
    public void display() {
        // Accessing protected members directly
        System.out.println("Value from Parent: " + value);
        show();
    }

    public static void main(String[] args) {
        Child c = new Child();
        c.display();
    }
}
package pack1;

public class Parent {
    protected int value = 20;

    protected void show() {
        System.out.println("Value: " + value);
    }
}
package pack2;

import pack1.Parent;

public class Child extends Parent {
    public void display() {
        // Accessing protected members via inheritance
        System.out.println("Value from Parent: " + value);
        show();
    }

    public static void main(String[] args) {
        Child c = new Child();
        c.display();
    }
}
