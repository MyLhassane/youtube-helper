# YouTube Video Reader

📖 تطبيق ويب بسيط (HTML + JavaScript) يعمل عبر **GitHub Pages** ليساعد على قراءة عنوان ووصف آخر فيديو تمت مشاهدته على YouTube، مع نطق المحتوى باستخدام **Web Speech API**.

## 🎯 الهدف
المشروع مخصص لمساعدة من يجدون صعوبة في متابعة محتوى الفيديو المكتوب أو المسموع بلغة أخرى.  
يقوم بجلب بيانات الفيديو (العنوان + الوصف) مباشرة من **YouTube Data API** بعد تسجيل الدخول، ثم قراءتها صوتيًا.

## 🚀 كيفية الاستخدام
1. افتح [رابط الصفحة](https://mylhassane.github.io/youtube-helper/) (غيّر `mylhassane` إلى اسم المستخدم في GitHub).  
2. اضغط على زر **🔑 تسجيل الدخول إلى يوتيوب** (OAuth مع Google).  
3. بعد تسجيل الدخول، اضغط على زر **🎬 جلب آخر فيديو**.  
4. ستظهر تفاصيل الفيديو (العنوان + الوصف) ويتم نطقها تلقائيًا.  

## ⚙️ الإعداد
- أنشئ مشروع في [Google Cloud Console](https://console.cloud.google.com/).  
- فعّل **YouTube Data API v3**.  
- أنشئ **OAuth Client ID** من نوع **Web Application**.  
- أضف رابط GitHub Pages إلى:
  - Authorized JavaScript origins → `https://mylhassane.github.io`
  - Authorized redirect URIs → `https://mylhassane.github.io/youtube-helper/`
- انسخ **Client ID** وضعه في ملف `index.html` مكان `YOUR_CLIENT_ID`.

## 🔒 الخصوصية
- المشروع لا يخزن أي بيانات حساسة.  
- تسجيل الدخول يتم مباشرة مع Google عبر OAuth.  
- **Client ID** ليس سريًا ويمكن وضعه علنًا في الكود.  

## 🛠️ التقنيات المستخدمة
- HTML + JavaScript (Vanilla)  
- [Google APIs Client Library](https://developers.google.com/api-client-library/javascript/start)  
- YouTube Data API v3  
- Web Speech API  

---
