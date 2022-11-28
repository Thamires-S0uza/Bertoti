    pagamento.java;

    package pattern;

    public class Pagamento {

     

     private Pagar pagar ;

     public void setPagar ( Pagar pagar ) {
                    this.pagar = pagar;

      }
      
     public void pagarConta () {
                    this.pagar.pagarConta();
      }

  <hr>

    pagarDebito.java
  
    package pattern

      public interface Pagar {

         public void pagarConta();

     } 
   <hr>      
      
     package pattern;

    public class pagarDebito implements Pagar{

        public void pagarConta() {
             System.out.println("Pagou conta no débito.");
        }
    }

   <hr>      
       
    pagarCredito.java

    package pattern;

        public class pagarCredito implements Pagar {

          public void pagarConta() {
                  System.out.pintln("Pagou conta no crédito.");

          }
        }
   <hr>      

    pagarPayPal.java

    package pattern;

    public class pagarPayPal implements Pagar {

      public void pagarConta() {

        System.out.println("Pagou conta no PayPal.");

     }
    }
