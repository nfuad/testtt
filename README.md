# testtt
md_content = """# 📋 Tibbi Məhsullar Bölməsi - Test Hesabatı

Bu hesabat platformadakı tibbi məhsullar kateqoriyası üzrə aparılmış funksional testlərin nəticələrini əks etdirir.

---

## ✅ Pozitiv Ssenarilər (Uğurlu Nəticələr)
*Sistemin gözlənildiyi kimi və problemsiz işlədiyini göstərən testlər:*

| Test Parametri | Gözlənilən Davranış | Nəticə |
| :--- | :--- | :--- |
| **Kateqoriya Keçidi** | "Tibbi məhsullar" bölməsi klikləndikdə açılmalıdır. | Pass |
| **Regional Filtrləmə** | Bakı şəhəri üzrə tibbi məhsullar siyahıya alınmalıdır. | Pass |
| **Məzmun Uyğunluğu** | Bölmədə yalnız tibbi təyinatlı mallar görünməlidir. | Pass |
| **Axtarış Funksionallığı** | "Termometr" axtarışı zamanı müvafiq cihazlar tapılmalıdır. | Pass |
| **Məhsul Kartı** | Seçilmiş məhsula kliklədikdə detallı baxış açılmalıdır. | Pass |

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

---
> *Qeyd: Bu hesabat proqramın QA (Keyfiyyətə Nəzarət) mərhələsi üçün hazırlanmışdır.*
"""

# Faylın saxlanılması
file_name = "Tibbi_Mehsullar_Test_Hesabati_v3.md"
with open(file_name, "w", encoding="utf-8") as f:
    f.write(md_content)
