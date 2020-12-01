# Evidencia-3-CJ

public interface principal {
    public void doctor();
    public void cita();
}

import java.util.Random;

public abstract class paciente implements principal{
    public void cita(){
        Random rand = new Random();
        int r = rand.nextInt(9999);
        System.out.println("El nombre del paciente es :");
        System.out.println("Numero unico del paciente: "+r);
        System.out.println("Enfermendad o sintoma: ");
    }

}


import java.util.Random;

public abstract class doctor implements principal{
    public void doctor(){
        Random rand = new Random();
        int r = rand.nextInt(9999);
        System.out.println("El nombre del doctor es Strange");
        System.out.println("ID:"+r);
    }

}


import java.util.Random;

public abstract class cita implements principal{
    public void cita(){
        Random rand = new Random();
        int r = rand.nextInt(999);
        System.out.println("La hora y dia de la citas es: ");
        System.out.println("Numero de la cita" + r);
    }

}
