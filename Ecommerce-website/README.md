# AI E-Commerce

مشروعي لنيل درجة البكالوريوس – جامعة العلوم والتكنولوجيا  
يهدف هذا المشروع إلى دمج تقنيات الذكاء الاصطناعي مع متجر إلكتروني لتحسين تجربة المستخدم وتطوير عمليات البيع والإدارة.

قم بتحميل المشروع من الرابط التالي : https://github.com/Esmailx/ai-ecommerce/releases/tag/v1.0.0



## خطوات تشغيل المشروع
 ## اولا 
 قم بتحميل المشروع من الرابط التالي : https://github.com/Esmailx/ai-ecommerce/releases/tag/v1.0.0 
 
 ## ثانيا

- نحتاج إلى تنزيل برنامج XAMPP لتشغيل المشروع على خادم محلي.

- نضع مجلد المشروع `ecommerce` داخل المجلد `htdocs` الموجود في مسار تثبيت برنامج XAMPP.

- نفتح برنامج XAMPP ونشغّل:
  - خادم Apache
  - قاعدة البيانات MySQL

- نفك الضغط عن قاعدة البيانات الموجودة في الملف `wp-ecommerce.zip`.

- لرفع قاعدة البيانات على الخادم المحلي:
  1. ننشئ قاعدة بيانات باسم `wp-ecommerce`.
  2. نفتح موجه الأوامر (Command Prompt).
  3. ننفذ الأمر التالي:

  mysql -u root -p -h localhost -D wp-ecommerce < wp-ecommerce.sql

- الآن لتشغيل خادم Flask، نتجه إلى مجلد `flask_api` ونقوم بتثبيت متطلبات المشروع:

  pipenv install -r requirements.txt

- نفتح موجه الأوامر داخل مسار مجلد `flask_api` ونفعل البيئة الافتراضية:

  pipenv shell

- لتشغيل خادم Flask ننفذ الأمر:

  flask --app store_api run

- بعد ذلك يصبح المشروع جاهزًا للتشغيل، نفتح المتصفح وندخل الرابط:

  localhost/ecommerce/

- لفتح لوحة تحكم المتجر ننتقل إلى الرابط:

  localhost/ecommerce/wp-admin

  بيانات الدخول:
  - e-mail: admin@admin.com
  - password: Admin123456?

- للتوجه إلى صفحة تقنيات الذكاء الاصطناعي نستخدم الرابط:

  localhost/ecommerce/manger

