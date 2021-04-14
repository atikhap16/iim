package modul2;

import java.util.Scanner;

class CD {
    String judul;
    String aktor;
    String sutradara;
    String publisher;
    int film;
    String stok;
    String lagi;

}

public class Main {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        CD VCD = new CD();

        System.out.println("===================================================================");
        System.out.println("                         Rental VCD                                ");
        System.out.println("===================================================================");
        int pilih = 1;
        while (pilih==1) {

            System.out.println("Judul               : ");
            VCD.judul = input.nextLine();

            System.out.println("Aktor               : ");
            VCD.aktor = input.nextLine();

            System.out.println("Sutradara           : ");
            VCD.sutradara = input.nextLine();

            System.out.println("Publisher                : ");
            VCD.publisher = input.nextLine();

            System.out.println("Stok                     : ");
            VCD.stok = input.nextLine();

            System.out.println("Kategori                 : ");
            System.out.println("1. Semua Umur");
            System.out.println("2. Dewasa");
            System.out.println("3. Remaja");
            System.out.println("4. Anak-anak");
            System.out.println("Masukkan Pilihan         : ");
            VCD.film = input.nextInt();

            System.out.println("===================================================================");
            System.out.println("                        DAFTAR FILM                                ");
            System.out.println("===================================================================");

            System.out.println("Judul Film                  : " + VCD.judul);
            System.out.println("Aktor                       : " + VCD.aktor);
            System.out.println("Sutradara                   : " + VCD.sutradara);
            System.out.println("Publisher                   : " + VCD.publisher);
            switch (VCD.film) {
            case 1:
                System.out.println("Kategori                    : Semua Umur (SU)");
                break;
            case 2:
                System.out.println("Kategori                    : Dewasa (D)");
                break;
            case 3:
                System.out.println("Kategori                    : Remaja (R)");
                break;
            case 4:
                System.out.println("Kategori                    : Anak-anak (AA)");
                break;

            }
            System.out.println("Stok                        : " + VCD.stok);

            System.out.println("Lakukan Lagi? : ( 1 untuk Ya dan 0 untuk Tidak )");
            pilih=input.nextInt();
            if(pilih!=1){
              pilih=0;
            }

        }

    }

}
