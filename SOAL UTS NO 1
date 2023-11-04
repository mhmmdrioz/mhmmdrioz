import java.util.Scanner;

class BiayaPercakapan {
    private int waktuAwal, waktuSelesai;

    public BiayaPercakapan(int jamAwal, int menitAwal, int detikAwal, int jamSelesai, int menitSelesai, int detikSelesai) {
        this.waktuAwal = jamAwal * 3600 + menitAwal * 60 + detikAwal;
        this.waktuSelesai = jamSelesai * 3600 + menitSelesai * 60 + detikSelesai;
    }

    public int hitungLamaPercakapan() {
        return waktuSelesai - waktuAwal;
    }

    public int hitungBiayaPercakapan() {
        int lamaPercakapanDetik = hitungLamaPercakapan();
        int biaya = (lamaPercakapanDetik * 150) / 5; // Biaya per detik * jumlah detik
        return biaya;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Masukkan jam percakapan dimulai: ");
        int jamAwal = input.nextInt();
        System.out.print("Masukkan menit percakapan dimulai: ");
        int menitAwal = input.nextInt();
        System.out.print("Masukkan detik percakapan dimulai: ");
        int detikAwal = input.nextInt();

        System.out.print("Masukkan jam percakapan selesai: ");
        int jamSelesai = input.nextInt();
        System.out.print("Masukkan menit percakapan selesai: ");
        int menitSelesai = input.nextInt();
        System.out.print("Masukkan detik percakapan selesai: ");
        int detikSelesai = input.nextInt();

        BiayaPercakapan percakapan = new BiayaPercakapan(jamAwal, menitAwal, detikAwal, jamSelesai, menitSelesai, detikSelesai);
        int biaya = percakapan.hitungBiayaPercakapan();
        int lamaPercakapan = percakapan.hitungLamaPercakapan();

        System.out.println("Lama percakapan: " + lamaPercakapan + " detik");
        System.out.println("Biaya percakapan: Rp" + biaya);
    }
}
