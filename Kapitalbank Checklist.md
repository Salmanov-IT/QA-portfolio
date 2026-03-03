# QA Checklist – Kapital Bank (Practice Project)

> Qeyd: Bu checklist tədris və portfolio məqsədilə hazırlanmışdır.

---

## Authentication – Login

| ID | Yoxlama | Nə etdim | Nəticə | Status | Qeyd |
|-|-|-|-|-|-|
| CL-01 | Düzgün username və şifrə ilə giriş | Valid məlumat daxil edib login etdim | Sistem dashboard-a yönləndirdi | Pass | - |
| CL-02 | Boş sahələr üçün validation | Inputları boş buraxıb login etdim | “Bu sahə doldurulmalıdır” mesajı çıxdı | Pass | - |
| CL-03 | Yanlış şifrə | Yanlış şifrə daxil etdim | Xəta mesajı göstərildi | Pass | - |
| CL-04 | Session timeout | Müəyyən müddət aktivlik etmədim | Sistem avtomatik logout etdi | Pass | Təxminən 10 dəq |
| CL-05 | Show/Hide password | Şifrə yazıb göz ikonuna klik etdim | Şifrə göstərildi/gizləndi | Pass | - |

---

## Registration

| ID | Yoxlama | Nə etdim | Nəticə | Status | Qeyd |
|-|-|-|-|-|-|
| CL- 06 | Email formatı | Yanlış formatda email daxil etdim | Validation mesajı çıxdı | Pass | - |
| CL-07 | Boş sahə yoxlanışı | Formanı boş göndərdim | Required mesajı çıxdı | Pass | - |
| CL-08 | Şifrə qaydaları | Qısa şifrə yazdım | Minimum tələblər göstərildi | Pass | - |
| CL-09 | Şifrə təkrarı | Fərqli şifrələr daxil etdim | Uyğunsuzluq mesajı çıxdı | Pass | - |
| CL-10 | Mövcud email | Mövcud email ilə qeydiyyat etdim | Sistem icazə vermədi | Pass | - |

---

## Pul Köçürmələri

| ID | Yoxlama | Nə etdim | Nəticə | Status | Qeyd |
|-|-|-|-|-|-|
| CL-11 | Bank daxili köçürmə | Eyni bank hesabına pul göndərdim | Köçürmə uğurlu oldu | Pass | - |
| CL-12 | Yanlış məlumat | Yanlış IBAN daxil etdim | Xəta mesajı çıxdı | Pass | - |
| CL-13 | Komissiya hesablanması | Köçürmə etdikdə komissiyanı yoxladım | Komissiya düzgün çıxıldı | Pass | - |
| CL-14 | Balans dəyişməsi | Köçürmə sonrası balansı yoxladım | Düzgün məbləğ çıxıldı | Pass | - |

---

## Təhlükəsizlik

| ID | Yoxlama | Nə etdim | Nəticə | Status | Qeyd |
|-|-|-|-|-|-|
| CL-15 | HTTPS istifadəsi | URL-i yoxladım | HTTPS aktiv idi | Pass | SSL mövcuddur |
| CL-16 | Yeni cihazdan giriş | Başqa brauzerdən login etdim | Təsdiq kodu tələb olundu | Pass | - |

---

## UI/UX

| ID | Yoxlama | Nə etdim | Nəticə | Status | Qeyd |
|-|-|-|-|-|-|
| CL-17 | Mobil uyğunluq | Mobile view-da yoxladım | UI düzgün açıldı | Pass | - |
| CL-18 | Dil dəyişmə | Dil dəyişdirdim | Bütün mətnlər düzgün dəyişdi | Pass | - |
