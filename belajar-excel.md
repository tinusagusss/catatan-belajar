# **Belajar Rumus Excel**
Excel memiliki banyak sekali fungsi atau rumus yang dapat digunakan untuk mengolah data sesuai dengan kebutuhan kita.

Berikut beberapa rumus atau fungsi yang sering digunakan:

## **Wildcard**
[Wildcard](https://www.adh-excel.com/2020/10/penggunaan-wild-card-di-excel.html) merupakan karakter khusus yang dapat digunakan untuk mewakili sebuah karakter ataupun nilai yang tidak diketehui.

Berikut beberapa jenis wildcard yang dapat digunakan:
1. Tanda Bintang (*)
2. Tanda Tanya (?)
3. Tanda Seru (!)
4. Tanda Kurung ([])
5. Tanda Kurang (-)
6. Tanda Pagar (#)

###  Tanda Bintang
----------

```
Nasi*
```
Berguna untuk mencari karakter didalam sell yang mengandung **awalan** *Nasi*
```
*Goreng*
```
Berguna untuk mencari karakter didalam sell yang mengandung kata *Goreng* **diantara** karakter lainnya
```
*Pedas
``` 
Berguna untuk mencari karakter didalam sell yang mengandung **akhiran** *Pedas*

## **Menggabungkan Cell**
Didalam excel terdapat banyak data yang dimuat dalam sebuah cell, dengan terpisahnya data-date tersebut akan ada dikondisi tertentu kita harus mengabungkan data-data tersebut menjadi satu.

Tentunya excel menyediakan fungsi yang dapat digunakan untuk dapat menggabungkan data. Berikut cara untuk menggabungkan beberapa cell dalam excel:

### Menggunakan Dan(&)
```
=Cell & Cell & Cell
```
### Menggunakan Concat()
```
=Concate(Cell, Cell)
```
### Menggunakan Textjoin()
```
=TEXTJOIN(" ", TRUE, Range)
```