# Definisikan kelas Mahasiswa
class Mahasiswa:
    def __init__(self, nama, kelas):
        self.nama = nama
        self.kelas = kelas
        self.tugas = []  # Daftar untuk menyimpan tugas yang dikumpulkan

    def kumpulkan_tugas(self, tugas):
        self.tugas.append(tugas)
        print(f'{self.nama} telah mengumpulkan tugas: {tugas}')

    def tampilkan_info(self):
        print(f'Nama Mahasiswa: {self.nama}')
        print(f'Kelas: {self.kelas}')
        print('Tugas yang dikumpulkan:')
        for i, t in enumerate(self.tugas, start=1):
            print(f'{i}. {t}')

# Membuat objek Mahasiswa untuk Arsita Ayu Irmayanti dari kelas 2D
mahasiswa1 = Mahasiswa('Arsita Ayu Irmayanti', '2D')

# Menampilkan informasi tentang mahasiswa
mahasiswa1.tampilkan_info()

# Arsita mengumpulkan beberapa tugas
mahasiswa1.kumpulkan_tugas('Tugas Matematika')
mahasiswa1.kumpulkan_tugas('Tugas Fisika')

# Menampilkan informasi tentang mahasiswa lagi untuk melihat tugas yang telah dikumpulkan
mahasiswa1.tampilkan_info()
