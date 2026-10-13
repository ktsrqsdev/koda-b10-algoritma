# Algoritma
## Algoritma Deskriptif
### memindahkan air
1. mulai
2. siapkan 1 wadah kosong tambahan
3. masukan **kopi** pada gelas B ke wadah kosong
4. masukan **teh** pada gelas A ke gelas B bekas **kopi**
5. masukan **kopi** yang ada di wadah tambahan ke gelas A bekas **teh**
6. selesai

### menentukan bilangan ganjil dan genap
1. mulai
2. tentukan bilangan yang mau di cek
3. jika bilangan yang sudah ditentukan habis kalau *dibagi 2* maka bilangan tersebut adalah **bilangan genap**.
4. jika bilangan yang ditentukan tidak habis kalau *dibagi 2* atau *sisa pembagian menghasilkan 1* maka bilangan tersebut adalah **bilangan ganjil**.
5. selesai

### menghitung luas dan keliling lingkaran
1. mulai
2. tentukan nilai jari jarinya
3. untuk menghitung luas maka gunakan rumus luas yaitu pi dikali jari jari dikali jari jari (luas = pi x r²)
4. untuk menghitung keliling gunakan rumus 2 dikali pi dikali jari jari (keliling = 2 x pi x r)
6. selesai

## Algoritma Flowchart
### Flowchart menentukan bilangan ganjil dan genap

``` mermaid

    flowchart TD
    start@{ shape: circle, label: "Start" }
    inputAngka@{ shape: lean-r, label: "angka" }
    modulo@{ shape: diamond, label: "angka % 2 == 0" }
    genap@{ shape: lean-r, label: "Genap" }
    ganjil@{ shape: lean-r, label: "Ganjil" }
    selesai@{ shape: dbl-circ, label: "Selesai" }
    
    start --> inputAngka
    inputAngka --> modulo
    modulo --ya--> genap
    modulo --tidak--> ganjil
    genap & ganjil --> selesai
    
    
```
