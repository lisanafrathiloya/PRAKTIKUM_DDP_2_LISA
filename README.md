print("selamat di toko peralatan olahraga")
print("masuk sebagai")
print("1. admin")
print("2. pembeli")
masuk_login =(input("admin/pembeli: "))

if masuk_login == "admin" :
    print("masukan password anda")
    print("menu admin") 
    print("1. menambahkan barang") 
    print("2. menampilkan barang")
    print("3. mengupdate barang")
    print("4. menghapus barang")
    
    menu_admin = input("pilih (1/2/3/4):" )
    
    if menu_admin == "1" :
        peralatan_olahraga = ['Raket', 'tongkat baseball', 'bat', 'shuttle cock', 'bola baseball', 'bola kasti' ]
        peralatan_olahraga.append('bola basket')
        print(peralatan_olahraga)
    elif menu_admin == "2" :
        from prettytable import PrettyTable
        peralatan = PrettyTable ()
        peralatan.field_names = ["no.", "nama barang", "harga"]
        peralatan.add_row(["1", "Raket", "Rp. 200.000"])
        peralatan.add_row(["2", "tongkat baseball", "Rp. 700.000"])
        peralatan.add_row(["3", "bat", "Rp.30.000"])
        peralatan.add_row(["4", "shuttle cock", "Rp. 120.000"])
        peralatan.add_row(["5", "bola baseball", "Rp. 145.000"])
        peralatan.add_row(["6", "bola kasti", "Rp. 20.000"])
        print(peralatan)
    elif menu_admin == "3" :
        peralatan_olahraga = ['Raket', 'tongkat baseball', 'bat', 'shuttle cock', 'bola baseball', 'bola kasti' ]
        peralatan_olahraga.insert(0, "bola volly")
        print(peralatan_olahraga)
    elif menu_admin == "4" :
        peralatan_olahraga = ['Raket', 'tongkat baseball', 'bat', 'shuttle cock', 'bola baseball', 'bola kasti' ]
        del peralatan_olahraga[2]
        print(peralatan_olahraga)
        
elif masuk_login == "pembeli" : 
    print("1. Raket                  Rp. 200.000")
    print("2. Tongkat baseball       Rp. 700.000")
    print("3. bat                    Rp. 30.000 ")
    print("4. shuttle coock          Rp. 120.000")
    print("5. bola baseball          Rp. 145.000")
    print("6. bola kasti             Rp. 20.000 ")
    
    pilih = input("memilih barang(1/2/3/4/5/6): ")
    if pilih == "1":
        Jumlah_harga = input("masukkan jumlah barang yang dibeli: ")
        total = 200000 * Jumlah_harga
        print(f"total belanjaan {total}")
    elif pilih == "2":
        Jumlah = input("masukkan jumlah barang yang dibeli: ")
        total = 700000 * Jumlah
        print(total)
    elif pilih == "3":
        Jumlah = input("masukkan jumlah barang yang dibeli: ")
        total = 30000 * Jumlah
        print(total)
    elif pilih == "4":
        Jumlah = input("masukkan jumlah barang yang dibeli: ")
        total = 120000 * Jumlah
        print(total)
    elif pilih == "5":
        Jumlah = input("masukkan jumlah barang yang dibeli: ")
        total = 145000 * Jumlah
        print(total)
    elif pilih == "6":
        Jumlah = input("masukkan jumlah barang yang dibeli: ")
        total = 20000 * Jumlah
        print(total)
else:
    print("data tidak valid")





![WhatsApp Image 2023-10-16 at 11 22 25](https://github.com/lisanafrathiloya/PRAKTIKUM_DDP_2_LISA/assets/144829981/318ebc14-2c23-48ce-82b8-41e8502cd3dc)
- Program user memilih menjadi admin dan memilih no 1. menambahkan barang
- maka hasil dari input barang ada tambahan 1 barang tambahan
![WhatsApp Image 2023-10-16 at 11 22 50](https://github.com/lisanafrathiloya/PRAKTIKUM_DDP_2_LISA/assets/144829981/e5de2413-f2a4-4ec6-a210-939bea14aa89)
- Program user memilih menjadi admin dan memilih no 2. menampilkan barang
- maka hasil dari input menampilkan barang yang tersedia
![WhatsApp Image 2023-10-16 at 11 23 08](https://github.com/lisanafrathiloya/PRAKTIKUM_DDP_2_LISA/assets/144829981/cbcb99a4-0888-4255-8648-1b3126ef66b2)
- Program user memilih menjadi admin dan memilih no 3. mengupdate barang
- maka hasil dari input mengupdate barang
![WhatsApp Image 2023-10-16 at 11 23 29](https://github.com/lisanafrathiloya/PRAKTIKUM_DDP_2_LISA/assets/144829981/5e5c0556-27ae-4883-9193-926aa465eb66)
- Program user memilih menjadi admin dan memilih no 4. menghapus barang
- maka hasil dari input menghapus salah satu barang
![WhatsApp Image 2023-10-16 at 11 23 18](https://github.com/lisanafrathiloya/PRAKTIKUM_DDP_2_LISA/assets/144829981/67320f3a-d813-448c-9000-221711963bf3)
- Program user memelih menjadi pembeli
- pemebeli bisa memilih barang yang ingin di beli
- dan user bisa memasukan jumlah barang yang di inginkan 




