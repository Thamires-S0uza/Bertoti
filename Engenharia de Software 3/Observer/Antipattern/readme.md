      package antipattern;
      
      Corrida.java

      public class Corrida implements Cronômetro{

    	public void update(int state) {
	   	System.out.println("Corrida: " + Integer.toString(state));		
	     }

     }

<hr>

    Natacao.java

     package antipattern;

    public class Natacao implements Cronômetro  {

	   public void update(int state) {
	  	System.out.println("Natação: " + Integer.toString(state * 2));		
	   }
	
     }

<hr>
