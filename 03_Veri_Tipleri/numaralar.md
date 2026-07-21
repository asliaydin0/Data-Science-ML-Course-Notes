# Python: Sayısal Veri Tipleri (Numbers)

Python'da sayısal veriler temel olarak iki türe ayrılır. Matematiksel işlemler ve veri analizi yaparken bu ayrımları bilmek önemlidir.

### 1. Integer (int)
Tam sayıları ifade eder. Pozitif, negatif veya sıfır olabilir.
* **Örnek:** `x = 10`, `y = -5`, `z = 0`

### 2. Float (float)
Ondalıklı sayıları ifade eder. Matematiksel hassasiyet gerektiren durumlarda kullanılır.
* **Örnek:** `x = 3.14`, `y = 2.0`, `z = -0.5`

### 3. Temel Matematiksel İşlemler
Python'da sayıları şu operatörlerle işleyebiliriz:

| Operatör | İşlem | Örnek |
| :--- | :--- | :--- |
| `+` | Toplama | `5 + 2 = 7` |
| `-` | Çıkarma | `5 - 2 = 3` |
| `*` | Çarpma | `5 * 2 = 10` |
| `/` | Bölme | `5 / 2 = 2.5` |
| `**` | Üs Alma | `5 ** 2 = 25` |
| `//` | Tam Bölme | `5 // 2 = 2` |

### 4. İpucu: İşlem Önceliği
Matematiksel işlemlerde standart işlem önceliği (Parantez, Üs, Çarpma/Bölme, Toplama/Çıkarma) geçerlidir. 

```python
# Örnek
sonuc = (10 + 5) * 2 / 3
print(sonuc) # Çıktı: 10.0
```

# String (Metin) Veri Tipi

Stringler, tek (`'...'`) veya çift (`"..."`) tırnak içerisine yazılan karakter dizileridir.

### Temel Özellikler
* **Birleştirme:** `+` operatörü ile metinleri birleştirebiliriz.
* **Çarpma:** Bir string'i tam sayı ile çarpmak, metni tekrar ettirir.
* **Uzunluk:** `len()` fonksiyonu metindeki karakter sayısını (boşluklar dahil) verir.

### Karakter Erişimi (İndeksleme)
Stringler birer karakter dizisidir ve Python'da indeksleme **0'dan başlar**.

```python
s = "Merhaba"
print(s[0]) # 'M' karakterini verir
print(s[6]) # 'a' karakterini verir
```
### Slicing (Dilimleme)

Bir dizinin (string, liste vb.) belirli bir aralığını almak için kullanılır.

## Söz Dizimi

```python
[başlangıç:bitiş:adım]
```

- **başlangıç:** Başlanacak indeks.
- **bitiş:** Bu indeks dahil değildir.
- **adım:** Kaçar kaçar ilerleyeceğini belirtir.

## Örnekler

```python
s = "PythonProgramlama"

print(s[0:6])   # 0'dan 6'ya kadar -> "Python"
print(s[6:])    # 6'dan sona kadar -> "Programlama"
print(s[::2])   # Tümünü al, 2'şer atla -> "PtoPormaa"
print(s[::-1])  # Tersten yazdır -> "amalmargorPnohtyP"
```

### Açıklamalar

| İfade | Açıklama |
|-------|----------|
| `s[0:6]` | İlk 6 karakteri alır. |
| `s[6:]` | 6. indexten sonuna kadar alır. |
| `s[:6]` | Baştan 6. indekse kadar alır. |
| `s[::2]` | Baştan sona 2 karakter atlayarak alır. |
| `s[::-1]` | String'i ters çevirir. |

---

# Gelişmiş İpuçları

## A. Tip Kontrolü

Bir değişkenin veri tipini öğrenmek için `type()` fonksiyonu kullanılır.

### Örnek

```python
x = 10
print(type(x))
```

**Çıktı**

```python
<class 'int'>
```

---
## B. Kullanıcıdan Veri Alma

Kullanıcıdan veri almak için `input()` fonksiyonu kullanılır.

> **Dikkat:** `input()` fonksiyonu her zaman **string (`str`)** döndürür. Sayısal işlemler yapılacaksa uygun veri tipine dönüştürülmelidir.

### Örnek

```python
yas = int(input("Yaşınızı girin: "))
print(yas)
```
Başka dönüşüm örnekleri:

```python
sayi = int(input("Sayı girin: "))
ondalik = float(input("Ondalıklı sayı girin: "))
```
---

## C. F-String (Metin Biçimlendirme)

Python'da değişkenleri metin içine yerleştirmenin en modern ve okunabilir yöntemidir.

### Söz Dizimi

```python
f"Metin {degisken}"
```
### Örnek

```python
ad = "Aslı"
print(f"Hoş geldin, {ad}!")
```

**Çıktı**

```text
Hoş geldin, Aslı!
```