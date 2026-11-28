# ONYXIA EA — Installation & Setup Guide

This guide covers the public ONYXIA EA v1.11 package for MetaTrader 5.

[Download the latest release](https://github.com/Onyxia-ea/onyxia-licenses/releases/latest) · [Back to repository](../README.md)

---

## English

### 1. Download and extract

1. Open the [ONYXIA EA Releases page](https://github.com/Onyxia-ea/onyxia-licenses/releases).
2. Download the archive attached to the release. The v1.11 asset is a **RAR** file.
3. Extract the archive with a compatible archive utility.

### 2. Install the Expert Advisor

1. Open MetaTrader 5.
2. Select **File → Open Data Folder**.
3. Open the <code>MQL5</code> folder, then open <code>Experts</code>.
4. Copy <code>ONYXIA EA.ex5</code> into that folder.
5. Return to MetaTrader 5.
6. In **Navigator**, right-click **Expert Advisors** and choose **Refresh**, or restart the terminal.
7. Find ONYXIA EA and attach it to the required chart.

### 3. Enable automatic license renewal and update notices

1. In MetaTrader 5, open **Tools → Options → Expert Advisors**.
2. Enable **Allow WebRequest for listed URL**.
3. Add the following address to the list:

   <code>https://raw.githubusercontent.com</code>

4. Confirm the settings.

If this permission is not enabled, automatic license renewal and update notices may not work. Where the EA offers a manual license-file fallback, obtain the updated license file through official ONYXIA support and place it in:

<code>MQL5/Files</code>

Do not download or use license files from unofficial sources.

### 4. Enable About-window actions

If you need the actions displayed in the EA's About window (for example, Download / Update, Copy ID and support shortcuts):

1. Open the EA properties.
2. Select the **Common** tab.
3. Enable **Allow DLL imports**.
4. Confirm that you are using the official ONYXIA EA package.

This is a separate setting from WebRequest. WebRequest is used for communication with the ONYXIA service; DLL permission enables the relevant About-window actions.

### 5. First launch checklist

- Confirm that ONYXIA EA appears in **Navigator → Expert Advisors**.
- Attach it to the intended chart.
- Review the EA inputs before enabling trading.
- Check the terminal's **Experts** and **Journal** tabs if something does not work as expected.
- Test the setup on a demo account before using it in a live environment.

### Troubleshooting

| Symptom | What to check |
|---|---|
| ONYXIA EA is not visible in Navigator | Confirm the file is in <code>MQL5/Experts</code>, then refresh Navigator or restart MT5. |
| License does not renew automatically | Confirm WebRequest is enabled and <code>https://raw.githubusercontent.com</code> is in the allowed list. |
| About-window actions are unavailable | Check **Allow DLL imports** in the EA's **Common** tab. |
| The EA does not behave as expected | Review the Experts and Journal logs, input settings and current terminal permissions. Contact official support with a description of the issue. |

---

## فارسی

### ۱. دانلود و استخراج فایل

1. وارد صفحه [انتشار نسخه‌های ONYXIA EA](https://github.com/Onyxia-ea/onyxia-licenses/releases) شوید.
2. فایل پیوست نسخه موردنظر را دانلود کنید. فایل نسخه v1.11 با فرمت **RAR** منتشر شده است.
3. فایل فشرده را با نرم‌افزار سازگار با RAR استخراج کنید.

### ۲. نصب اکسپرت در متاتریدر ۵

1. متاتریدر ۵ را باز کنید.
2. از منوی **File → Open Data Folder** وارد پوشه اطلاعات متاتریدر شوید.
3. وارد پوشه <code>MQL5</code> و سپس <code>Experts</code> شوید.
4. فایل <code>ONYXIA EA.ex5</code> را در این پوشه کپی کنید.
5. به متاتریدر برگردید.
6. در پنجره **Navigator** روی بخش **Expert Advisors** راست‌کلیک کرده و **Refresh** را انتخاب کنید؛ یا متاتریدر را ببندید و دوباره اجرا کنید.
7. اکسپرت ONYXIA EA را پیدا کرده و روی چارت موردنظر قرار دهید.

### ۳. فعال‌سازی ارتباط آنلاین برای تمدید خودکار لایسنس

1. در متاتریدر وارد مسیر **Tools → Options → Expert Advisors** شوید.
2. گزینه **Allow WebRequest for listed URL** را فعال کنید.
3. آدرس زیر را به فهرست آدرس‌های مجاز اضافه کنید:

   <code>https://raw.githubusercontent.com</code>

4. تنظیمات را تأیید کنید.

در صورت غیرفعال‌بودن این دسترسی، تمدید خودکار لایسنس و اعلان‌های آپدیت ممکن است کار نکنند. اگر نسخه اکسپرت امکان استفاده از فایل لایسنس دستی را ارائه می‌کند، فایل به‌روزشده را فقط از پشتیبانی رسمی ONYXIA دریافت و در مسیر زیر قرار دهید:

<code>MQL5/Files</code>

از فایل‌های لایسنس دریافت‌شده از منابع غیررسمی استفاده نکنید.

### ۴. فعال‌سازی دکمه‌های پنجره About

برای استفاده از دکمه‌هایی مانند Download / Update، Copy ID و میانبرهای پشتیبانی:

1. پنجره تنظیمات اکسپرت را باز کنید.
2. وارد تب **Common** شوید.
3. گزینه **Allow DLL imports** را فعال کنید.
4. مطمئن شوید فایل رسمی ONYXIA EA را نصب کرده‌اید.

توجه کنید که این گزینه با WebRequest متفاوت است؛ WebRequest برای ارتباط با سرویس ONYXIA استفاده می‌شود و DLL imports امکان استفاده از برخی دکمه‌های پنجره About را فراهم می‌کند.

### ۵. بررسی اولیه پس از نصب

- بررسی کنید ONYXIA EA در مسیر **Navigator → Expert Advisors** نمایش داده شود.
- اکسپرت را روی چارت موردنظر قرار دهید.
- پیش از فعال‌کردن معاملات، ورودی‌ها و تنظیمات ریسک را بررسی کنید.
- در صورت بروز مشکل، تب‌های **Experts** و **Journal** را بررسی کنید.
- پیش از استفاده در حساب واقعی، نصب و تنظیمات را روی حساب آزمایشی بررسی کنید.

### عیب‌یابی

| مشکل | موردی که باید بررسی شود |
|---|---|
| اکسپرت در Navigator دیده نمی‌شود | مسیر <code>MQL5/Experts</code> و Refresh یا راه‌اندازی مجدد متاتریدر را بررسی کنید. |
| لایسنس خودکار تمدید نمی‌شود | فعال‌بودن WebRequest و ثبت آدرس <code>https://raw.githubusercontent.com</code> را بررسی کنید. |
| دکمه‌های پنجره About نمایش داده نمی‌شوند | گزینه **Allow DLL imports** در تب **Common** را بررسی کنید. |
| اکسپرت درست کار نمی‌کند | گزارش‌های Experts و Journal، تنظیمات ورودی و مجوزهای ترمینال را بررسی کنید. |

### ارتباط با پشتیبانی رسمی

- کانال تلگرام: [@onyxia_ea](https://t.me/onyxia_ea)
- پشتیبانی: [@OnyxiaEA_Support](https://t.me/OnyxiaEA_Support)
- ربات لایسنس: [@OnyxiaEA_Bot](https://t.me/OnyxiaEA_Bot)
- ایمیل: [onyxiaea@gmail.com](mailto:onyxiaea@gmail.com)

**نکته امنیتی:** شناسه دستگاه (Device ID)، فایل لایسنس، اطلاعات حساب و تصاویر خصوصی را در Issue یا Comment عمومی GitHub منتشر نکنید. این اطلاعات را فقط از مسیرهای رسمی پشتیبانی ارسال کنید.

---

## Important notes

- ONYXIA EA is a trading tool, not a promise of returns. Trading involves risk.
- Keep the EA inputs and risk settings under your control.
- Do not edit files under <code>licenses/</code>, <code>update.txt</code> or <code>.gitattributes</code> in this repository. They are part of the license and update delivery workflow.
