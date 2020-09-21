# Menjumlahkan setiap angka pada Nomor Handphone
Introduction to programming

    package com.ol.binus;
    import java.util.Scanner;

    public class Main {

        public static void main(String[] args) {
            Scanner input = new Scanner(System.in);
            System.out.print("Masukkan nomor handphone: ");

            // Deklarasi variable untk input nohp
            String digits = input.next();
            int i, j, jumlah = 0 ;  // Deklarasi variable
            for(i = 0; i < digits.length(); i++){
                j = i+1;
                jumlah = jumlah + Integer.parseInt(digits.substring(i,j));
                System.out.print(digits.substring(i,j) + "+" ); // cetak per-karakter dari nomor hp
            }
            System.out.print(" = Totalnya: " + jumlah); // jumlah keseluruhan dari nohp
        }
    }
