# JSON Proxy PHP

سكربت PHP يعمل كوسيط لتحميل بيانات JSON من رابط خارجي (Codeberg) مع تجاوز مشاكل CORS.

## استخدامه

1. ارفع الملف `proxy.php` إلى أي استضافة تدعم PHP.
2. من الواجهة الأمامية (HTML أو JavaScript) استخدم الرابط بهذا الشكل:

```js
fetch("https://yourdomain.com/proxy.php")
  .then(res => res.json())
  .then(data => console.log(data));
