# actividad2_punto9_poo
package departamentos;
import java.util.Scanner;
public class DEPARTAMENTOS {

    public static void main(String[] args) {
        double  vd1,vd2,vd3,salar,totven,porven,salar1,salar2,salar3;
        
        Scanner ingresotecl = new Scanner (System.in);
       
        System.out.println("Ingrese las ventas del `departamento 1: ");
        vd1 = ingresotecl.nextDouble();
        
        System.out.println("Ingrese las ventas del `departamento 2: ");
        vd2 = ingresotecl.nextDouble();
        
        System.out.println("Ingrese las ventas del `departamento 3: ");
        vd3 = ingresotecl.nextDouble();
        
        System.out.println("Ingrese los salarios que reciben los vendedores: ");
        salar = ingresotecl.nextDouble();
        
        totven=vd1+vd2+vd3;
        porven=0.33*totven;
        if (vd1>porven){
            salar1=salar+(0.2*salar);
        }
        else{
            salar1=salar;
        }
        
       if (vd2>porven){
           salar2=salar+(0.2*salar);
       }
       else{
           salar2=salar;
       }
       if (vd3>porven){
          salar3=salar+(0.2*salar); 
       }
       else{
           salar3=salar;
       }
       
       System.out.println("SALARIO VENDEDORES DEPTO. 1: "+ salar1 +" SALARIO VENDEDORES DEPTO. 2: "+ salar2 +" SALARIO VENDEDORES DEPTO. 3: "+ salar3);
        
        
    }
    
}
