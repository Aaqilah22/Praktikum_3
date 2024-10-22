# Praktikum3
## 1. Membuat Class Pegawai
  // Kelas Pegawai
  public class Pegawai {
      private String nama;
      private double gajiPokok;

      // Setter dan Getter untuk nama
      public void setNama(String nama) {
          this.nama = nama;
      }

      public String getNama() {
          return nama;
      }

      // Setter dan Getter untuk gajiPokok
      public void setGajiPokok(double gajiPokok) {
          this.gajiPokok = gajiPokok;
      }

      public double getGajiPokok() {
          return gajiPokok;
      }

      // Method untuk mencetak informasi pegawai
      public void cetakInfo() {
          System.out.println("Nama: " + nama);
          System.out.println("Gaji Pokok: Rp" + gajiPokok);
      }
    }  
Penjelasan:
*Atribut :*
- nama (tipe String): Untuk menyimpan nama pegawai.
- gajiPokok (tipe double): Untuk menyimpan gaji pokok pegawai
*Setter dan Getter :*
- setNama(String nama): Method ini digunakan untuk memberikan nilai pada atribut nama.
- getNama(): Method ini mengembalikan nilai dari atribut nama.
- setGajiPokok(double gajiPokok): Method ini digunakan untuk memberikan nilai pada atribut gajiPokok.
- getGajiPokok(): Method ini mengembalikan nilai dari atribut gajiPokok.
*Method cetakInfo() :*
Adalah method untuk mencetak informasi pegawai, seperti nama dan gaji pokok. Method ini tidak menerima parameter dan tidak mengembalikan nilai (void).

## 2. Membuat Kelas Manager
  // Kelas Manager (turunan dari Pegawai)
  public class Manager extends Pegawai {
    private double tunjangan;

    // Setter dan Getter untuk tunjangan
    public void setTunjangan(double tunjangan) {
        this.tunjangan = tunjangan;
    }

    public double getTunjangan() {
        return tunjangan;
    }

    @Override
    public void cetakInfo() {
        super.cetakInfo(); // Memanggil cetakInfo() dari superclass (Pegawai)
        System.out.println("Tunjangan: Rp" + tunjangan);
    }

    // Method untuk mencetak tunjangan saja
    public void cetakTunjangan() {
        System.out.println("Tunjangan: Rp" + tunjangan);
    }
  }
Penjelasan :
*Atribut :*
tunjangan (tipe double): Atribut tambahan untuk menyimpan tunjangan yang diterima oleh seorang manager.
*Setter dan Getter :*
- setTunjangan(double tunjangan): Method ini digunakan untuk memberikan nilai pada atribut tunjangan.
- getTunjangan(): Method ini mengembalikan nilai dari atribut tunjangan.
*Method cetakTunjangan() :*
Method ini khusus untuk mencetak nilai tunjangan seorang manager. Berbeda dengan cetakInfo(), method ini hanya fokus pada tunjangan saja.
*Override Method cetakInfo() :*
Di kelas Manager, method cetakInfo() di-override (diganti) untuk menampilkan informasi tambahan, yaitu tunjangan. Method super.cetakInfo() digunakan untuk memanggil cetakInfo() dari kelas Pegawai dan kemudian ditambah dengan informasi tunjangan.

## 3. Membuat Kelas Programmer
  // Kelas Programmer (turunan dari Pegawai)
public class Programmer extends Pegawai {
    private double bonus;

    // Setter dan Getter untuk bonus
    public void setBonus(double bonus) {
        this.bonus = bonus;
    }

    public double getBonus() {
        return bonus;
    }

    // Override method cetakInfo
    @Override
    public void cetakInfo() {
        super.cetakInfo(); // Memanggil cetakInfo() dari superclass (Pegawai)
        System.out.println("Bonus: Rp" + bonus);
    }

    // Method untuk mencetak bonus saja
    public void cetakBonus() {
        System.out.println("Bonus: Rp" + bonus);
    }
  }
Penjelasan :
*Atribut :*
bonus (tipe double): Atribut tambahan yang digunakan untuk menyimpan bonus yang diterima oleh programmer.
*Setter dan Getter :*
- setBonus(double bonus): Method ini digunakan untuk memberikan nilai pada atribut bonus.
- getBonus(): Method ini mengembalikan nilai dari atribut bonus.
*Method cetakBonus() :*
Method ini khusus digunakan untuk mencetak nilai bonus seorang programmer.
*Override Method cetakInfo() :*
Sama seperti pada kelas Manager, method cetakInfo() di-override untuk menambahkan informasi tentang bonus di samping informasi pegawai standar. Method super.cetakInfo() digunakan untuk memanggil method dari kelas induk.

## 4. Membuat Kelas Main
  public class Main {
    public static void main(String[] args) {
        // Membuat objek Manager
        Manager manager = new Manager();
        manager.setNama("Budi");
        manager.setGajiPokok(5000000);
        manager.setTunjangan(2000000);
        manager.cetakInfo();

        System.out.println();

        // Membuat objek Programmer
        Programmer programmer = new Programmer();
        programmer.setNama("Andi");
        programmer.setGajiPokok(4000000);
        programmer.setBonus(1500000);
        programmer.cetakInfo();
    }
  }
Penjelasan :
- Pertama, kita membuat objek Manager bernama Budi dan mengatur gajiPokok serta tunjangan. Kemudian, method cetakInfo() akan mencetak semua informasi yang dimiliki oleh objek tersebut.
- Selanjutnya, kita membuat objek Programmer bernama Andi dan mengatur gajiPokok serta bonus. Sama seperti sebelumnya, method cetakInfo() akan mencetak informasi lengkap programmer.

## Out put
![Out put](https://github.com/user-attachments/assets/eec16604-8a4a-47ba-a910-4fe39b18282f)
