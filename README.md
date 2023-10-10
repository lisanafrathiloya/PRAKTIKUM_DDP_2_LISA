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
