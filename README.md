# Fleet Navigation | مدیریت ترابری

A Persian-language, right-to-left web interface for planning and managing employee transportation. It brings route mapping, shift organization, vehicle capacity tracking, and reporting into one interface.

## Project background

Built around practical transportation workflows, the project turns day-to-day operational needs into a visual management tool. Process knowledge guided the requirements and design, with AI assistance used during development.

## Features

- Interactive maps for managing routes and stops
- Six service shifts for organizing employee transportation
- Vehicle capacity and passenger count management
- Route drawing, editing, and comparison of similar routes
- Transportation reports, Excel exports, print/PDF output, and JSON import/export

## Getting started

1. Download the repository or clone it:

   ```bash
   git clone https://github.com/Mersadkazemi9/fleet-navigation.git
   ```

2. Open `index.html` in your browser.

Without a backend, the interface starts with empty data in temporary preview mode. Changes exist only in memory and are lost when the page is reloaded. Internet access is required for external libraries, fonts, maps, and place search.

## Backend integration

This repository contains the frontend interface only. A backend and database are not included.

Persistent, shared storage requires an authenticated API on the same origin at `/api/transport/state`. The opening comment in `index.html` documents the GET/PUT contract, validation rules, authentication requirements, CSRF protection, and revision checks for concurrent updates.

## Configuration

Update `TRANSPORT_HUB` in `index.html` to set your organization's central location. The current coordinates are a sample location in Tehran.

## Technology

HTML, CSS, JavaScript, Leaflet, and SheetJS. The interface supports Persian text and right-to-left layouts.

## Public version

The public version uses generic branding and a sample hub location. It includes no preloaded operational routes.

---

## معرفی فارسی

رابط فارسی و راست‌به‌چپ برای مدیریت مسیرهای سرویس کارکنان، ایستگاه‌ها، خودروها و گزارش‌های ترابری.

## امکانات

- مدیریت مسیرها و ایستگاه‌ها روی نقشه
- تفکیک سرویس‌ها در شش شیفت
- مدیریت ظرفیت خودرو و تعداد مسافران
- ترسیم و ویرایش مسیرها و مقایسه مسیرهای مشابه
- گزارش‌ها، خروجی Excel، چاپ/PDF و ورود و خروج JSON

## اجرا

فایل `index.html` را دانلود و در مرورگر باز کنید. بدون سرور، برنامه با داده‌های خالی در حالت موقت اجرا می‌شود و تغییرات با بارگذاری مجدد از بین می‌روند. نقشه، جست‌وجو، فونت و کتابخانه‌های خارجی به اینترنت نیاز دارند.

برای استفاده با ذخیره‌سازی دائمی، یک API در همان دامنه با مسیر `/api/transport/state` لازم است. قرارداد API، احراز هویت، کنترل هم‌زمانی و اعتبارسنجی در توضیحات ابتدای `index.html` آمده است. این مخزن فقط رابط کاربری را شامل می‌شود و سرور و پایگاه داده در آن پیاده‌سازی نشده‌اند.

## تنظیم موقعیت سازمان

موقعیت `TRANSPORT_HUB` در کد، یک نقطه نمونه در تهران است. پیش از استفاده آن را با موقعیت موردنظر خود جایگزین کنید.

## درباره این نسخه

این نسخه عمومی فاقد نام، لوگو، آدرس و مختصات شرکت است و مسیرهای عملیاتی از پیش بارگذاری‌شده ندارد.

Developed by [Mersad Kazemi](https://github.com/Mersadkazemi9).
