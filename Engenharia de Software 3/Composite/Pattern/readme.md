package pattern;

     public class Brigadeiro implements Produto {

     @Override
   
     public void comprar() {
         System.out.println("Comprando brigadeiro");
        
       }
       
     }

<hr>

    package pattern;

    public class Bolo implements Produto {
	   @Override
	   public void comprar() {
	   	System.out.println("Comprando bolo");
	       }
     }
   
   <hr>
   
      package pattern;

     import java.util.ArrayList;
     import java.util.List;

        public class Carrinho implements Produto {
	    	private List<Produto> produtos = new ArrayList<Produto>();
		
		    @Override
	    	public void Comprar() {
	   		for(Produto p: produto)
	   		{
	  			p.Comprar();
		  	}
	   		System.out.println("Compra realizada!");
		   	produtos.remover();
	    	}

	   	public void adicionar(Produto p){
			this.produtos.add(p);
		   }
		
	   	public void remover(Produto p){
	  		produtos.remover(p);
	  	}
