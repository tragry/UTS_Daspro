# UTS_Daspro
Tugas Tim_ Membuat aplikasi yang lebih kompleks menggunakan bahasa pemrograman Python

# PROGRAM TOKO BUNGA
# OLEH MELINA WIDIASTUTIK DAN TIARA ANGGREYANI


import sys

print('\t\t\t\t==============================')
print('\t\t\t\t       TOKO BUNGA ARNA')
print('\t\t\t\t==============================')
print()
print('TOKO BUNGA ARNA MENYEDIAKAN : ')
print('\t\t\t1. Bunga Kaktus            : Rp 75.000,-')
print('\t\t\t2. Bunga Matahari          : Rp 75.000,-')
print('\t\t\t3. Bunga Melati Jasmine    : Rp 150.000,-')
print('\t\t\t4. Bunga Mawar aneka warna : Rp 110.000,-')
print()

print('Toko Bunga ARNA memberikan diskon : ')
print('1. Diskon 25% untuk pembelian diatas Rp 500.000,-')
print('2. Diskon 10% untuk pembelian diatas Rp 350.000,-')
print('3. Diskon 5% untuk pembelian diatas Rp 250000,-')

print()
pilihan = int(input('Masukkan pilihan (1/2/3/4) ? : '))

if pilihan ==1 :
    hargaBunga = 75000
elif pilihan ==2 :
    hargaBunga = 75000
elif pilihan ==3 :
    hargaBunga = 150000
elif pilihan ==4 :
    hargaBunga = 110000
else :
    print()
    print('Maaf paket yang anda pilih tidak tersedia')
    print('Atas nama Toko Bunga ARNA saya mengucapkan Terimakasih')
    sys.exit()
    
jumlah = int(input('Berapa Banyak Yang Mau di Beli? :'))

pembelanjaan = hargaBunga*jumlah
    
if pembelanjaan > 500000 :
    diskon = 25
elif pembelanjaan > 350000 :
    diskon = 10
elif pembelanjaan > 250000 :
    diskon = 5
else :
    diskon = 0
    
jumlahDiskon = pembelanjaan * diskon/100

hargaAkhir = pembelanjaan - jumlahDiskon

print()
print('\t\t\t\tRekap Pembelanjaan Anda')
print('\t\t\t\t=======================')
print()
print('Pilihan Paket      : %d' %pilihan)
print('Harga Paket        : Rp.%d' %hargaBunga)
print('Jumlah Pembelian   : %d Bunga' %jumlah)
print('Pembelanjaan       : Rp.%d' %pembelanjaan)
print('Diskon             : %d%%' %diskon)
print('Jumlah Diskon      : %d' %jumlahDiskon)
print('---------------------------------')
print('HARGA AKHIR        : Rp.%d' %hargaAkhir)

print()
print('Terimakasih Atas Kunjungan Anda !!!!')




