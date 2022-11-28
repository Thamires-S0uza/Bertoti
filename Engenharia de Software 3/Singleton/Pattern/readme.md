       package pattern;

       public class App {

	      public static void main(String[] args) {
        BancoInter primeiroBanco = BancoInter.getInstance();
        
        /* AINDA A MESMA INSTÂNCIA DE bd */
        BancoInter novoBanco = BancoInter.getInstance();

	      }
       }
