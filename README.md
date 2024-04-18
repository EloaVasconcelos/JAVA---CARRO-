# JAVA---CARRO-


public class Carro {
	public String marca;
	public String modelo;
	public int veloatual;
	public double velomax;
	public boolean ligado;


public void ligar() {
	this.ligado = true;
	
	
}

public void desligar() {
	this.ligado = false;

}

public boolean acelerar (int aceleracao) {   
	if(ligado = true) {
		this.veloatual+=aceleracao;
	}
	
		if(veloatual <= velomax) {
			
		return true;
	}
	else { // JÁ ATENDE AS DUAS CONDIÇÕES - SE ESTIVER DESLIGADO A VELOCIDADE NÃO AUMENTA 
		return false;
	}
		
	if(ligado = false) {
		return false ; 
		
		}
	
			


public boolean frear (int frear) {
	
	this.veloatual -= velomax;
	if(veloatual > 0){
		return true;
		
	}
	else {
		return false;
	}
		
	}
}



	

	
	
