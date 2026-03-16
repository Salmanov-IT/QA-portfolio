# QEYD: Bu Test Case lər tədris məqsədi ilə hazırlanmışdır.
# Detailed Test Cases

---

##  Login Page – Test Cases

| Test Case ID | Scenario ID | Title | Precondition | Test Steps | Test Data | Expected Result |
|-|-|-|-|-|-|-|
| TC-01 | TS-01 | Valid login | İstifadəçi Signed up edib | 1.  Login səhifəsinə daxil ol 2.  Valid username daxil et 3.  Valid password daxil et 4.  Login klik et | valid_user / valid_pass | İstifadəçi dashboard səhifəsinə yönləndirilməlidir |
| TC-02 | TS-02 | Login with invalid password | İstifadəçi mövcuddur | 1.Login səhifəsinə daxil ol 2.Valid username 3.Invalid password 4.Login klik et | valid user / invalid password | Sistem loginə icazə verməməli və xəta mesajı göstərməlidir |
| TC-03 | TS-03 | Login with empty fields | Heç bir şərt yoxdur | 1. Login səhifəsinə daxil ol 2. Inputları boş burax 3. Loginə klik et | empty | Validasiya mesajı göstərilməlidir |
| TC-04 | TS-04 | Forgot password redirect | Heç bir şərt yoxdur | 1. Login səhifəsinə daxil ol 2. “Forgot Password” linkinə klik et | Heçnə daxil edilmir| İstifadəçi şifrə bərpa səhifəsinə yönləndirilməlidir |
| TC-05 | TS-05 | Error message validation | İstifadəçi mövcud deyil | 1. Login səhifəsinə daxil ol 2. Yanlış username və password daxil et 3. Login klik et | wrong user / wrong pass | Aydın və düzgün xəta mesajı göstərilməlidir |

---

##  Credit Calculator – Test Cases

| Test Case ID | Scenario ID | Title | Precondition | Test Steps | Test Data | Expected Result |
|-|-|-|-|-|-|-|
| TC-06 | TS-06 | Valid credit calculation | Kalkulyator səhifəsi açıqdır | 1. Məbləğ daxil et 2. Müddət seç 3. Hesabla klik et | 10000 AZN / 12 ay | Aylıq ödəniş düzgün hesablanmalıdır |
| TC-07 | TS-07 | Zero amount validation | Kalkulyator səhifəsi açıqdır | 1. Məbləğ hissəsinə 0 yaz 2. Müddət seç 3. Hesabla klik et | 0 AZN | Xəta mesajı göstərilməlidir |
| TC-08 | TS-07 | Negative amount validation | Kalkulyator səhifəsi açıqdır | 1. Məbləğ hissəsinə -500 yaz 2. Hesabla klik et | -500 AZN | Sistem mənfi dəyəri qəbul etməməlidir |
| TC-09 | TS-08 | Exceeding maximum limit | Kalkulyator səhifəsi açıqdır | 1. Maksimum limitdən artıq məbləğ daxil et 2. Hesabla klik et | 1000000 AZN | Xəbərdarlıq mesajı göstərilməlidir |
| TC-10 | TS-09 | UI result display check | Kalkulyator səhifəsi açıqdır | 1. Valid məlumat daxil et 2. Hesabla klik et | 5000 AZN / 6 ay | Nəticə düzgün formatda və oxunaqlı göstərilməlidir |

---

## Search Function – Test Cases

| Test Case ID | Scenario ID | Title | Precondition | Test Steps | Test Data | Expected Result |
|-|-|-|-|-|-|-|
| TC-11 | TS-10 | Valid search keyword | Ana səhifə açıqdır | 1. Axtarış sahəsinə məhsul adı yaz 2. Enter bas | kredit | Uyğun nəticələr göstərilməlidir |
| TC-12 | TS-11 | Case sensitivity check | Ana səhifə açıqdır | 1. Axtarış sahəsinə eyni sözü böyük hərflə yaz 2. Enter bas | KREDIT | Nəticələr kiçik hərflə eyni olmalıdır |
| TC-13 | TS-12 | Special characters search | Ana səhifə açıqdır | 1. Axtarış sahəsinə xüsusi simvol daxil et 2. Enter bas | @#$% | Sistem xəta verməməli və uyğun mesaj göstərməlidir |
