Latihan 1
Cetak Nama

void main() {
  print("Hello, saya 'rifqy'");
}

Cetak nama dari input pengguna

void main() {
  stdout.write("Masukkan nama Anda: ");
  String? nama = stdin.readLineSync();
  print('Hello, saya "$nama"');
  print("Hello, saya '$nama'");
}

Konstanta integer

void main() {
  const int angka = 7;
  print("Nilai konstanta adalah $angka");
}

Menghitung bunga sederhana

import 'dart:io';

void main() {
  stdout.write("Masukkan pokok pinjaman: ");
  double p = double.parse(stdin.readLineSync()!);

  stdout.write("Masukkan waktu (tahun): ");
  double t = double.parse(stdin.readLineSync()!);

  stdout.write("Masukkan suku bunga (%): ");
  double r = double.parse(stdin.readLineSync()!);

  double bunga = (p * t * r) / 100;
  print("Bunga sederhana adalah $bunga");
}

Input bilangan bulat

import 'dart:io';

void main() {
  stdout.write("Masukkan bilangan bulat: ");
  int angka = int.parse(stdin.readLineSync()!);
  print("Angka yang dimasukkan: $angka");
}

Nama lengkap dari input

import 'dart:io';

void main() {
  stdout.write("Nama depan: ");
  String? depan = stdin.readLineSync();

  stdout.write("Nama belakang: ");
  String? belakang = stdin.readLineSync();

  print("Nama lengkap: $depan $belakang");
}

Hasil bagi dan sisa

import 'dart:io';

void main() {
  stdout.write("Masukkan bilangan pertama: ");
  int a = int.parse(stdin.readLineSync()!);

  stdout.write("Masukkan bilangan kedua: ");
  int b = int.parse(stdin.readLineSync()!);

  print("Hasil bagi: ${a ~/ b}"); // integer division
  print("Sisa bagi: ${a % b}");
}

Tukar dua bilangan

import 'dart:io';

void main() {
  stdout.write("Masukkan nilai a: ");
  int a = int.parse(stdin.readLineSync()!);

  stdout.write("Masukkan nilai b: ");
  int b = int.parse(stdin.readLineSync()!);

  print("Sebelum tukar: a=$a, b=$b");

  int temp = a;
  a = b;
  b = temp;

  print("Setelah tukar: a=$a, b=$b");
}

Hapus spasi dari String

import 'dart:io';

void main() {
  stdout.write("Masukkan kalimat: ");
  String? kalimat = stdin.readLineSync();
  String tanpaSpasi = kalimat!.replaceAll(' ', '');
  print("Tanpa spasi: $tanpaSpasi");
}

Ubah String ke int

import 'dart:io';

void main() {
  stdout.write("Masukkan angka: ");
  String? input = stdin.readLineSync();
  int angka = int.parse(input!);
  print("Hasil konversi: $angka");
}

Bagi tagihan
dart
Salin
Edit
import 'dart:io';

void main() {
  stdout.write("Masukkan jumlah tagihan: ");
  double tagihan = double.parse(stdin.readLineSync()!);

  stdout.write("Masukkan jumlah orang: ");
  int orang = int.parse(stdin.readLineSync()!);

  double perOrang = tagihan / orang;
  print("Setiap orang harus membayar: $perOrang");
}
 # dart-basic
