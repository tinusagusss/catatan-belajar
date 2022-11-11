# Belajar Dart Dasar
----------
## Membuat Project 
```markdown
<!-- Create Project -->
dart craete <project_name>

<!-- Open Project using VSC -->
code .\<project_name>

```

## Variable
Semua tipe data di dalam Dart merupakan Object.
```markdown
<!-- Singgle Data -->
<date_type> <name>;

<!-- Singgle Data -->
var <name>;

<!-- Singgle Data -->
dynamic <name>;

<!-- Final Variable -->
final <date_type> <name>;

<!-- Final Variable -->
final <name>;

<!-- Const Variable -->
const <date_type> <name>;
```
## Kata Kunci
Final, Const, Late, num

Late menjadikan variable menjadi lazy

num bisa menjadi variable sebagai integer dan decimal.

## String

### Interpolation
Kita dapat menggunakan interpolation untuk mengambil nilai dari suatu variable.

`${<isi expression>}` atau jika sederhana `$<isi expression>`

### Backslash 
hanya dapat digunakan untuk satu karakter untuk satu backslash.
```dart
  var name = 'Hello Wolrd';

  print('Isi pesan : $name, terdapat kata \'world\' di pesan tersebut');
```

### Multi-line
```dart
  var longString = ''' 
  <Multi String>
   '''
```
## Number
variable ini dapat menyimpan nilai bulat dan juga desimal.

```dart
num number = 1;

number 1.4;
```
## Kenapa main menggunakan void? 
Dikarenakan main tugasnya hanya memanggil function atau logic yang telah dibuat sehingga tidak perlu mengembalikan nilai.

## Petik satu atau petik dua?
Lebih baik kita menggunakan petik satu untuk kebutuhan print sebuah String. Namun, ketika ada nilai didalam string gunakan petik dua

## Dynamic 
tipe data yang digunakan untuk menampung data apapun kedalam variable.

`var` `num`
## Penamaan variable
Kita menggunakan camelCase.

## Final and Const
Keduanya sama-sama membuat variable manjadi immutable, namun satu perbedaan sederhana yang dapat dijumpai pada mereka berdua ialah: `const` sama sekali tidak dapat di modifikasi nilai didalam sebuah array, sedangkan `final` masih bisa diubah.

`int? number` agar variable dapat dibiarkan kosong terlebih dahulu sampai nanti akan digunakan.
`late var <variable> = function();` digunakan untuk hanya mengambil nilai dari suatu funtion namun tidak mengeksekusi seluruh perintah didalamnya.

## Operator Type Test
### as 
Merupakan typecast yang artinya dalam melakukan konnversi tipe data secara paksa

```dart
dynamic number = 1;

var variableInt = number as int;

// Tidak Bisa
var variableInt = number as String;
```
### is
Bernilai benar apabila object sesuai tipe datanya
```dart
dynamic number = 1;

print(number is int);
print(number is bool);
```
### is!
Bernilai benar apabila object tidak sesuai tipe datanya
```dart
dynamic number = 1;

print(number !is int);
print(number !is bool);
```
## Collection
### List

```dart
  List<int> listInt = [];

  var listString = <String>[];
  print('$listInt $listString');

  var names = <String>[];

  names.add('agus');

  print('$names ${names.length}');
```
### Set
Set tidak menjamin urutannya sesuai dan tidak memiliki index.

untuk dapat menyimpan data data yang unik.
### Map


Pertemuan 05 Wajib upload ke GitHub.