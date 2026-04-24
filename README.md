# testtt
from ds_python_interpreter import HTML
import os

# Define the content for the Markdown file
md_content = """# Tibbi Məhsullar Bölməsinin Test Hesabatı

## 1. Pozitiv Yoxlamalar (Uğurlu Testlər)
Aşağıdakı funksionallıqlar gözlənildiyi kimi çalışır:

* **Kateqoriya Keçidi:** Kateqoriyalarda "Tibbi məhsullar" bölməsinə kliklədikdə səhifə problemsiz açılır.
* **Regional Filtr:** "Bakıdakı tibbi məhsullar" seçiminə kliklədikdə müvafiq siyahı açılır.
* **Məzmun Uyğunluğu:** Tibbi məhsullar bölməsində yalnız həmin kateqoriyaya aid məhsullar nümayiş olunur.
* **Axtarış Funksiyası:** Axtarış sahəsinə "termometr" yazdıqda sistem yalnız termometrləri nəticə olaraq çıxarır.
* **Məhsul Kartı:** Tibbi məhsullar kateqoriyasındakı hər hansı konkret məhsula kliklədikdə məhsulun detallı səhifəsi açılır.

## 2. Neqativ Yoxlamalar (Məhdudiyyətlər və Xətalar)
Aşağıdakı hallar sistemin məhdudiyyətlərini və ya potensial xətaları göstərir:

* **Çoxlu Şəhər Seçimi:** Sistem eyni anda bir neçə şəhəri seçməyə icazə vermir.
* **Qiymət Sahəsi:** Qiymət xanasına mənfi rəqəm yazmaq mümkün deyil (Gözlənilən davranışdır).
* **Sıfır Qiymət Filtri:** Həm minimum, həm də maksimum qiymətə "0" yazdıqda heç bir məhsul tapılmır.
* **Məkan Uyğunsuzluğu:** Bakıda yerləşən termometri Ağdam üçün axtarışa verdikdə, məntiqi olaraq nəticə çıxmır.
* **Çatdırılma Filtri:** "Bütün növ çatdırılmalar" seçildikdə, yalnız bir növ çatdırılması olan məhsulların da siyahıda görünməsi müşahidə olunur.
"""

# Save to a .md file
file_path = "tibbi_mehsullar_test_hesabati.md"
with open(file_path, "w", encoding="utf-8") as f:
    f.write(md_content)

print(f"File saved: {file_path}")
