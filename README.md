# ResearchManager

سامانه مدیریت پژوهش و پروژه‌های تحقیقاتی توسعه یافته با فریم‌ورک Django.

---

## معرفی پروژه

ResearchManager یک سامانه تحت وب برای مدیریت پژوهش‌ها، پروژه‌های تحقیقاتی و کاربران است. این پروژه با هدف یادگیری و پیاده‌سازی مفاهیم توسعه بک‌اند، مدیریت کاربران، بارگذاری فایل و استقرار پروژه با Docker توسعه داده شده است.

کاربران می‌توانند در سامانه ثبت‌نام کرده، پروفایل شخصی خود را مدیریت کنند و به اطلاعات پروژه‌های پژوهشی دسترسی داشته باشند.

---

## امکانات پروژه

* ثبت‌نام کاربران
* ورود و خروج از سیستم
* مدیریت پروفایل کاربران
* بارگذاری تصویر پروفایل
* بارگذاری تصویر کاور
* مدیریت پروژه‌های پژوهشی
* ارسال ایمیل برای کاربران
* مدیریت فایل‌های رسانه‌ای (Media)
* استفاده از متغیرهای محیطی (.env)
* استقرار با Docker و Docker Compose

---

## تکنولوژی‌های استفاده شده

### Backend

* Python
* Django

### پایگاه داده

* SQLite

### کتابخانه‌ها

* Pillow
* Python-Decouple

### DevOps

* Docker
* Docker Compose
* Git
* GitHub

---

## نصب و اجرای پروژه

### 1. دریافت پروژه

```bash
git clone https://github.com/mohammadjawid143/ResearchManager.git
cd ResearchManager
```

### 2. ساخت محیط مجازی

```bash
python -m venv env
```

فعال‌سازی در ویندوز:

```bash
env\Scripts\activate
```

فعال‌سازی در لینوکس:

```bash
source env/bin/activate
```

### 3. نصب وابستگی‌ها

```bash
pip install -r requirements.txt
```

### 4. ایجاد فایل تنظیمات

فایلی با نام `.env` در ریشه پروژه ایجاد کنید:

```env
SECRET_KEY=your_secret_key
DEBUG=True

EMAIL_HOST_USER=your_email@gmail.com
EMAIL_HOST_PASSWORD=your_app_password
```

### 5. اعمال Migration ها

```bash
python manage.py migrate
```

### 6. اجرای پروژه

```bash
python manage.py runserver
```

سپس از طریق آدرس زیر وارد شوید:

```text
http://127.0.0.1:8000
```

---

## اجرای پروژه با Docker

ساخت و اجرای کانتینر:

```bash
docker compose up --build
```

یا:

```bash
docker-compose up --build
```

---

## ساختار پروژه

```text
ResearchManager
│
├── accounts/
├── templates/
├── static/
├── media/
├── ResearchProject/
├── manage.py
├── requirements.txt
├── Dockerfile
├── docker-compose.yml
└── README.md
```

---

## اهداف پروژه

این پروژه با هدف یادگیری و تمرین موارد زیر توسعه داده شده است:

* توسعه Backend با Django
* احراز هویت کاربران
* مدیریت فایل و تصاویر
* کار با متغیرهای محیطی
* استقرار برنامه با Docker
* مدیریت نسخه با Git و GitHub

---

## توسعه‌های آینده

* مهاجرت به PostgreSQL
* پیاده‌سازی REST API
* تعریف نقش‌های مختلف کاربران
* سیستم همکاری پژوهشی
* استقرار ابری (Cloud Deployment)

---

## توسعه‌دهنده

**Mohammad Jawid Tabish**

دانشجوی مهندسی کامپیوتر و علاقه‌مند به توسعه Backend با Python و Django.
