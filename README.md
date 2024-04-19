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




## CÓDIGO ARRUMADO (TENTATIVA)

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

	    
     /*Pensamento: Faz o calculo e verifica se a velocidade atual+aceleração vai passar ou nao da velocidade permitida, se for menor ai sim o vai ser somado e retornar true */

    public boolean acelerar(int aceleracao) {
        if (ligado = true) {
            if ((veloatual + aceleracao) <= velomax) { 
                this.veloatual += aceleracao; 
                return true;
		
            } else {
                return false;
            }

// Outro metodo 

    public boolean frear(int frear) {
    if ((veloatual - frear) > 0 ) {
        this.veloatual -= frear; // Se não for negativa ai sim pode fazer o calculo, retornando true
            return true;
	    
        } else {
            this.veloatual = 0;  se for igual a zero, retorna falso   
            return false;
        }
    }
}



-- TESTES -- 


public class Principal {
	public static void main(String[]args) {
		Carro c1 = new Carro();
		
		c1.veloAtual = 30;
		c1.veloMax = 350;
		
		
		
	 /*Testando o metodo frear */ 
                c1( 
		System.out.println("A velocidade atual é: " + c1.veloAtual + " de uma velocidade maxima permitida de: " + c1.veloMax + "\nSua aceleração foi: " + retorno);
		System.out.println("-------------------------------------------------------------------------------------------");
		
		retorno = c1.acelerar(350);
		System.out.println("Não foi possivel acelerar, pois o retorno: " + retorno);
		System.out.println("-------------------------------------------------------------------------------------------");
		
		retorno = c1.acelerar(170);
		System.out.println("A velocidade atual é: " + c1.veloAtual + " de uma velocidade maxima permitida de: " + c1.veloMax + "\nSua aceleração foi: " + retorno);
		System.out.println("-------------------------------------------------------------------------------------------");


  /*Testando o metodo frear */ 
		boolean retornof = c1.freiar(200);
		System.out.println("A velocidade atual é: " + c1.veloAtual +  "\nSua desaceleração foi: " + retornof);
		System.out.println("-------------------------------------------------------------------------------------------");
		
		retornof = c1.freiar(200);
		System.out.println("A velocidade atual é: " + c1.veloAtual +  "\nSua desaceleração foi: " + retornof);
		System.out.println("-------------------------------------------------------------------------------------------");
	}
	
}

