package tiendaMusica;

import java.util.Scanner;

public class FrerardInventario {

    public static void main(String[] args) {
        
        Scanner sc = new Scanner(System.in);
        
        // Nombre de la tienda
        System.out.println("=== Bienvenido a la Tienda de Música Frerard ===");
        System.out.println("Sistema básico de teoría de inventarios");

        String articulo;
        double K, D, H, Y;
        double Q, N, TCU;
        
        // Entrada de datos
        System.out.print("Ingrese el nombre del artículo o instrumento: ");
        articulo = sc.nextLine();
        
        System.out.print("Ingrese el costo por pedido: ");
        K = sc.nextDouble();
        
        System.out.print("Ingrese la demanda anual: ");
        D = sc.nextDouble();
        
        System.out.print("Ingrese el costo de almacenamiento por unidad: ");
        H = sc.nextDouble();
        
        System.out.print("Ingrese el costo de compra por unidad: ");
        Y = sc.nextDouble();

        
        
        
       

        
