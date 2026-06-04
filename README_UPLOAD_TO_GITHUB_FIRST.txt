تعليمات الرفع على GitHub
========================

بعد فك الضغط، ارفع محتويات هذا المجلد إلى GitHub كما هي.
لا ترفع الملفات منفردة بدون المجلدات.

لازم تظهر الملفات في الصفحة الرئيسية للمستودع بهذا الشكل:

app/
build.gradle
settings.gradle
codemagic.yaml
.github/
README_AR.txt

مهم جداً:
- ملف AndroidManifest.xml لا يجب أن يظهر في الصفحة الرئيسية.
- ملف MainActivity.java لا يجب أن يظهر في الصفحة الرئيسية.
- ملف styles.xml لا يجب أن يظهر في الصفحة الرئيسية.

هذه الملفات يجب أن تكون داخل:
app/src/main/AndroidManifest.xml
app/src/main/java/com/cp9rap/cashierprinter/MainActivity.java
app/src/main/res/values/styles.xml

إذا GitHub أظهر AndroidManifest.xml و MainActivity.java في الصفحة الرئيسية، فمعناه الرفع خطأ.

الأفضل ترفع من كمبيوتر أو لابتوب حتى تبقى المجلدات كما هي.
بعد الرفع، افتح Codemagic واضغط Check for configuration file ثم Start new build.
