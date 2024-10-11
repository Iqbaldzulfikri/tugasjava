import java.util.Scanner;

public class No1 {
    public static void main(String[] args) throws Exception {
        Scanner inputan = new Scanner(System.in);
        System.out.print("Masukkan angka: ");
        int angka = inputan.nextInt();
        if (angka % 2 == 0) {
            System.out.println("Genap");
        } else {
            System.out.println("Ganjil");
        }
        inputan.close();
    }
    }

    
import java.util.Scanner;

public class No2dan3 {
    public static void main(String[] args) {
        Scanner inputan = new Scanner(System.in);
        System.out.print("Masukkan nilai anda: ");
        int nilai = inputan.nextInt();
        if (nilai > 75) {
            System.out.print("Selamat Anda Lulus");
        } else {
            System.out.print("Maaf Anda Tidak Lulus");
        }
        if (nilai > 85) {
            System.out.print(" Dengan Predikat A (" +nilai+ ")" );
        } else if (nilai > 75 && nilai < 85) {
            System.out.print(" Dengan Predikat B (" +nilai+ ")");
        } else if (nilai > 65 && nilai < 75) {
            System.out.print(" Dengan Predikat C (" +nilai+ ")");
        } else if (nilai > 55 && nilai < 65) {
            System.out.print(" Dengan Predikat D (" +nilai+ ")");
        } else {
            System.out.print(" Dengan Predikat E (" +nilai+ ")");
        }
        inputan.close();
    }
}


import java.util.Scanner;

public class No4 {
    public static void main(String[] args) {
        Scanner inputan = new Scanner(System.in);
        int jumlah;
        int sisa, seratusRibu, limaPuluhRibu, duaPuluhRibu, sepuluhRibu, limaRibu,duaRibu ,seribu , limaRatus, seratus;
       
        System.out.print("Masukan Jumlah Uang : ");
        jumlah = inputan.nextInt();
        
        seratusRibu = (int)(jumlah / 100000);
        sisa = (int)(jumlah % 100000);
        limaPuluhRibu = (sisa / 50000);
        sisa = sisa % 50000;
        duaPuluhRibu = (sisa / 20000);
        sisa = sisa % 20000;
        sepuluhRibu = (sisa / 10000);
        sisa = sisa % 10000;
        limaRibu = (sisa / 5000);
        sisa = sisa % 5000;
        duaRibu = (sisa / 2000);
        sisa = sisa % 2000;
        seribu = (sisa / 1000);
        sisa = sisa % 1000;
        limaRatus = (sisa / 500);
        sisa = sisa % 500;
        seratus = (sisa / 100);
        System.out.println("Jumlah Uang = " + jumlah);
        if (seratusRibu > 0) System.out.println(seratusRibu + " lembar 100 Ribuan");
        if (limaPuluhRibu > 0) System.out.println(limaPuluhRibu + " lembar 50 Ribuan");
        if (duaPuluhRibu > 0) System.out.println(duaPuluhRibu + " lembar 20 Ribuan");
        if (sepuluhRibu > 0) System.out.println(sepuluhRibu + " lembar 10 Ribuan");
        if (limaRibu > 0) System.out.println(limaRibu + " lembar 5 Ribuan");
        if (duaRibu > 0) System.out.println(duaRibu + " lembar 2 Ribuan");
        if (seribu > 0) System.out.println(seribu + " lembar 1 Ribuan");
        if (limaRatus > 0) System.out.println(limaRatus + " logam 500");
        if (seratus > 0) System.out.println(seratus + " logam 100");
        // jika menggunakan else if maka sisa dari pembagian sebeleumnya tidak berjalan
        inputan.close();
    }
}


import java.util.Scanner;

public class No5 {
    public static void main(String[] args) {
        Scanner inputan = new Scanner(System.in);
        System.out.print("Masukkan jumlah jeruk : ");
        int totalJeruk = inputan.nextInt();
        if (totalJeruk == 1) {
            System.out.println( "Beli " +totalJeruk + " = 3000");
        } else if (totalJeruk == 2) {
            System.out.println( "Beli " +totalJeruk + " = 5000");
        } else if (totalJeruk == 5) {
            System.out.println( "Beli " +totalJeruk + " = 10000");
        } else {
            int harga = (totalJeruk / 5) * 10000 + (totalJeruk % 5) * 3000;
            System.out.println( "Beli " +totalJeruk + " = " + harga );
        }
        inputan.close();
    }
}

