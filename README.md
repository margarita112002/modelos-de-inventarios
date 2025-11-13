package tiendaMusica;

import java.util.Scanner;

public class FrerardInventario {

    public static void main(String[] args) {
        
        Scanner sc = new Scanner(System.in);
        
        // Nombre de la tienda
        System.out.println("=== Bienvenido a la Tienda de Música Frerard ===");
        System.out.println("Sistema básico de teoría de inventarios");

       // Declarar variables
        String articulo;
        double K, D, H, Y, descuento;
        double Q_normal, N_normal, TCU_normal;
        double Q_desc, N_desc, TCU_desc, Y_desc;
        
        // Pedir datos al usuario
        System.out.print("Nombre del artículo o instrumento: ");
        articulo = sc.nextLine();
        System.out.print("Costo por pedido (K): ");
        K = sc.nextDouble();
        
        System.out.print("Demanda anual (D): ");
        D = sc.nextDouble();
        
        System.out.print("Costo de almacenamiento por unidad (H): ");
        H = sc.nextDouble();
        
        System.out.print("Costo de compra por unidad (Y): ");
        Y = sc.nextDouble();
        
        System.out.print("Descuento por cantidad (en %): ");
        descuento = sc.nextDouble();
        
        
        
