import java.util.Scanner;

public class GanjilGenap {

    public static void main(String[] args) {
    
        Scanner input = new Scanner(System.in);

        System.out.println("=== Menentukan Bilangan Ganjil Genap === ");
        System.out.print("Masukkan sebuah angka: ");
        int angka = input.nextInt();
        
        if (angka % 2 == 0) {
            System.out.println(angka + " adalah bilangan genap.");
        } else {
            System.out.println(angka + " adalah bilangan ganjil.");
        }
        
        input.close();
    }
}


import java.util.Scanner;

public class MenentukanLulus {

    public static void main(String[] args) {
    
        Scanner scanner = new Scanner(System.in);
        System.out.println("=== Menentukan Lulus ===");

        System.out.print("Masukan nilai mahasiswa : " );
        double nilaiMahasiswa = scanner.nextDouble();

        String keterangan;

        if (nilaiMahasiswa >= 75) {
            keterangan = "Lulus";
        } else{
            keterangan = "Tidak Lulus";
        }
        
        System.out.println("Keterangan : " + keterangan);

        scanner.close();
    }
}


import java.util.Scanner;

public class MenentukanGrade {

    public static void main(String[] args) {
    
        Scanner scanner = new Scanner(System.in);
        System.out.println("===== Menentukan Grade =====");

        System.out.print("Masukan Nilai Mahasiswa :");
        double nilaiMahasiswa = scanner.nextDouble();

        String grade;

        if (nilaiMahasiswa >= 85) {
            grade = "A";
        } else if (nilaiMahasiswa >= 75){
            grade = "B";
        } else if (nilaiMahasiswa >= 65){
            grade = "C";
        } else if (nilaiMahasiswa >= 55){
            grade = "D";
        } else {
            grade = "E";
        }

        System.out.println("Grade Mahasiswa : " + grade);
        scanner.close();
    }
}


import java.util.Scanner;

public class PecahanUang {

    public static void main(String[] args) {
    
        Scanner scanner = new Scanner(System.in);
        System.out.println("=== Menghitung Pecahan uang === ");

        System.out.print("Masukkan jumlah uang: ");
        int jumlahUang = scanner.nextInt();

        int seratusRibu, limaPuluhRibu, duaPuluhRibu, sepuluhRibu, limaRibu, duaRibu, seribu, limaRatus, seratus;

        if (jumlahUang >= 100000) {
            seratusRibu = jumlahUang / 100000;
            jumlahUang = jumlahUang % 100000;
            System.out.println(seratusRibu + " lembar/keping 100000 rupiah");
        }

        if (jumlahUang >= 50000) {
            limaPuluhRibu = jumlahUang / 50000;
            jumlahUang = jumlahUang % 50000;
            System.out.println(limaPuluhRibu + " lembar/keping 50000 rupiah");
        }

        if (jumlahUang >= 20000) {
            duaPuluhRibu = jumlahUang / 20000;
            jumlahUang = jumlahUang % 20000;
            System.out.println(duaPuluhRibu + " lembar/keping 20000 rupiah");
        }

        if (jumlahUang >= 10000) {
            sepuluhRibu = jumlahUang / 10000;
            jumlahUang = jumlahUang % 10000;
            System.out.println(sepuluhRibu + " lembar/keping 10000 rupiah");
        }

        if (jumlahUang >= 5000) {
            limaRibu = jumlahUang / 5000;
            jumlahUang = jumlahUang % 5000;
            System.out.println(limaRibu + " lembar/keping 5000 rupiah");
        }

        if (jumlahUang >= 2000) {
            duaRibu = jumlahUang / 2000;
            jumlahUang = jumlahUang % 2000;
            System.out.println(duaRibu + " lembar/keping 2000 rupiah");
        }

        if (jumlahUang >= 1000) {
            seribu = jumlahUang / 1000;
            jumlahUang = jumlahUang % 1000;
            System.out.println(seribu + " lembar/keping 1000 rupiah");
        }

        if (jumlahUang >= 500) {
            limaRatus = jumlahUang / 500;
            jumlahUang = jumlahUang % 500;
            System.out.println(limaRatus + " lembar/keping 500 rupiah");
        }

        if (jumlahUang >= 100) {
            seratus = jumlahUang / 100;
            jumlahUang = jumlahUang % 100;
            System.out.println(seratus + " lembar/keping 100 rupiah");
        }

        scanner.close();
    }
}


import java.util.Scanner;

public class Jeruk {

    public static void main(String[] args) {
    
        Scanner scanner = new Scanner(System.in);
        System.out.println("=== Menghitung Harga Jeruk === ");

        System.out.print("Masukkan jumlah buah jeruk: ");
        int buah = scanner.nextInt();

        int harga_5 = 10000, harga_2 = 5000, harga_1 = 3000;
        int total = 0;

        if (buah >= 5) {
            int harga_buah_5 = (buah / 5) * harga_5;
            buah = buah % 5; 
            total += harga_buah_5;
        }

        if (buah >= 2) {
            int harga_buah_2 = (buah / 2) * harga_2;
            buah = buah % 2; 
            total += harga_buah_2;
        }

        if (buah >= 1) {
            int harga_buah_1 = buah * harga_1;
            total += harga_buah_1;
        }

        System.out.println("Total harga: " + total);
        scanner.close();
    }
}

