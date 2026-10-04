# guestna-video-assets

مجلد الوسائط المشترك لـ[GuestNa Video Studio](https://github.com/AbdullahDarras/guestna-video-studio): لقطات، صور، موسيقى، تسجيلات صوت. .

## كيف يُستخدم
`npm run setup` في مستودع الاستوديو يسحب هذا المستودع تلقائياً إلى `../guestna-video-assets` ويربطه بـ`public/media`. للتحديث لاحقاً: `npm run assets:update`.

## الهيكل
```
<video-name>/        مثل edu/ و app/
  ...                الملفات التي يعلنها src/videos/<video-name>/assets.json في مستودع الاستوديو
```
المصدر والرخصة لكل ملف مكتوبان في `assets.json` داخل مستودع الاستوديو (ستوك مرخّص عبر Magnific، توليد ذكاء اصطناعي، أو من جستنا).

## إضافة أصل جديد
1. ضع الملف في مجلد الفيديو المناسب هنا (`git add` ثم `commit` ثم `push`).
2. أعلنه في `assets.json` للفيديو (المسار، الوصف، المصدر).
3. `npm run assets:check` في الاستوديو.

## قواعد
- لا تحمّل من يوتيوب أو جوجل (حقوق نشر).
- الأشخاص بمظهر سعودي فقط. وثّق أي توليد بالذكاء الاصطناعي.
- حجم الملف أقل من 100 ميغا (حد GitHub). الملفات الأكبر تحتاج Git LFS.
