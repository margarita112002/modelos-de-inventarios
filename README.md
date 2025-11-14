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

        //modelo normal//
        Q_normal = Math.sqrt((2 * K * D) / H);
        N_normal = D / Q_normal;
        TCU_normal = (K * N_normal) + (H * (Q_normal / 2)) + (Y * D);

        // modelo con descuento// Aplicar descuento al precio unitario
        Y_desc = Y - (Y * (descuento / 100));
        
        Q_desc = Math.sqrt((2 * K * D) / H);
        N_desc = D / Q_desc;
        TCU_desc = (K * N_desc) + (H * (Q_desc / 2)) + (Y_desc * D);

         //mostrar mis resultados
         System.out.println("\n==== RESULTADOS ====");
         System.out.println("Artículo: " + articulo);
        
        System.out.println("\n--- Modelo Normal ---");
        System.out.printf("Cantidad óptima de pedido (Q): %.2f unidades\n", Q_normal);
        System.out.printf("Número de pedidos por año (N): %.2f\n", N_normal);
        System.out.printf("Costo total anual (TCU): $%.2f\n", TCU_normal);
        
        
        
        
