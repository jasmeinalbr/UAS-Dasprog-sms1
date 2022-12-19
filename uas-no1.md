# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Jasmein Al-baar Putri Rus'an
<br>NIM		: 1227050063
<br>Jurusan		: [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
  Array adalah sebuah variabel yang punya kemampuan untuk menyimpan lebih dari 1 nilai yang memiliki tipe yang sama. Atau dalam kata lain array adalah sekumpulan data dengan tipe data yang sama.
  Array 2 dimensi adalah array yang memiliki lebih 2 bentuk index array. Jika pada array 1 dimensi hanya memiliki satu bentuk index, di array 2 dimensi atau bisa kita sebut array multidimensi memiliki lebih dari satu bentuk index array. Jika di dalam array 1 dimensi hanya menggunakan sebuah tanda [] (bracket) namun pada array 2 dimensi kita membuat 2 tanda [] tersebut.
  Pada program ini dibuat untuk menginputkan angka untuk baris dan kolom pada matriks. Lalu program akan menampilkan matriks tersebut. Setelah tertampilkan maka program akan membuat matriks tersebut menjadi matriks transpose menggunakan looping.
  
## Source Code
#include <iostream>
using namespace std;

int main () {
	int i, j, m, n, matriks[10][10], transpose[10][10];

	cout << "Masukkan jumlah baris matriks : ";
	cin >> m;
	cout << "Masukkan jumlah kolom matriks : ";
	cin >> n;

	cout << endl << "Masukkan nilai matriks : \n";
    cout << "- spasi untuk kolom selanjutnya dan enter untuk baris selanjutnya - \n";
	for (i = 0; i < m; i++) {
		for (j = 0; j < n; j++) {
    		cin  >> matriks[i][j];
    	}
	}

	for (i = 0; i < m; i++) {
    	for (j = 0; j < n; j++) {
    		transpose[j][i] = matriks[i][j];
    	}
	}

	cout << "Hasil Transpose Matriks : \n";
	for (i = 0; i < n; i++) {
    	for (j = 0; j < m; j++) {
    	cout << transpose[i][j] << "\t";
    	}
    cout << endl;
	}
}
  
## Output
  ![WhatsApp Image 2022-12-19 at 15 57 19](https://user-images.githubusercontent.com/120997021/208386845-e6d56b9a-ddcf-4f8f-9175-76063968306d.jpeg)


  
