# WhatSave CI/CD - February 2026 Updates

## Workflows Added

### 1. android-ci-cd.yml
**CI/CD Pipeline الرئيسي**
- بناء APK تلقائي
- تشغيل الاختبارات
- فحص الـ APK
- فحص الأمان

### 2. code-quality.yml
**فحص جودة الكود**
- Ktlint (تنسيق Kotlin)
- Detekt (تحليل Kotlin)
- SpotBugs
- تقارير التغطية

### 3. release.yml
**إصدار نسخ جديدة**
- بناء Release APK
- إنشاء Release على GitHub
- رفع الملفات تلقائياً

---

## طريقة التفعيل

### 1. أنشئ المجلد
```bash
mkdir -p .github/workflows
```

### 2. انسخ الملفات
انسخ الملفات الثلاثة إلى `.github/workflows/`

### 3.تفعيل GitHub Actions
ستبدأ العمليات تلقائياً عند:
- رفع كود لـ master/main
- إنشاء Pull Request
- إنشاء tag جديد (للإصدارات)

---

## استخدام الإصدارات

لإنشاء إصدار جديد:
```bash
git tag v1.0.0
git push origin v1.0.0
```

---

## الملفات

| الملف | الوصف |
|------|-------|
| `android-ci-cd.yml` | CI/CD الأساسي |
| `code-quality.yml` | فحص الجودة |
| `release.yml` | الإصدارات التلقائية |

---

**آخر تحديث:** فبراير 2026
