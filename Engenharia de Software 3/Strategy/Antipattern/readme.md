    comprar.java

    package antipattern;

    public class Pagar extends Compra

     public void realizarpagarDebito() {
            System.out.println("Realizou compra no débito...");
     }
    }

<hr> 

    package antipattern;

    public abstract class Compra {

       private void pagarCreditor() {
           System.out.println("Realizou compra no crédito...");
      }

    }

<hr> 

    package antipattern;

    public class Compra extends pagarCredito {

      public void pagarCreditor() {
          System.out.println("Realizou compra no crédito...");
      }
    }
    
    <hr> 
    
    package antipattern;

    public class Compra {

     public void pagarPayPal() {
     System.out.println("Realizou compra no PayPal...");

     }
    }
