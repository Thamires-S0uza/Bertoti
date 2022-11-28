     package pattern;

     public abstract class Observer {
	   protected Subject subject;
	    public abstract void update();

<hr>

        Corrida.java
       
        package pattern;

        public class Corrida extends Observer {
      	public Corrida (Subject subject){
	      this.subject = subject;
	      this.subject.anexar(this);
     	}

	     @Override
	   public void update() {
		System.out.println("Corrida: " + Integer.toString(subject.getState()));		
    
    
 <hr>
 
    Natacao.java
    
      package pattern;

        public class Natacao extends Observer {
	      public Natacao(Subject subject){
	      this.subject = subject;
	      this.subject.anexar(this);
	    }

	     @Override
	      public void update() {
		    System.out.println("Natação: " + Integer.toString(subject.getState() * 2));		
	     }    	
     }

<hr>
