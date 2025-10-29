group 3 ict1n1
menu-driven system application using all java components 


import java.util.Scanner;

public class MenuDrivenSystem {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        showLoadingScreen();

        int choice;
        do {
            showMenu();
            choice = readInt(sc, "Enter your choice: ");

            switch (choice) {
                case 1:
                    calculator(sc);
                    break;
                case 2:
                    conversion(sc);
                    break;
                case 3:
                    oddEven(sc);
                    break;
                case 4:
                    circleCalculator(sc);
                    break;
                case 5:
                    aboutUs();
                    break;
                case 6:
                    System.out.println("\nExiting program...");
                   
        final String RESET = "\u001B[0m";
final String BROWN = "\u001B[33m";

System.out.println(BROWN + "                     ───▄▀▀▀▀▄▄▄▄▄▀▀▀▀▄───                          ");
System.out.println(BROWN + "                     ───█▒▒░░░░░░░░░▒▒█───                          ");
System.out.println(BROWN + "                     ────█░░█░░░░░█░░█────                          ");
System.out.println(BROWN + "                     ─▄▄──█░░░▀█▀░░░█──▄▄─                          ");
System.out.println(BROWN + "                     █░░█─▀▄░░░░░░░▄▀─█░░█                          ");
System.out.println("============================================================================");
System.out.println("   ████████╗██╗  ██╗ █████╗ ███╗   ██╗██╗  ██╗██╗   ██╗ ██████╗ ██╗   ██╗   ");
System.out.println("   ╚══██╔══╝██║  ██║██╔══██╗████╗  ██║██║ ██╔╝╚██╗ ██╔╝██╔═══██╗██║   ██║   ");
System.out.println("      ██║   ███████║███████║██╔██╗ ██║█████╔╝  ╚████╔╝ ██║   ██║██║   ██║   ");
System.out.println("      ██║   ██╔══██║██╔══██║██║╚██╗██║██╔═██╗   ╚██╔╝  ██║   ██║██║   ██║   ");
System.out.println("      ██║   ██║  ██║██║  ██║██║ ╚████║██║  ██╗   ██║   ╚██████╔╝╚██████╔╝   ");
System.out.println("      ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═══╝╚═╝  ╚═╝   ╚═╝    ╚═════╝  ╚═════╝    ");
System.out.println("============================================================================");
                   
                sleepSafe(1000);
                    break;
                default:
                    System.out.println("Invalid choice. Please try again.\n");
            }
        } while (choice != 6);

        sc.close();
    }

    // ===== Helper Methods =====
    private static void sleepSafe(long ms) {
        try {
            Thread.sleep(ms);
        } catch (InterruptedException ignored) {}
    }

    private static int readInt(Scanner sc, String prompt) {
        while (true) {
            System.out.print(prompt);
            String line = sc.nextLine().trim();
            try {
                return Integer.parseInt(line);
            } catch (NumberFormatException e) {
                System.out.println("Please enter a valid integer.");
            }
        }
    }

    private static double readDouble(Scanner sc, String prompt) {
        while (true) {
            System.out.print(prompt);
            String line = sc.nextLine().trim();
            try {
                return Double.parseDouble(line);
            } catch (NumberFormatException e) {
                System.out.println("Please enter a valid number.");
            }
        }
    }

    // ===== User Interface =====
    private static void showMenu() {
        System.out.println("\n=====================================");
        System.out.println("          MENU-DRIVEN SYSTEM");
        System.out.println("=======================================");
        System.out.println("[1] Calculator");
        System.out.println("[2] Conversion (mm, cm, m)");
        System.out.println("[3] Odd or Even");
        System.out.println("[4] Area and Circumference of Circle");
        System.out.println("[5] About Us");
        System.out.println("[6] Exit");
        System.out.println("=====================================\n");
    }

    private static void showLoadingScreen() {
        final String RESET = "\u001B[0m";
        final String BROWN = "\u001B[33m";

System.out.println("                     ───▄▀▀▀▄▄▄▄▄▄▄▀▀▀▄───                     ");
System.out.println("                     ───█▒▒░░░░░░░░░▒▒█───                     ");
System.out.println("                      ───█░░█░░░░░█░░█────                     ");
System.out.println("                     ─▄▄──█░░░▀█▀░░░█──▄▄─                     ");
System.out.println("                     █░░█─▀▄░░░░░░░▄▀─█░░█                     ");
System.out.println("===============================================================");   
System.out.println("=  ██╗      ██████╗  █████╗ ██████╗   ██╗███╗   ██╗ ██████╗   =");
System.out.println("=  ██║     ██╔═══██╗██╔══██╗██╔═══██╗ ██║████╗  ██║██╔════╝   =");
System.out.println("=  ██║     ██║   ██║███████║██║    ██║██║██