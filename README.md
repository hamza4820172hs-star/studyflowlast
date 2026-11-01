# StudyFlow — Android APK

## بناء APK من GitHub Actions

1. أنشئ Repository جديدًا على GitHub.
2. فك ضغط هذا الملف وارفع **كل الملفات والمجلدات الموجودة داخله** إلى جذر المستودع.
3. افتح تبويب **Actions** في المستودع.
4. إذا ظهر تنبيه لتفعيل GitHub Actions، وافق عليه.
5. شغّل workflow باسم **Build StudyFlow APK** من زر **Run workflow**، أو اعمل Commit/Push على فرع `main`.
6. بعد انتهاء البناء بنجاح، افتح عملية البناء الأخيرة (Run).
7. من قسم **Artifacts** حمّل `StudyFlow-debug-apk`.
8. فك ضغط ملف الـ Artifact، وستجد `app-debug.apk` جاهزًا للتثبيت على هاتف Android.

## ملاحظات
- هذا المشروع يبني نسخة **Debug APK** للتجربة والتثبيت المباشر.
- لا تحتاج إلى رفع مجلد `android`؛ GitHub Actions ينشئ مشروع Android أثناء البناء.
- معرّف التطبيق: `com.studyflow.app`.
- بيانات StudyFlow محفوظة محليًا داخل WebView؛ لا تمسح بيانات التطبيق أو تحذفه إذا كنت تريد الاحتفاظ ببياناته المحلية.
