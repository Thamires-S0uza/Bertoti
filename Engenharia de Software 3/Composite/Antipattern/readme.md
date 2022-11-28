 package antipattern;

    public class Brigadeiro {
	   public void buy() {
		  System.out.println("Comprando brigadeiro...");
    	}
    }
   
 <hr>   
 
      package antipattern;

      public class Bolo {
	      public void buy() {
	    	System.out.println("Comprando bolo...");
	   }
   }
    
  <hr>
  
     package antipattern;

     import java.util.ArrayList;
     import java.util.List;

     public class Sacola {
     private List<Bolo> bolos = new ArrayList<Bolo>();
	   private List<Brigadeiro> brigadeiros = new ArrayList<Brigadeiro>();
	
	   public void buy() {
	   	for(Bolo can: bolos)
		  {
		 	can.buy();
	    }
		   for(Brigadeiro cad: brigadeiros)
	   	{
			 cad.buy();
		    }
	    	System.out.println("Compra realizada!");
		     bolos.clear();
		     brigadeiros.clear();
     	}

	    public void addBolo(Bolo c){
	   	this.bolos.add(c);
	    }
	
	    public void addBrigadeiro(Brigadeiro c){
	   	this.brigadeiros.add(c);
	    }
	
	    public void removeBolo(Bolo c){
	   	bolos.remove(c);
     	}
	
	    public void removeBrigadeiro(Brigadeiro c){
		  brigadeiros.remove(c);
     	}
	
     }
