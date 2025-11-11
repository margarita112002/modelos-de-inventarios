package tiendaMusica;

import java.util.Scanner;

public class FrerardInventario {

    public static void main(String[] args) {
        
        Scanner sc = new Scanner(System.in);
        
        // Nombre de la tienda
        System.out.println("=== Bienvenido a la Tienda de Música Frerard ===");
        System.out.println("Sistema básico de teoría de inventarios");

        String articulo;
        int demandaAnual;
        double costoPedido, costoAlmacenamiento, costoUnitario;
        double cantidadOptima, puntoReorden, tcu;
        int tiempoEntrega;

        // Pedir datos al usuario
        System.out.print("Nombre del artículo o instrumento: ");
        articulo = sc.nextLine();
        
        System.out.print("Cantidad actual en inventario: ");
        stock = sc.nextInt();
        
        System.out.print("Demanda mensual del producto (cuántos se venden al mes): ");
        demandaMensual = sc.nextInt();

       

        
