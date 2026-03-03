#   Hi I'm Yusif

## Junior QA Engineer

## Test Strategy (KapitalBank)

###  Goal
- Kapital bankın saytının ve mobil tətbiqinin funksionalliğını,yük altında necə işləyəcəyini və təhlükəsiz işləməsini test edəciyik
- Əsas fokusumuz sistemə girişin təmin edilməsi bak əməliiyatlarının təhlükəzisliyi və şəxsi məlumatların qorunmasının təmin edilməsi 

### Scope

#### İstifadəçi  Authentication:
- Sistemə login
- Şifrə dəyişmə
- SMS təsdiqi

#### Hesab və kart əməliyyatları
- Hesab balansının görüntülənməsi
- Kart məlumatlarının göstərilməsi
- Kartın bloklanması və aktivləşdirilməsi
- Kart limitlərinin dəyişdirilməsi

#### Pul köçürmələri
- KapitalBank daxili köçürmələr
- Digər banklara köçürmələr
- Köçürmə tarixçəsinin görüntülənməsi

#### Ödənişlər
- Komunal ödənişlər
- Mobil və internet ödənişləri
- Cərimə ödənişləri
- Kredit ödənişləri
- Kreditin görüntülənməsi
- Ödəniş cədvəllərinin görüntülənməsi
  
#### Bildirişlər və mesajlar
- Push notification-lar
- SMS və e-mail bildirişləri
- Sistem mesajları

#### Profil və ayarlar
- Şəxsi məlumatların yenilənməsi
- Dil seçimi
- Təhlükəsizlik ayarları

##### Out of Scope:
- Bankın daxili server infrastrukturu
- bank sistemində backend tərəfdə ediləcək dəyişikliklər

###  Test Types
- Functional Testing 
- Security Testing 
- Performance / Load Testing
- Usability / UI Testing
- Regression Testing

###  Test Methodology
- Manual Testing: main funksiyalarin yoxlanmasi 
- Automation Testing: critical əməliyyatlar üçün postmanin istifadə olunması

### Test Environment
|Component|Details|
|-|-|
| OS | Windows 10, macOS, iOS, Android |
| Browser | Chrome, Firefox, Edge, Safari |
| Devices | Mobile (Android/iOS), Desktop |

###  Test Documents
- Test Plan
- Test Cases
- Test Execution Reports
- Regression Test Suite

###  Risks & Priority
| Risk | Priority | Notes |
|-|-|-|
| Money Transfer | High | Main operation, must be correct |
| Login & OTP | High | Critical for security |
| Statement & Reports | Medium | Accuracy needed, no money loss |
| UI changes | Low | Visual, no impact on functionality |


