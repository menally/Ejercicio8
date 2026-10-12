import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.print("Ingresa una cantidad grande de segundos (ej. 5000): ");

        int total = input.nextInt();
        //total:Guarda la cantidad de segundos//

        int r1 = total / 3600;
        //r1: Calcula las horas//

        int residuo = total % 3600;
        //residuo: Guarda los segundos que quedan después de calcular las horas//

        int r2 = residuo / 60;
        //r2: Calcula los minutos//

        int r3 = residuo % 60;
        //r3: Calcula los segundos restantes//

        System.out.println("Conversión final: " + r1 + "h : " + r2 + "m : " + r3 + "s");
        //println: Muestra la conversión//

        input.close();
    }
}
//El programa convierte una cantidad de segundos a horas,minutos y segundos//