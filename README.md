# TestForge

**Automated Project Testing & Validation Toolkit**

[English](#english) · [فارسی](#فارسی)

---

<a name="english"></a>

# 🇬🇧 English

## Overview

**TestForge** is a professional toolkit for testing, validating, and analyzing software projects.

It is designed to help developers verify whether a project actually works as expected, identify bugs, analyze failures, and produce clear test reports based on real test results.

TestForge focuses on **evidence-based testing** rather than assumptions.

## What Is TestForge Used For?

TestForge can be used to:

* Test software functionality
* Detect and verify bugs
* Run automated tests
* Analyze project structure
* Validate important user workflows
* Test edge cases and invalid inputs
* Review error handling
* Identify potential security issues
* Analyze performance where possible
* Review code quality
* Generate professional test reports
* Distinguish confirmed problems from untested or unconfirmed issues

### Core Principle

> **Test it. Verify it. Report it.**

TestForge never treats untested functionality as working.

---

## Key Features

* 🔍 Project inspection
* 🧪 Automated testing
* ✅ Test result validation
* 🐛 Bug detection and verification
* 🔐 Security checks
* ⚡ Performance analysis
* 📊 Test statistics
* 📝 Professional test reports
* 🌐 English and Persian documentation
* 🛑 Clear `PASS`, `FAIL`, `BLOCKED`, and `NOT TESTED` states
* 🚫 No fabricated test results

---

## How It Works

TestForge follows a structured testing process:

```text
Project
   ↓
Inspection
   ↓
Test Planning
   ↓
Execution
   ↓
Bug Verification
   ↓
Analysis
   ↓
Final Report
```

### 1. Inspect

TestForge first analyzes the project structure, dependencies, configuration, and important files.

### 2. Plan

It determines which parts of the project should be tested based on the project's actual functionality.

### 3. Execute

Tests are executed against the real project whenever the environment allows it.

### 4. Verify

Potential problems are reproduced and verified before being classified as confirmed bugs.

### 5. Report

A final report summarizes the results, failures, limitations, and recommendations.

---

## Test Results

TestForge uses four primary statuses:

| Status       | Meaning                                                         |
| ------------ | --------------------------------------------------------------- |
| `PASS`       | The test was executed and passed                                |
| `FAIL`       | The test was executed and failed                                |
| `BLOCKED`    | Testing could not continue because of an environment limitation |
| `NOT TESTED` | The test was not executed                                       |

This prevents assumptions from being presented as test results.

---

## Bug Severity

| Severity   | Description                                   |
| ---------- | --------------------------------------------- |
| `CRITICAL` | Severe failure or major security/data problem |
| `HIGH`     | Important functionality is broken             |
| `MEDIUM`   | Significant issue with a possible workaround  |
| `LOW`      | Minor issue or edge case                      |
| `INFO`     | Observation or improvement suggestion         |

---

## Example Usage

After installing and configuring TestForge, run:

```bash
testforge test ./my-project
```

For a specific test configuration:

```bash
testforge test ./my-project --config testforge.json
```

To generate a report:

```bash
testforge report
```

To view available commands:

```bash
testforge --help
```

> The exact commands may depend on the installed version and project configuration.

---

## Example Test Report

```text
TestForge Report
────────────────────────────

Project: ExampleProject

Overall Status: PASS WITH ISSUES

Tests:
  Total:       42
  Passed:      37
  Failed:       3
  Blocked:      1
  Not Tested:   1

Critical: 0
High:     1
Medium:   2
Low:      0

Final Verdict:
Core functionality is operational, but several
issues require attention.
```

---

## Security

TestForge is designed to identify common security concerns such as:

* Exposed API keys
* Hardcoded secrets
* Unsafe input handling
* Authentication problems
* Authorization issues
* Sensitive information exposure
* Unsafe command execution

TestForge does **not** perform destructive security attacks.

---

## Important Limitations

TestForge does not claim that a project is completely bug-free.

Testing is limited by:

* Available dependencies
* Operating system
* Runtime environment
* Missing credentials
* Network availability
* Unsupported platforms
* External services

When something cannot be tested, TestForge reports the limitation instead of inventing a result.

---

## Development

Clone the repository:

```bash
git clone https://github.com/far6od/testforge.git
cd testforge
```

Install the required dependencies according to the project's setup instructions.

Run the test suite:

```bash
testforge test .
```

---

## Contributing

Contributions are welcome.

Before submitting a pull request:

1. Test your changes.
2. Add or update relevant tests.
3. Document new functionality.
4. Make sure existing tests continue to pass.
5. Clearly describe the changes.


---

<a name="فارسی"></a>

# 🇮🇷 فارسی

## معرفی

**TestForge** یک ابزار حرفه‌ای برای **تست، اعتبارسنجی و تحلیل پروژه‌های نرم‌افزاری** است.

هدف آن این است که بررسی کند یک پروژه واقعاً مطابق انتظار کار می‌کند یا خیر، مشکلات را پیدا و تأیید کند و در نهایت یک گزارش حرفه‌ای و قابل اعتماد از نتایج تست ارائه دهد.

تمرکز TestForge بر **تست واقعی و مبتنی بر شواهد** است، نه حدس و فرض.

## TestForge برای چه کاری است؟

با TestForge می‌توان:

* عملکرد نرم‌افزار را تست کرد
* باگ‌ها را پیدا و تأیید کرد
* تست‌های خودکار اجرا کرد
* ساختار پروژه را بررسی کرد
* جریان‌های اصلی استفاده از برنامه را آزمایش کرد
* ورودی‌های نامعتبر و حالت‌های خاص را تست کرد
* مدیریت خطاها را بررسی کرد
* مشکلات امنیتی احتمالی را شناسایی کرد
* عملکرد برنامه را در صورت امکان بررسی کرد
* کیفیت کد را تحلیل کرد
* گزارش حرفه‌ای تست ایجاد کرد
* مشکلات تأییدشده را از موارد تست‌نشده جدا کرد

### اصل اصلی

> **تست کن، تأیید کن، گزارش بده.**

TestForge هیچ قابلیت تست‌نشده‌ای را به‌عنوان قابلیت سالم معرفی نمی‌کند.

---

## قابلیت‌های اصلی

* 🔍 بررسی ساختار پروژه
* 🧪 اجرای تست‌های خودکار
* ✅ اعتبارسنجی نتایج
* 🐛 شناسایی و تأیید باگ
* 🔐 بررسی‌های امنیتی
* ⚡ تحلیل عملکرد
* 📊 آمار تست‌ها
* 📝 گزارش حرفه‌ای
* 🌐 مستندات فارسی و انگلیسی
* 🛑 وضعیت‌های `PASS`، `FAIL`، `BLOCKED` و `NOT TESTED`
* 🚫 جلوگیری از تولید نتایج ساختگی

---

## TestForge چگونه کار می‌کند؟

روند کلی به شکل زیر است:

```text
پروژه
  ↓
بررسی اولیه
  ↓
طراحی برنامه تست
  ↓
اجرای تست
  ↓
تأیید مشکلات
  ↓
تحلیل نتایج
  ↓
گزارش نهایی
```

### ۱. بررسی اولیه

ساختار پروژه، وابستگی‌ها، تنظیمات و فایل‌های مهم بررسی می‌شوند.

### ۲. برنامه‌ریزی تست

بر اساس قابلیت‌های واقعی پروژه مشخص می‌شود چه قسمت‌هایی باید تست شوند.

### ۳. اجرای تست

در صورت امکان، تست‌ها روی خود پروژه واقعی اجرا می‌شوند.

### ۴. تأیید

مشکلات احتمالی تا حد امکان دوباره اجرا و بررسی می‌شوند تا مشخص شود واقعاً باگ هستند یا خیر.

### ۵. گزارش نهایی

در پایان، نتیجه تست‌ها، خطاها، محدودیت‌ها و پیشنهادهای اصلاحی ارائه می‌شود.

---

## وضعیت نتایج

| وضعیت        | معنی                                           |
| ------------ | ---------------------------------------------- |
| `PASS`       | تست اجرا شده و موفق بوده است                   |
| `FAIL`       | تست اجرا شده و با شکست مواجه شده است           |
| `BLOCKED`    | به دلیل محدودیت محیط امکان تست وجود نداشته است |
| `NOT TESTED` | تست اجرا نشده است                              |

---

## سطح اهمیت باگ‌ها

| سطح        | معنی                                        |
| ---------- | ------------------------------------------- |
| `CRITICAL` | مشکل بسیار شدید یا مشکل مهم امنیتی/اطلاعاتی |
| `HIGH`     | قابلیت مهم پروژه خراب است                   |
| `MEDIUM`   | مشکل قابل توجه با امکان وجود راه‌حل جایگزین |
| `LOW`      | مشکل جزئی یا مربوط به حالت خاص              |
| `INFO`     | پیشنهاد یا نکته بهبود                       |

---

## نحوه استفاده

بعد از نصب و تنظیم TestForge می‌توانید پروژه را تست کنید:

```bash
testforge test ./my-project
```

برای استفاده از تنظیمات مشخص:

```bash
testforge test ./my-project --config testforge.json
```

برای ساخت گزارش:

```bash
testforge report
```

برای مشاهده راهنمای دستورات:

```bash
testforge --help
```

> دستورات دقیق ممکن است با توجه به نسخه و تنظیمات پروژه متفاوت باشند.

---

## نمونه گزارش

```text
TestForge Report
────────────────────────────

Project: ExampleProject

Overall Status: PASS WITH ISSUES

Tests:
  Total:       42
  Passed:      37
  Failed:       3
  Blocked:      1
  Not Tested:   1

Critical: 0
High:     1
Medium:   2
Low:      0

Final Verdict:
Core functionality is operational, but several
issues require attention.
```

---

## امنیت

TestForge می‌تواند مواردی مانند موارد زیر را بررسی کند:

* API Keyهای قابل مشاهده
* Secretهای قرارگرفته در کد
* مدیریت ناامن ورودی
* مشکلات احراز هویت
* مشکلات سطح دسترسی
* افشای اطلاعات حساس
* اجرای ناامن دستورات

TestForge برای تست امنیتی، عملیات مخرب یا تخریبی انجام نمی‌دهد.

---

## محدودیت‌ها

TestForge نمی‌تواند تضمین کند که یک پروژه کاملاً بدون باگ است.

نتایج تست ممکن است به موارد زیر وابسته باشند:

* وابستگی‌های موجود
* سیستم‌عامل
* محیط اجرا
* اطلاعات ورود و API Keyها
* اتصال اینترنت
* سرویس‌های خارجی
* پلتفرم‌های پشتیبانی‌شده

اگر تستی امکان اجرا نداشته باشد، TestForge آن را به‌عنوان `BLOCKED` یا `NOT TESTED` گزارش می‌کند و نتیجه ساختگی تولید نمی‌کند.

---

## توسعه

دریافت پروژه:

```bash
git clone https://github.com/far6od/testforge.git
cd testforge
```

سپس وابستگی‌های مورد نیاز پروژه را نصب کنید.

برای اجرای تست:

```bash
testforge test .
```

---

## مشارکت

مشارکت در توسعه TestForge آزاد است.

قبل از ارسال Pull Request:

1. تغییرات خود را تست کنید.
2. تست‌های مربوطه را اضافه یا به‌روزرسانی کنید.
3. قابلیت جدید را مستند کنید.
4. مطمئن شوید تست‌های قبلی همچنان موفق هستند.
5. تغییرات را به‌صورت واضح توضیح دهید.


---

## Support

For questions, bug reports, or feature requests, open an issue in the GitHub repository.

برای پرسش، گزارش باگ یا پیشنهاد قابلیت جدید، یک Issue در مخزن GitHub ایجاد کنید.
