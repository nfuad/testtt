# testtt
Bu hesabat platformadakı tibbi məhsullar kateqoriyası üzrə aparılmış funksional testlərin nəticələrini əks etdirir.

## ✅ Pozitiv Yoxlamalar
*Sistemin gözlənildiyi kimi və problemsiz işlədiyini göstərən testlər:*

### 📂 Kateqoriya və Giriş
* **Kateqoriya Keçidi:** Kateqoriyalarda "Tibbi məhsullar" bölməsinə kliklədikdə səhifə problemsiz açıldı.
* **Məhsul Kartı:** Tibbi məhsullar kateqoriyasındakı hər hansı konkret məhsula kliklədikdə məhsulun detallı səhifəsi açıldı.

### 🔍 Axtarış və Məzmun
* **Axtarış Funksiyası:** Axtarış sahəsinə "termometr" yazdıqda sistem yalnız termometrləri nəticə olaraq çıxardı.
* **Məzmun Uyğunluğu:** Tibbi məhsullar bölməsində yalnız həmin kateqoriyaya aid məhsullar nümayiş olundu.

### 📍 Regional Uyğunluq
* **Regional Filtr:** "Bakıdakı tibbi məhsullar" seçiminə kliklədikdə müvafiq siyahı dərhal açıldı.

---

## ❌ Neqativ Ssenarilər (Məhdudiyyətlər və Qüsurlar)
*Sistemin limitlərini, qadağalarını və ya məntiqi çatışmazlıqlarını göstərən hallar:*

### 📍 Şəhər və Məkan Filtrləri
* **Çoxlu Seçim Məhdudiyyəti:** Sistem eyni anda bir neçə müxtəlif şəhəri seçməyə imkan vermir.
* **Regional Tapılmama:** Bakı bazasına aid olan termometrin Ağdam axtarışında çıxmaması (Məntiqi doğruluq).

### 💸 Qiymət və Rəqəmsal Girişlər
* **Mənfi Qiymət Bloku:** Qiymət xanasına mənfi rəqəm daxil etmək bloklanıb (Sistem təhlükəsizliyi).
* **Sıfır Nəticə:** Minimum və maksimum qiymət "0" təyin edildikdə bazada heç bir məhsul tapılmır.

### 🚚 Çatdırılma Məntiqi
* **Filtr Uyğunsuzluğu:** "Bütün növ çatdırılmalar" seçildikdə, yalnız tək növ çatdırılması olan məhsulların da siyahıda qalması (Filtr optimizasiyası tələb olunur).

> *Qeyd: Bu hesabat proqramın QA (Keyfiyyətə Nəzarət) mərhələsi üçün hazırlanmışdır.*
