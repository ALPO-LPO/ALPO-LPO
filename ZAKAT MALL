package pertemuan.pkg3;

import java.util.Scanner;

public class Pertemuan3 {

    // Metode utama program
    public static void main(String[] args) {

        String ulangi;  // Variabel untuk menyimpan pilihan pengguna apakah ingin menghitung zakat lagi
        System.out.println("Selamat datang di Program Kalkulator Zakat Maal!");

        Scanner scanner = new Scanner(System.in);  // Membuat objek Scanner untuk membaca input dari pengguna

        do {
            System.out.print("Masukkan jumlah total harta yang Anda miliki (dalam Rupiah): ");

            // Memastikan input pengguna adalah angka
            while (!scanner.hasNextDouble()) {
                System.out.println("Oops! Input Anda tidak valid. Silakan masukkan jumlah harta berupa angka yang benar.");
                scanner.next();  // Mengabaikan input yang tidak valid
            }

            double harta = scanner.nextDouble();  // Menyimpan input jumlah harta
            scanner.nextLine();  // Membersihkan input buffer

            // Mengecek apakah jumlah harta sudah mencapai nisab
            if (harta >= 6859394) {
                double zakatMaal = harta * 0.025;  // Menghitung jumlah zakat maal (2,5%)
                System.out.printf("Anda wajib membayar zakat sebesar: Rp%.2f\n", zakatMaal);
            } else {
                System.out.println("Harta Anda belum mencapai nisab. Jadi, Anda belum wajib membayar zakat.");
            }

            // Menanyakan apakah pengguna ingin menghitung zakat lagi
            System.out.print("Apakah Anda ingin menghitung zakat lagi? (ketik 'ya' untuk melanjutkan, atau 'tidak' untuk keluar): ");
            ulangi = scanner.nextLine();  // Membaca pilihan pengguna

        } while (ulangi.equalsIgnoreCase("ya"));  // Mengulangi perhitungan jika pengguna memilih "ya"

        System.out.println("Terima kasih telah menggunakan Program Kalkulator Zakat Maal. Semoga bermanfaat!");
        scanner.close();  // Menutup Scanner untuk menghindari kebocoran sumber daya
    }
}
