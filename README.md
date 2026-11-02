# EventPass

منصة لإنشاء دعوات إلكترونية للمناسبات باستخدام React وNode.js وPostgreSQL.

## التشغيل

1. ثبّت Node.js وPostgreSQL.
2. نفّذ `npm install` في المجلد الرئيسي.
3. نفّذ `npm install` داخل `client` وداخل `server`.
4. انسخ `server/.env.example` إلى `server/.env` وضع بيانات قاعدة البيانات ومفتاح JWT.
5. من داخل `server` نفّذ:
   - `npx prisma generate`
   - `npx prisma migrate dev --name init`
6. من المجلد الرئيسي نفّذ `npm run dev`.

واجهة الموقع تعمل على `http://localhost:5173` والـ API على `http://localhost:4000`.

## إعداد قاعدة البيانات

عدّل `DATABASE_URL` في `server/.env` إلى رابط PostgreSQL الخاص بك. لا تضع أسرار قاعدة البيانات في ملفات الواجهة أو GitHub.
