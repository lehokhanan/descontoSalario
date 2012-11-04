POO
import java.util.Scanner;
/**
 *
 * @author jpssantos
 */
public class descontoSalario {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
       
        double salBruto,salLiq;
        System.out.printf("Entre com o salario bruto(desprezando os centavos): ");
        Scanner input = new Scanner(System.in);
        
        salBruto = input.nextDouble();
        
        if (salBruto <= 1174){
        salLiq = salBruto - (salBruto*0.08);
        System.out.printf("Salario liquido = R$%f\n",salLiq);
        }
        if (salBruto > 1174 && salBruto <= 1637){
        salLiq = salBruto - (salBruto*0.09);
        System.out.printf("Salario liquido = R$%f\n",salLiq);
        }
        if (salBruto > 1637 && salBruto <= 1958){
        salLiq = salBruto - (salBruto*0.165);
        System.out.printf("Salario liquido = R$%f\n",salLiq);
        }
        if (salBruto > 1958 && salBruto <= 2453){
        salLiq = salBruto - (salBruto*0.185);
        System.out.printf("Salario liquido = R$%f\n",salLiq);
        }
        if (salBruto > 2453 && salBruto <= 3271){
        salLiq = salBruto - (salBruto*0.26);
        System.out.printf("Salario liquido = R$%f\n",salLiq);
        }
        
    }
}
