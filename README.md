package com.mycompany.pratica1;
public class Pratica1 {
    public static void main(String[] args) {
       Perfume c1 = new Perfume();
       c1.modelo = "Gota de chuva!";
       c1.marca = "Natura!";
       c1.cor = "Amarelo";
       c1.tampar();
       c1.borrifar();
       c1.destampar();
       c1.borrifar();
       c1.status();
    }
}

package com.mycompany.pratica1;

public class Perfume {
    public String modelo;
    public String marca;
    public String cor;
    public boolean tampar;
    
    public void status(){
    System.out.println("Qual o modelo do perfume?\n" + this.modelo);
    System.out.println("Qual a marca do perfume?\n" + this.marca);
    System.out.println("Qual é a cor dele?\n" + this.cor);
    System.out.println("Ele está tampado?\n" + this.tampar);
   
    }
    public void borrifar(){
        if (this.tampar == true){
            System.out.println("Erro! O perfume está tampado.! ");
        } else {
            System.out.println("Borrifando perfume. .!");
        }
    }
    public void tampar(){
        this.tampar = true;
    }
    public void destampar(){
        this.tampar = false;
    }
}
        
