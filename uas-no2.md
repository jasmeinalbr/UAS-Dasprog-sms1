# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Jasmein Al-baar Putri Rus'an
<br>NIM		:	1227050063
<br>Jurusan		: [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
  Array adalah sebuah variabel yang punya kemampuan untuk menyimpan lebih dari 1 nilai yang memiliki tipe yang sama. Atau dalam 
kata lain array adalah sekumpulan data dengan tipe data yang sama.
  Array 2 dimensi adalah array yang memiliki lebih 2 bentuk index array. Jika pada array 1 dimensi hanya memiliki satu bentuk index, di array 2 dimensi 
atau bisa kita sebut array multidimensi memiliki lebih dari satu bentuk index array. Jika didalam array 1 dimensi hanya menggunakan sebuah 
tanda [] (bracket) namun pada array 2 dimensi kita membuat 2 tanda [] tersebut.
  Pada program ini dibuat untuk menginputkan angka lalu masuk ke dalam fungsi for dan if. Jika angka tersebut dapat dibagi 3 atau 5 atau 7
maka angkanya akan terlihat pada bagian output terakhir.

## Source Code
#include <iostream>
#include <iomanip>
using namespace std;

int main () {

    int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

    cout<<"Input jumlah baris : "; 
    cin >> jumlahBaris;
    cout<<"Input jumlah kolom : "; 
    cin >> jumlahKolom;
    cout << endl;

    for (i = 0; i < jumlahBaris; i++) {
        for(j = 0; j < jumlahKolom; j++) {
            cout << "Baris " << i+1 << ", kolom " << j+1 << " = ";
            cin >> arr[i][j];
        }
        cout << endl;
    }

   
    cout << "\nAngka yang habis dibagi 3 atau 5 atau 7 : " << endl;

    for (i = 0; i < jumlahBaris ; i++) {
        for (j = 0; j < jumlahKolom; j++) {
            if (arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0) {
            cout << setw(3) << arr[i][j] << " ";
            }
        }
    cout << endl;
    }

    cout << endl;
    return 0;
}

## Output
  ![WhatsApp Image 2022-12-19 at 16 07 26](https://user-images.githubusercontent.com/120997021/208388869-45ac8d41-bde3-4cff-8f9e-21e11ad0d32c.jpeg)
