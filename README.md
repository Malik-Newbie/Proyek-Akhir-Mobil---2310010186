# Proyek-Akhir-Mobil---2310010186

##DESKRIPSi
Aplikasi ini menerima input berupa nama dan kode mobil, dan memberikan output berupa informasi dari mobil tersebut seperti nama mobil, tahun produksi, dan dari mana mobil tersebut diproduksi.
Aplikasi ini mengimplementasikan beberapa konsep penting dalam pemrograman berorientasi objek (OOP) seperti Class, Object, Atribut, Method Constructor, Method Mutator, Method Accessor, Encapsulation, Inheritance, Overloading, Overriding, Seleksi, Perulangan, IO Sederhana, Array, dan Error Handling.

##Penjelasan Koding
1. **Class** adalah template atau blueprint dari object. Pada kode ini, `Mobil`, `MobilDetail`, dan `MobilBeraksi` adalah contoh dari class.

```bash
public class Mobil {
    ...
}

public class MobilDetail extends Mobil {
    ...
}

public class MahasiswaBeraksi {
    ...
}

2. **Object** adalah instance dari class. Pada kode ini, `mbl[i] = new MobilDetail(nama1, kode1);` adalah contoh pembuatan object.

```bash
mbl[i] = new MobilDetail(nama1, kode1);
```

3. **Atribut** adalah variabel yang ada dalam class. Pada kode ini, `nama` dan `kode` adalah contoh atribut.

```bash
String nama;
String kode;
```

4. **Constructor** adalah method yang pertama kali dijalankan pada saat pembuatan object. Pada kode ini, constructor ada di dalam class `Mobil` dan `MobilDetail`.

```bash
public Mobil(String nama, String kode) {
    this.nama = nama;
    this.npm = kode;
}

public MobilDetail(String nama, String npm) {
    super(nama, kode);
}
```

5. **Mutator** atau setter digunakan untuk mengubah nilai dari suatu atribut. Pada kode ini, `setNama` dan `setKode` adalah contoh method mutator.

```bash
public void setNama(String nama) {
    this.nama = nama;
}

public void setNpm(String kode) {
    this.kode = kode;
}
```

6. **Accessor** atau getter digunakan untuk mengambil nilai dari suatu atribut. Pada kode ini, `getNama`, `getKode` adalah contoh method accessor.

```bash
public String getNama() {
    return nama;
}

public String getKode() {
    return kode;
}
```

7. **Encapsulation** adalah konsep menyembunyikan data dengan membuat atribut menjadi private dan hanya bisa diakses melalui method. Pada kode ini, atribut `nama` dan `kode` dienkapsulasi dan hanya bisa diakses melalui method getter dan setter.

```bash
private String nama;
private String kode;
```

8. **Inheritance** adalah konsep di mana sebuah class bisa mewarisi property dan method dari class lain. Pada kode ini, `MobilDetail` mewarisi `Mobil` dengan sintaks `extends`.

```bash
public class MobilDetail extends Mobil {
    ...
}
```

9. **Polymorphism** adalah konsep di mana sebuah nama dapat digunakan untuk merujuk ke beberapa tipe atau bentuk objek berbeda. Ini memungkinkan metode-metode dengan nama yang sama untuk berperilaku berbeda tergantung pada tipe objek yang mereka manipulasi, polymorphism bisa berbentuk Overloading ataupun Overriding. Pada kode ini, method `displayInfo(String)` di `Mahasiswa` merupakan overloading method `displayInfo` dan `displayInfo` di `MahasiswaDetail` merupakan override dari method `displayInfo` di `Mahasiswa`.

```bash
public String displayInfo() {
    return "Nama: " + getNama() + "\nKode: " + getKode();
}

@Override
public String displayInfo() {
    ...
}
```

10. **Seleksi** adalah statement kontrol yang digunakan untuk membuat keputusan berdasarkan kondisi. Pada kode ini, digunakan seleksi `if else` dalam method `getNegaraProduksi`.

```bash
if (kodeNegaraProduksi.equals("1")) {
            return "Jepang";
        } if (kodeNegaraProduksi.equals("2")){
            return "AMERIKA";
        }else {
            return "Negara lain";
        }
```

11. **Perulangan** adalah statement kontrol yang digunakan untuk menjalankan blok kode berulang kali. Pada kode ini, digunakan loop `for` untuk meminta input dan menampilkan data.

```bash
for (int i = 0; i < mbl.length; i++) {
System.out.print("Masukkan nama mobil " + (i + 1) + ": ");
String nama1 = scanner.nextLine();
System.out.print("Masukkan kode mobil " + (i + 1) + ": ");
String kode1 = scanner.nextLine();
```

12. **Input Output Sederhana** digunakan untuk menerima input dari user dan menampilkan output ke user. Pada kode ini, digunakan class `Scanner` untuk menerima input dan method `System.out.println` untuk menampilkan output.

```bash
Scanner scanner = new Scanner(System.in);
System.out.print("Masukkan nama mobil " + (i + 1) + ": ");
String nama1 = scanner.nextLine();
System.out.print("Masukkan kode mobil " + (i + 1) + ": ");
String kode1 = scanner.nextLine();

System.out.println("================================");
System.out.println("Data Mobil: ");
System.out.println(data.displayInfo());
```

13. **Array** adalah struktur data yang digunakan untuk menyimpan beberapa nilai dalam satu variabel. Pada kode ini, `MobilDetail[] mbl = new MobilDetail[2];` adalah contoh penggunaan array.

```bash
MobilDetail[] mbl = new MobilDetail[2];
```

14. **Error Handling** digunakan untuk menangani error yang mungkin terjadi saat runtime. Pada kode ini, digunakan `try catch` untuk menangani error.

```bash
try {
} catch (Exception e) {
    System.out.println("Terjadi Kesalahan: " + e.getMessage());
}
```

## Pembuat
Nama: Malik Jabbar Hernanda
NPM: 2310010186
Kelas: 4A NR Banjarmasin TI
