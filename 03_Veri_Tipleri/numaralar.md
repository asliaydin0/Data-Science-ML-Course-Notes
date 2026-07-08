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


## 2. String (Metin) Veri Tipi

Stringler, tek (`'...'`) veya çift (`"..."`) tırnak içerisine yazılan karakter dizileridir.

