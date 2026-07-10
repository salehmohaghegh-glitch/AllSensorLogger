
# 📱 سنسورلاگر جامع | All‑in‑One Sensor Data Logger

<div dir="rtl" align="right">

**یک ابزار تحت وب و اپلیکیشن اندرویدی برای ضبط هم‌زمان داده‌های شتاب‌سنج، ژیروسکوپ، قطبنما، میدان مغناطیسی و GPS با قابلیت ناوبری اینرسی (Dead Reckoning) و خروجی CSV.**

</div>

**A web‑based tool and Android app for simultaneously logging accelerometer, gyroscope, magnetometer, orientation and GPS data with inertial navigation (Dead Reckoning) and CSV export.**

---

## ✨ ویژگی‌ها | Features

<div dir="rtl" align="right">

- 🔄 **ضبط همزمان** داده‌های ۵ سنسور اصلی دستگاه  
- 🧭 **ناوبری اینرسی (Dead Reckoning)** با فیلتر مکمل و کالیبراسیون خودکار  
- 📊 **نمایش زنده** روی داشبورد به‌روز‌شونده  
- 📥 **خروجی CSV** استاندارد برای تحلیل در اکسل، پایتون یا متلب  
- 📱 **بدون نیاز به نصب** – فقط یک مرورگر کافیست (نسخه وب)  
- 📦 **اپلیکیشن اندروید** – قابل ساخت با Capacitor (APK)  
- 🔋 **Wake Lock** برای جلوگیری از خواب صفحه هنگام ضبط طولانی  
- 🌐 **پشتیبانی از GPS** با دقت بالا (موقعیت، سرعت، ارتفاع)  
- 🧲 **پشتیبانی از مگنتومتر** (در مرورگرهای پشتیبان)  
- 📋 **پیش‌نمایش لاگ** به‌صورت لحظه‌ای  
- ⚙️ **کالیبراسیون خودکار** بایاس شتاب‌سنج و ژیروسکوپ (۵ ثانیه)  

</div>

- 🔄 **Simultaneous logging** of 5 core device sensors  
- 🧭 **Dead Reckoning navigation** with complementary filter and auto‑calibration  
- 📊 **Live dashboard** with real‑time updates  
- 📥 **Standard CSV export** for Excel, Python or MATLAB  
- 📱 **No installation** – runs in any modern browser (web version)  
- 📦 **Android app** – buildable with Capacitor (APK)  
- 🔋 **Wake Lock API** to keep screen on during long recordings  
- 🌐 **High‑accuracy GPS** (location, speed, altitude)  
- 🧲 **Magnetometer support** (on compatible browsers)  
- 📋 **Live log preview** as data arrives  
- ⚙️ **Auto‑calibration** of accelerometer and gyroscope bias (5 seconds)  

---

## 📸 پیش‌نمایش | Screenshot

![Sensor Logger Dashboard](https://via.placeholder.com/800x400?text=Live+Screenshot+of+Sensor+Logger)

> *(تصویر واقعی را پس از اجرا جایگزین کنید)*

---

## 🚀 اجرا | Live Demo

**آدرس صفحات گیت‌هاب (پس از انتشار):**  
👉 [https://salehmohaghegh-glitch.github.io/AllSensorLogger/](https://salehmohaghegh-glitch.github.io/AllSensorLogger/)

---

## 📋 نحوه استفاده (نسخه وب) | How to Use (Web Version)

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

## 📦 ساخت اپلیکیشن اندروید (APK) | Building Android App (APK)

<div dir="rtl" align="right">

پروژه با **CapacitorJS** به اپلیکیشن اندروید تبدیل شده است. فایل‌های منبع اندروید در پوشه‌ی `android/` قرار دارند.

### پیش‌نیازها

- **Node.js** (نسخه ۱۸ یا بالاتر)
- **Java JDK 17** یا جدیدتر
- **Android Studio** با SDK Tools نصب‌شده
- **Gradle** (به‌صورت خودکار توسط Android Studio مدیریت می‌شود)

### مراحل ساخت

۱. مخزن را کلون کنید:
   ```bash
   git clone https://github.com/salehmohaghegh-glitch/AllSensorLogger.git
   cd AllSensorLogger
   ```

۲. وابستگی‌های Node.js را نصب کنید:
   ```bash
   npm install
   ```

۳. پروژه را با Capacitor همگام‌سازی کنید:
   ```bash
   npx cap sync
   ```

۴. پروژه را در Android Studio باز کنید:
   ```bash
   npx cap open android
   ```

۵. در Android Studio، از منوی **Build** → **Build Bundle(s) / APK(s)** → **Build APK(s)** را انتخاب کنید.

۶. فایل `app-debug.apk` در مسیر `android/app/build/outputs/apk/debug/` ایجاد می‌شود.

</div>

The project has been converted to an Android app using **CapacitorJS**. Android source files are located in the `android/` folder.

### Prerequisites

- **Node.js** (version 18 or higher)
- **Java JDK 17** or newer
- **Android Studio** with SDK Tools installed
- **Gradle** (managed automatically by Android Studio)

### Build Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/salehmohaghegh-glitch/AllSensorLogger.git
   cd AllSensorLogger
   ```

2. Install Node.js dependencies:
   ```bash
   npm install
   ```

3. Sync the project with Capacitor:
   ```bash
   npx cap sync
   ```

4. Open the project in Android Studio:
   ```bash
   npx cap open android
   ```

5. In Android Studio, go to **Build** → **Build Bundle(s) / APK(s)** → **Build APK(s)**.

6. The `app-debug.apk` file will be generated at `android/app/build/outputs/apk/debug/`.

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
- **[Tailwind CSS](https://tailwindcss.com/)** – استایل‌بندی سریع و واکنش‌گرا
- **DeviceMotion API** – شتاب‌سنج و ژیروسکوپ
- **DeviceOrientation API** – جهت‌گیری (آزیموت، پیچ، رول)
- **Geolocation API** – موقعیت‌یابی GPS
- **Magnetometer API** – میدان مغناطیسی (نسل جدید)
- **Wake Lock API** – جلوگیری از خاموش شدن صفحه
- **[CapacitorJS](https://capacitorjs.com/)** – تبدیل به اپلیکیشن اندروید
- **Font: Vazirmatn + Inter** – نمایش زیبا در هر دو زبان

---

## 📁 ساختار فایل‌ها | File Structure

```
Sensorlogger/
├── index.html                      # صفحه اصلی برنامه (وب)
├── android/                        # پروژه اندروید (تولیدشده توسط Capacitor)
│   ├── app/
│   │   ├── src/main/               # کدها و منابع اصلی اندروید
│   │   ├── build.gradle            # پیکربندی ماژول
│   │   └── proguard-rules.pro      # قوانین ProGuard
│   ├── gradle/wrapper/             # Gradle Wrapper
│   ├── build.gradle                # پیکربندی سطح پروژه
│   ├── settings.gradle             # تنظیمات پروژه
│   ├── gradle.properties           # ویژگی‌های Gradle
│   └── local.properties            # (محلی – به مخزن اضافه نمی‌شود)
├── capacitor.config.json           # پیکربندی Capacitor
├── package.json                    # وابستگی‌های Node.js
└── README.md                       # این فایل
```

---

## 🤝 مشارکت | Contributing

<div dir="rtl" align="right">

پیشنهادات، گزارش باگ و درخواست‌های Pull شما با خوش‌آمد گویی مواجه می‌شوند.  
لطفاً ابتدا یک **Issue** باز کنید تا دربارهٔ تغییرات مورد نظر گفت‌وگو کنیم.

</div>

Suggestions, bug reports and pull requests are very welcome.  
Please open an **Issue** first to discuss your proposed changes.

---

## 📄 مجوز | License

این پروژه تحت مجوز **MIT** منتشر شده است – استفاده، تغییر و توزیع آن آزاد است.

This project is released under the **MIT License** – free to use, modify and distribute.

---

## 🙏 سپاس‌گزاری | Acknowledgments

- الهام‌گرفته از پروژه‌های متن‌باز حوزهٔ جمع‌آوری داده‌های حرکتی  
- تشکر ویژه از توسعه‌دهندگان مرورگرها برای پیاده‌سازی APIهای سنسور  
- تشکر از تیم **CapacitorJS** برای ابزار قدرتمند تبدیل وب به اپلیکیشن موبایل

---

<div dir="rtl" align="center">

**🇮🇷 ساخته شده با ❤️ در ایران | Made with ❤️ in Iran**

</div>
```

---
