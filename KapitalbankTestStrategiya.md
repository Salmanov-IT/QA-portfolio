# QA Engineer

## Test Strategy (KapitalBank)

---

## 1. Introduction

Bu sənəd KapitalBankın web saytı və mobil tətbiqi üçün test strategiyasını təsvir edir . Məqsəd sistemin funksional düzgünlüyünü, təhlükəsizliyini və performansını təmin etməkdir.

---

## 2. Goal

Layihənin əsas məqsədi:

- Sistemə təhlükəsiz girişin təmin edilməsi
- Bank əməliyyatlarının düzgün icrası
- Pul köçürmələrinin dəqiqliyi
- Şəxsi və maliyyə məlumatlarının qorunması
- Yük altında stabil işləmə

---

## 3. Scope

### 3.1 Authentication
- Sistemə login
- Şifrə dəyişmə
- SMS OTP təsdiqi

### 3.2 Hesab və Kart Əməliyyatları
- Hesab balansının görüntülənməsi
- Kart məlumatlarının göstərilməsi
- Kartın bloklanması / aktivləşdirilməsi
- Kart limitlərinin dəyişdirilməsi

### 3.3 Pul Köçürmələri
- KapitalBank daxili köçürmələr
- Digər banklara köçürmələr
- Köçürmə tarixçəsinin görüntülənməsi

### 3.4 Ödənişlər
- Kommunal ödənişlər
- Mobil və internet ödənişləri
- Cərimə ödənişləri
- Kredit ödənişləri
- Kredit məlumatlarının görüntülənməsi
- Ödəniş cədvəllərinin görüntülənməsi

### 3.5 Bildirişlər
- Push notification
- SMS və e-mail bildirişləri
- Sistem mesajları

### 3.6 Profil və Ayarlar
- Şəxsi məlumatların yenilənməsi
- Dil seçimi
- Təhlükəsizlik ayarları

---

## 4. Out of Scope

- Bankın daxili server infrastrukturu
- Backend arxitektura dəyişiklikləri
- Core banking sistem dəyişiklikləri

---

## 5. Test Approach & Methodology

### 5.1 Development Model – Agile (Scrum)

Layihə Agile metodologiyası əsasında idarə olunur.

- Sprint müddəti: 2 həftə
- Acceptance Criteria əsasında test case-lər yazılır
- Sprint sonunda review və retrospective keçirilir

Test prosesi development ilə paralel aparılır.

---

### 5.2 Test Methodology

#### Manual Testing
- Positive və Negative ssenarilər
- Exploratory testing
- UI validation

#### Automation Testing
- API testing (Postman)
- Kritik əməliyyatların yoxlanması (Login, OTP, Money Transfer)

#### Risk-Based Testing
- High risk modullar prioritetlə test edilir
- Maliyyə əməliyyatlarına xüsusi diqqət ayrılır

---

## 6. Test Types

- Functional Testing
- Security Testing
- Performance / Load Testing
- Regression Testing
- Smoke Testing
- Usability Testing

---

## 7. Test Environment

| Component | Details |
|-----------|----------|
| OS | Windows 10, macOS, iOS, Android |
| Browser | Chrome, Firefox, Edge, Safari |
| Devices | Mobile (Android/iOS), Desktop |

---

## 8. Test Artifacts

- Test Plan
- Test Cases
- Bug Reports
- Test Execution Report
- Regression Test Suite

---

## 9. Risk Analysis

### 9.1 Money Transfer Risk
Yanlış məbləğ köçürülməsi və ya transaction failure.

**Impact:** Maliyyə itkisi və reputasiya zərəri  
**Priority:** High  

**Mitigation:**
- Backend response validation
- Transaction ID verification
- Regression testing

---

### 9.2 Login & OTP Risk
OTP gecikməsi və ya authentication bypass.

**Impact:** Unauthorized access  
**Priority:** High  

**Mitigation:**
- Timeout testing
- Brute-force ssenarilər
- Multi-device login testi

---

### 9.3 Performance Risk
Yüksək istifadəçi yükü zamanı sistemin ləngiməsi.

**Impact:** Transaction failure  
**Priority:** High  

**Mitigation:**
- Load testing
- Stress testing
- Response time monitorinq

---

### 9.4 Statement Accuracy Risk
Balans və hesabatların səhv göstərilməsi.

**Impact:** Müştəri narazılığı  
**Priority:** Medium  

**Mitigation:**
- Database validation
- API response yoxlanışı

---

### 9.5 UI Risk
Vizual dəyişikliklərin funksionallığa təsiri.

**Priority:** Low  

**Mitigation:**
- UI regression testing
- Cross-browser testing

---

## 10. Entry Criteria

- Development tamamlanıb
- Test environment hazırdır
- Requirement təsdiqlənib

---

## 11. Exit Criteria

- Critical bug yoxdur
- High severity bug-lar fix olunub
- Regression testing uğurla tamamlanıb
- Test coverage ≥ 90%

---

## 12. Conclusion

Bu test strategiyası Agile mühitdə təhlükəsiz, stabil və yüksək keyfiyyətli bank sistemi təqdim etmək məqsədi daşıyır.

