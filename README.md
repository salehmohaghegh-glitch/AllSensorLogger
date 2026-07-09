# 📱 سنسورلاگر جامع | All‑in‑One Sensor Data Logger

<div dir="rtl" align="right">

**یک ابزار تحت وب برای ضبط هم‌زمان داده‌های شتاب‌سنج، ژیروسکوپ، قطبنما، میدان مغناطیسی و GPS در مرورگر موبایل – با قابلیت خروجی CSV و نمایش زنده.**

</div>

**A web‑based tool to simultaneously log accelerometer, gyroscope, magnetometer, orientation and GPS data directly in your mobile browser – with live preview and CSV export.**

---

## ✨ ویژگی‌ها | Features

<div dir="rtl" align="right">

- 🔄 **ضبط همزمان** داده‌های ۵ سنسور اصلی دستگاه  
- 📊 **نمایش زنده** روی داشبورد به‌روز‌شونده  
- 📥 **خروجی CSV** استاندارد برای تحلیل در اکسل، پایتون یا متلب  
- 📱 **بدون نیاز به نصب** – فقط یک مرورگر کافیست  
- 🔋 **Wake Lock** برای جلوگیری از خواب صفحه هنگام ضبط طولانی  
- 🌐 **پشتیبانی از GPS** با دقت بالا (موقعیت، سرعت، ارتفاع)  
- 🧲 **پشتیبانی از مگنتومتر** (در مرورگرهای پشتیبان)  
- 📋 **پیش‌نمایش لاگ** به‌صورت لحظه‌ای  

</div>

- 🔄 **Simultaneous logging** of 5 core device sensors  
- 📊 **Live dashboard** with real‑time updates  
- 📥 **Standard CSV export** for Excel, Python or MATLAB  
- 📱 **No installation** – runs in any modern browser  
- 🔋 **Wake Lock API** to keep screen on during long recordings  
- 🌐 **High‑accuracy GPS** (location, speed, altitude)  
- 🧲 **Magnetometer support** (on compatible browsers)  
- 📋 **Live log preview** as data arrives  

---

## 📸 پیش‌نمایش | Screenshot

![Sensor Logger Dashboard](https://via.placeholder.com/800x400?text=Live+Screenshot+of+Sensor+Logger)

> *(تصویر واقعی را پس از اجرا جایگزین کنید)*

---

## 🚀 اجرا | Live Demo

**آدرس صفحات گیت‌هاب (پس از انتشار):**  
👉 [https://your-username.github.io/sensor-logger/](https://your-username.github.io/sensor-logger/)

---

## 📋 نحوه استفاده | How to Use

<div dir="rtl" align="right">

۱. فایل `index.html` را در مرورگر موبایل (کروم، فایرفاکس یا اج) باز کنید.  
۲. روی دکمه **شروع ضبط** کلیک کنید – در صورت درخواست مجوز، آن را تأیید کنید.  
۳. دستگاه را تکان دهید یا حرکت دهید تا داده‌ها ثبت شوند.  
۴. پس از اتمام، دکمه **توقف ضبط** را بزنید.  
۵. روی **دانلود CSV** کلیک کنید تا فایل داده‌ها ذخیره شود.  

</div>

1. Open `index.html` in your mobile browser (Chrome, Firefox or Edge).  
2. Tap **Start Recording** – grant sensor permissions if prompted.  
3. Move or shake your device to capture sensor data.  
4. Press **Stop Recording** when finished.  
5. Click **Download CSV** to save the logged data.

---

## 🧩 ساختار داده‌های خروجی | Output Data Structure

فایل CSV شامل ستون‌های زیر است:

| ستون | توضیح | Unit |
|------|-------|------|
| `Timestamp_ISO` | زمان ثبت به‌صورت ISO 8601 | – |
| `Accel_X/Y/Z` | شتاب خطی در سه محور | m/s² |
| `Total_Accel` | اندازه بردار شتاب کل | m/s² |
| `Gyro_X/Y/Z_Rate` | سرعت زاویه‌ای در سه محور | deg/s |
| `Azimuth/Pitch/Roll` | زوایای جهت‌گیری دستگاه | درجه |
| `Mag_Field_X/Y/Z` | میدان مغناطیسی در سه محور | µT |
| `Total_Mag_Field` | شدت کل میدان مغناطیسی | µT |
| `Latitude/Longitude` | موقعیت جغرافیایی | درجه |
| `Altitude` | ارتفاع از سطح دریا | متر |
| `Accuracy` | دقت موقعیت‌یابی | متر |
| `Heading` | جهت حرکت (آزیموت) | درجه |
| `Speed` | سرعت حرکت | m/s |

---

## 🛠 تکنولوژی‌های استفاده‌شده | Tech Stack

- **HTML5 / CSS3 / JavaScript (ES Module)**
- **[Tailwind CSS](https://tailwindcss.com/)** – برای استایل‌بندی سریع و واکنش‌گرا
- **DeviceMotion API** – شتاب‌سنج و ژیروسکوپ
- **DeviceOrientation API** – جهت‌گیری (آزیموت، پیچ، رول)
- **Geolocation API** – موقعیت‌یابی GPS
- **Magnetometer API** – میدان مغناطیسی (نسل جدید)
- **Wake Lock API** – جلوگیری از خاموش شدن صفحه
- **Font: Vazirmatn + Inter** – برای نمایش زیبا در هر دو زبان

---

## 📁 ساختار فایل‌ها | File Structure
