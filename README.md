# ChatUp 💬
## چت و فایل‌شیرینگ

یک سایت ساده برای چت کردن و اشتراک‌گذاری فایل‌های بین 55 نفر.

---

## ✨ ویژگی‌ها

- ✅ **چت لحظه‌ای** - پیام‌های بی‌درنگ
- ✅ **آپلود فایل** - اشتراک‌گذاری فایل‌های مختلف
- ✅ **دستیار خودکار** - پاسخ‌های خودکار
- ✅ **واسط فارسی** - تماماً به زبان فارسی
- ✅ **رایگان** - بدون هزینه

---

## 🚀 نحوه استفاده

### 1. **GitHub Pages فعال کنید**
- به Settings → Pages بروید
- Branch رو `main` انتخاب کنید
- Save کنید

### 2. **سایت بدون Firebase (اکنون)**
- فایل `index.html` آماده است
- می‌توانید از آن استفاده کنید

### 3. **تبدیل به سایت دائمی (اختیاری)**

اگر می‌خواهید داده‌ها ذخیره شود، Firebase اضافه کنید:

#### مرحله 1: Firebase ایجاد کنید
- https://firebase.google.com بروید
- پروژه جدید ایجاد کنید
- Realtime Database فعال کنید

#### مرحله 2: کد اضافه کنید
فایل `firebase-config.js` ایجاد کنید:

```javascript
import { initializeApp } from "https://www.gstatic.com/firebasejs/9.0.0/firebase-app.js";
import { getDatabase, ref, push, onValue } from "https://www.gstatic.com/firebasejs/9.0.0/firebase-database.js";

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "your-project.firebaseapp.com",
  databaseURL: "https://your-project.firebaseio.com",
  projectId: "your-project",
  storageBucket: "your-project.appspot.com",
  messagingSenderId: "YOUR_ID",
  appId: "YOUR_APP_ID"
};

const app = initializeApp(firebaseConfig);
const database = getDatabase(app);

export { database, ref, push, onValue };
```

---

## 📦 ساختار فایل‌ها

```
chatup/
├── index.html           # صفحه اصلی سایت
├── firebase-config.js   # تنظیمات Firebase (اختیاری)
├── style.css           # طراحی (داخل HTML)
└── README.md          # این فایل
```

---

## 🔧 تنظیمات

### برای رایگان (بدون Firebase):
- داده‌ها فقط در مرورگر شما ذخیره می‌شود
- وقتی صفحه رو بسته کنید، داده‌ها حذف می‌شود

### برای دائمی (با Firebase):
- داده‌ها در سرور Firebase ذخیره می‌شود
- تا 55 نفر رایگان استفاده کنند

---

## 👥 برای 55 نفر

هر یک می‌تواند:
- 💬 پیام بفرستد
- 📁 فایل آپلود کند
- 👥 کاربران دیگر را ببیند

---

## 🎨 تنظیم رنگ‌ها

در فایل `index.html` این خط‌ها را تغییر دهید:

```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

رنگ‌های دلخواه:
- آبی: `#3498db`
- سبز: `#2ecc71`
- قرمز: `#e74c3c`

---

## 📞 کمک و پشتیبانی

اگر مشکل دارید:

1. Issues رو باز کنید: https://github.com/killer99mn/chatup/issues
2. یا به من پیام بدهید

---

## 📄 لایسنس

MIT License - آزاد برای استفاده

---

**نوشته شده با ❤️ برای شما**
