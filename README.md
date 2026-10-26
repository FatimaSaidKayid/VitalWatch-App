# VitalWatch

Clinical Monitoring. Early Detection. Faster Response.

واجهة تجريبية (Demo) لمراقبة المرضى والتصعيد السريري، بيانات وهمية فقط - غير مخصصة للاستخدام الطبي الفعلي.
Fictional demonstration data only - not for clinical use.

## التشغيل محلياً
افتح `index.html` مباشرة في المتصفح (نقر مزدوج)، أو شغّل `python3 -m http.server 8000` ثم افتح `http://localhost:8000`.

## النشر على GitHub Pages
Settings → Pages → Source: `Deploy from a branch` → Branch: `main` / `(root)` → Save.

## كتطبيق (App)
### 1) PWA (الأسرع)
انشر المجلد على GitHub Pages (HTTPS)، ثم افتح الرابط من الجوال:
- Android/Chrome: القائمة ⋮ ← «تثبيت التطبيق».
- iPhone/Safari: مشاركة ← «إضافة إلى الشاشة الرئيسية».
يعمل بعد التثبيت بدون إنترنت (Service Worker).

### 2) ملف APK / AAB (Capacitor)
يتطلب Node 20+ و Android Studio:
```
npm install
npm run android:init     # مرة واحدة
npm run android:open     # ثم Build ← Build APK(s) من Android Studio
```
بعد أي تعديل: `npm run android:sync`.
