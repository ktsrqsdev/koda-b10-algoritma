# Algoritma
## memindahkan air
1. mulai
2. siapkan 1 wadah kosong tambahan
3. masukan **kopi** pada gelas B ke wadah kosong
4. masukan **teh** pada gelas A ke gelas B bekas **kopi**
5. masukan **kopi** yang ada di wadah tambahan ke gelas A bekas **teh**
6. selesai

## menentukan bilangan ganjil dan genap
### Algoritma Deskriptif
1. mulai
2. tentukan bilangan yang mau di cek
3. jika bilangan yang sudah ditentukan habis kalau *dibagi 2* maka bilangan tersebut adalah **bilangan genap**.
4. jika bilangan yang ditentukan tidak habis kalau *dibagi 2* atau *sisa pembagian menghasilkan 1* maka bilangan tersebut adalah **bilangan ganjil**.
5. selesai
   
### Algoritma Flowchart
``` mermaid

    flowchart TD
    start@{ shape: circle, label: "Start" }
    inputAngka@{ shape: lean-r, label: "bilangan" }
    modulo@{ shape: diamond, label: "bilangan % 2 == 0" }
    genap@{ shape: lean-r, label: "Genap" }
    ganjil@{ shape: lean-r, label: "Ganjil" }
    selesai@{ shape: dbl-circ, label: "Selesai" }
    
    start --> inputAngka
    inputAngka --> modulo
    modulo --ya--> genap
    modulo --tidak--> ganjil
    genap & ganjil --> selesai
    
    
```

### Pseudo-Code
```sh
DECLARE bilangan : INTEGER

bilangan <- 4

IF bilangan MOD 2 = 0 THEN
    OUTPUT "Genap"
ELSE
    OUTPUT "GANJIL"
ENDIF
```

---
## menghitung luas dan keliling lingkaran
1. mulai
2. tentukan nilai jari jarinya
3. jika jari jarinya habis dibagi 7 pi menggunakan 22/7
4. jika tidak maka pi menggunakan 3.14
5. untuk menghitung luas maka gunakan rumus luas yaitu pi dikali jari jari dikali jari jari (luas = pi x r x r)
6. untuk menghitung keliling gunakan rumus 2 dikali pi dikali jari jari (keliling = 2 x pi x r)
7. selesai

### Algoritma Flowchart
``` mermaid
flowchart TD
    start@{ shape: circle, label: "Start" }
    stop@{ shape: dbl-circ, label: "Stop" }
    r@{ shape: lean-r, label: "r" }
    modr@{ shape: diamond, label: "r % 7 == 0" }
    luas1@{ shape: rect, label: "luas = 22/7 * r * r" }
    luas2@{ shape: rect, label: "luas = 3.14 * r * r" }
    keliling1@{ shape: rect, label: "keliling = 2 * 22/7 * r" }
    keliling2@{ shape: rect, label: "keliling = 2 * 3.14 * r" }
    outputluas@{ shape: lean-r, label: "luas" }
    outputkeliling@{ shape: lean-r, label: "keliling" }


    start --> r
    r --> modr
    modr --ya--> luas1
    modr --tidak--> luas2
    luas1 --> keliling1
    luas2 --> keliling2
    keliling1 & keliling2 --> outputluas
    outputluas --> outputkeliling
    outputkeliling --> stop
    
```

### Pseudo-Code

