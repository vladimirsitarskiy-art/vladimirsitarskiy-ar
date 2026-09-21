import java.util.Scanner;

public class BasicTypesLab {
    public static void main(String[] args) {
        // Етап 1: Виведення меж та розмірів базових типів
        System.out.println("*** ХАРАКТЕРИСТИКИ ПРИМІТИВІВ У JAVA ***");
        
        System.out.println("\n--- Тип byte ---");
        System.out.println("Пам'ять: " + Byte.BYTES + " б / " + Byte.SIZE + " біт");
        System.out.println("Діапазон: від " + Byte.MIN_VALUE + " до " + Byte.MAX_VALUE);

        System.out.println("\n--- Тип short ---");
        System.out.println("Пам'ять: " + Short.BYTES + " б / " + Short.SIZE + " біт");
        System.out.println("Діапазон: від " + Short.MIN_VALUE + " до " + Short.MAX_VALUE);

        System.out.println("\n--- Тип int ---");
        System.out.println("Пам'ять: " + Integer.BYTES + " б / " + Integer.SIZE + " біт");
        System.out.println("Діапазон: від " + Integer.MIN_VALUE + " до " + Integer.MAX_VALUE);

        System.out.println("\n--- Тип long ---");
        System.out.println("Пам'ять: " + Long.BYTES + " б / " + Long.SIZE + " біт");
        System.out.println("Діапазон: від " + Long.MIN_VALUE + " до " + Long.MAX_VALUE);

        System.out.println("\n--- Тип float ---");
        System.out.println("Пам'ять: " + Float.BYTES + " б / " + Float.SIZE + " біт");
        System.out.println("Діапазон: від " + Float.MIN_VALUE + " до " + Float.MAX_VALUE);

        System.out.println("\n--- Тип double ---");
        System.out.println("Пам'ять: " + Double.BYTES + " б / " + Double.SIZE + " біт");
        System.out.println("Діапазон: від " + Double.MIN_VALUE + " до " + Double.MAX_VALUE);
        System.out.println("****************************************\n");

        // Етап 2: Робота з консольним введенням
        Scanner reader = new Scanner(System.in);
        System.out.println(">>> БЛОК ВВЕДЕННЯ ЗМІННИХ <<<");

        System.out.print("Задайте число типу byte (-128..127): ");
        String strB = reader.nextLine();
        byte valByte = Byte.parseByte(strB);
        System.out.println("-> Записано: " + valByte);

        System.out.print("Задайте число типу short: ");
        String strS = reader.nextLine();
        short valShort = Short.parseShort(strS);
        System.out.println("-> Записано: " + valShort);

        System.out.print("Задайте число типу int: ");
        String strI = reader.nextLine();
        int valInt = Integer.parseInt(strI);
        System.out.println("-> Записано: " + valInt);

        System.out.print("Задайте число типу long: ");
        String strL = reader.nextLine();
        long valLong = Long.parseLong(strL);
        System.out.println("-> Записано: " + valLong);

        System.out.print("Задайте дробове число float (через крапку): ");
        String strF = reader.nextLine();
        float valFloat = Float.parseFloat(strF);
        System.out.println("-> Записано: " + valFloat);

        System.out.print("Задайте дробове число double: ");
        String strD = reader.nextLine();
        double valDouble = Double.parseDouble(strD);
        System.out.println("-> Записано: " + valDouble);

        System.out.print("Задайте логічне значення (true/false): ");
        String strBool = reader.nextLine();
        boolean valBool = Boolean.parseBoolean(strBool);
        System.out.println("-> Записано: " + valBool);

        System.out.println("\n[!] Парсинг всіх типів завершено успішно.");
        
        reader.close();
    }
}