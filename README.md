package trabalho;

import javax.swing.*;

public class Questao_dois {
    public static void main(String[] args) {
        double bim_um = Double.parseDouble(JOptionPane.showInputDialog(null, "digite a nota1"));
        double bim_dois = Double.parseDouble(JOptionPane.showInputDialog(null, "digite a nota 2"));
        double bim_tres = Double.parseDouble(JOptionPane.showInputDialog(null, "digite a nota 3"));
        double bim_qua = Double.parseDouble(JOptionPane.showInputDialog(null, "digite a nota 4"));
        double soma = bim_um + bim_dois + bim_tres + bim_qua;
        int bimestres = 4;
        double media = soma / bimestres;
        JOptionPane.showMessageDialog(null, "sua média foi " + media);

        if (media<6.0){
            JOptionPane.showMessageDialog(null,"você nao foi aprovado");
            double A = Double.parseDouble(JOptionPane.showInputDialog(null,"digite sua nota na recuperação"));
            if (A>=6){
                JOptionPane.showMessageDialog(null,"você foi aprovado");
            }
            if (A<6){
                JOptionPane.showMessageDialog(null,"você foi reprovado");
            }
        }
        else {
            JOptionPane.showMessageDialog(null,"você foi aprovado");
        }







    }


}
