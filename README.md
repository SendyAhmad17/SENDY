# Ujian Akhir Semester 
<br>Mata Kuliah 	:DASAR PEMROGRAMAN
<br> Nama		:SENDI AHMAD RAFIUDIN
<br>NIM		:	1227050121
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
program yang saya buat menjelaskan tentang program matrix dua dimensi yang menjalankan program membuat sebuah kolom dan dengan barisnya. dan untuk yang nomor dua menjelaskan tentang array dua dimensi yang mana angka angkanya menampilkan bilangan yang habis dibagi 3,5,7.

## Source Code
    #include <iostream>
    #include <iomanip>

    using namespace std;

    int main()
    {
      cout << "##  PROGRAM C++ INPUT MATRIX DUA DIMENSI ##" << endl;
      cout << "==========================================" << endl;
      cout << endl;

      int matriks[100][100], tranfous[100][100];
      int jum_baris, jum_kolom, i, j, n, m;

      cout << "Input jumlah baris matriks: ";
      cin >> jum_baris;

      cout << "Input jumlah kolom matriks: ";
      cin >> jum_kolom;
      cout << endl;

      // proses input array
      for(i = 0; i < jum_baris ; i++){
        for(j = 0; j < jum_kolom; j++){
          cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
          cin >> matriks[i][j];
        }
        cout << endl;
      }

      cout << "Hasil matriks: " << endl;

      // menampilkan array
      for(i = 0; i < jum_baris ; i++){
        for(j = 0; j < jum_kolom; j++){
          cout << setw(3) << matriks[i][j] << " ";
        }
        cout << endl;
      }
      for(i = 0; i < jum_baris ; i++){
        for(j = 0; j < jum_kolom; j++){
          tranfous [j][i]=matriks[i][j];
        }
        cout << endl;
      }
      for(i = 0; i < jum_baris ; i++){
        for(j = 0; j < jum_kolom; j++){
          cout << tranfous [j][i];
        }
        cout << endl;
      }

     cout << "No.2 Menampilkan bilangan yang habis dibagi 3, 5 dan 7" << endl;
      cout << "==============================================================="<<endl;
      cout << "input jumlah baris matriks: ";
      cin >> m;
      cout << "input4";
      cout<<"4 jumlah kolom matriks: ";
      cin >> n;

      cout << "Masukkan Nilai-Nilai\n";
      for (int i = 0; i < m; i++)
      {
          for (int j = 0; j < n; j++)
        {
            cout <<"("<<i+1<<","<<j+1<<") : ";
          cin  >> matriks[i][j];
        }
      }
      cout << endl;

      bool cek = true;
      cout << "Nilai yang bisa dibagi 3, 5, 7 yaitu :";
      for (int i = 0; i < m; i++)
      {
        for (int j = 0; j < n; j++)
        {
          if (matriks[i][j]%3==0 && matriks[i][j]%5==0 && matriks[i][j]%7==0)
          {
            cout << " " << matriks[i][j];
            cout << endl;
            cek = false;
          }
        }
      }
      if (cek)
      {
        cout << " Maaf nilai yang anda input tidak dapat dibagi 3, 5 dan 7" <<endl;
      }

      return 0;
    }

## Output
![image](https://user-images.githubusercontent.com/119504590/209554109-9ce3c248-8c1f-4b28-af16-51b1180fa5e0.png)
![image](https://user-images.githubusercontent.com/119504590/209554350-30a1e2c0-7f8d-4ae4-b9a9-bfb95bab6222.png)


