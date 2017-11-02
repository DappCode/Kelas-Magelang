# Pertemuan 11 
## Nur Arif
## Boostrap

### colom 
- `row` = maksimal colomnya 12, jadi jika jumlah `col` belum mencapai dua belas maka masih di colom yang sama, dan jika sudah mencapai 12 maka dia akan membuat colom baru di bawahnya.
    - berfungsi menghilangi margin

- `auto` = membuat lebar colom sesuai dengan ukuran content yang ada.

- `col-sm-8` = jika ukuran small keatas maka akan membuat colom 8 , jika kebawah maka akan membuat colom menjadi 100%. 

- membuat kolom untuk di atas `start` 
- membuat kolom untuk di tengah `center`
- membuat kolom unntuk di bawah `end`
    ```html
    <div class="row align-items-start">
    <div class="row align-items-center">
    <div class="row align-items-end">
    ```

- `arround` = membuat colom di antaranya, dan memiliki padding di tepinya  
    - tidak akan berjalan jiga jumlah `col` dari contentnya mencapai 12.

- `between` = membuat kolom dianataranya tetapi tidak memiliki, paddingnya di tepinya
    - sama seperti arround

- ## no gutters 
    > menghilangkan margin tepinya 


- ## flex order 
    > mengurutkan kkolomnya, walaupun di html di buat nomor ke 5
- ## membuat Margin 
    - mr : margin right
    - ml : margin left

- ## Nasting
    > di dalam grid bisa bikin grid lagi.
