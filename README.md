# TestForge

**A professional toolkit for automated software testing, validation, and quality analysis.**

[English](#english) · [فارسی](#فارسی) · [Main Prompt](./PROMPT.md)

> **Want to build or test TestForge with Claude?**
> See the **[Main Prompt](./PROMPT.md)** — the complete prompt for building, testing, verifying, and documenting TestForge.

---

<a name="english"></a>

# 🇬🇧 English

## Overview

**TestForge** is a professional toolkit for testing, validating, and analyzing software projects.

It helps developers determine whether a project actually works as expected, identify and verify bugs, execute available tests, analyze failures, and generate professional test reports based on real results.

TestForge follows an evidence-based approach:

> **Test → Verify → Report**

It never treats untested functionality as working.

---

## What Is TestForge Used For?

TestForge can be used to:

* Test software functionality
* Detect and verify bugs
* Run automated tests
* Inspect project structure
* Validate important workflows
* Test edge cases and invalid inputs
* Review error handling
* Identify potential security issues
* Analyze performance where possible
* Review code quality
* Generate professional test reports

---

## Main Features

* Project inspection
* Automated testing
* Test result validation
* Bug detection and verification
* Security checks
* Performance analysis
* Test statistics
* Professional reports
* English and Persian documentation
* Clear test statuses
* Evidence-based results
* No fabricated test results

---

## Main Prompt

The repository includes the complete development prompt used to instruct Claude to build, test, verify, and document TestForge.

### [Open PROMPT.md →](./PROMPT.md)

The prompt instructs Claude to:

1. Inspect the project.
2. Build the real application.
3. Run actual tests.
4. Verify bugs.
5. Test edge cases.
6. Check security.
7. Generate reports.
8. Test TestForge itself.
9. Fix confirmed implementation problems.
10. Produce a final verification report.

> **Important:** The prompt is designed to prevent fabricated test results. Claude must clearly distinguish between `PASS`, `FAIL`, `BLOCKED`, and `NOT_TESTED`.

---

## How It Works

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

TestForge analyzes the project structure, dependencies, configuration, and important files.

### 2. Plan

Testing is based on the actual functionality of the project.

### 3. Execute

Tests are executed against the real project whenever the environment allows it.

### 4. Verify

Potential problems are reproduced and verified before being classified as confirmed bugs.

### 5. Report

TestForge generates a structured report containing the results, failures, limitations, and recommendations.

---

## Test Statuses

| Status       | Meaning                                                         |
| ------------ | --------------------------------------------------------------- |
| `PASS`       | Test was executed successfully                                  |
| `FAIL`       | Test was executed and failed                                    |
| `BLOCKED`    | Testing could not continue because of an environment limitation |
| `NOT_TESTED` | Test was not executed                                           |

TestForge must never use `PASS` for functionality that was not actually tested.

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

```bash
testforge test ./my-project
```

Use a configuration file:

```bash
testforge test ./my-project --config testforge.json
```

Generate a report:

```bash
testforge report
```

Show available commands:

```bash
testforge --help
```

> Exact commands may depend on the installed version and project configuration.

---

## Example Report

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

TestForge can identify common security concerns such as:

* Exposed API keys
* Hardcoded secrets
* Unsafe input handling
* Authentication problems
* Authorization issues
* Sensitive information exposure
* Unsafe command execution

TestForge does not perform destructive security attacks.

---

## Limitations

TestForge cannot guarantee that a project is completely free of bugs.

Testing can be limited by:

* Operating system
* Runtime environment
* Missing dependencies
* Missing credentials
* Network availability
* External services
* Unsupported platforms

When something cannot be tested, TestForge reports the limitation instead of inventing a result.

---

## Development

Clone the repository:

```bash
git clone https://github.com/far6od/testforge.git
cd testforge
```

Install the required dependencies according to the project setup instructions.

Run the tests:

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
5. Clearly describe your changes.

---

## License

TestForge is open-source software.

See [`LICENSE`](./LICENSE) for licensing information.

---

<a name="فارسی"></a>

# 🇮🇷 فارسی

## معرفی

**TestForge** یک ابزار حرفه‌ای برای **تست، اعتبارسنجی و تحلیل پروژه‌های نرم‌افزاری** است.

هدف TestForge این است که بررسی کند یک پروژه واقعاً مطابق انتظار کار می‌کند یا خیر، مشکلات را پیدا و تأیید کند و در نهایت یک گزارش حرفه‌ای بر اساس نتایج واقعی تست ارائه دهد.

اصل اصلی پروژه:

> **تست → تأیید → گزارش**

TestForge قابلیت‌هایی را که تست نشده‌اند، به‌عنوان قابلیت سالم معرفی نمی‌کند.

---

## TestForge برای چه کاری است؟

با TestForge می‌توان:

* عملکرد نرم‌افزار را تست کرد
* باگ‌ها را پیدا و تأیید کرد
* تست‌های خودکار اجرا کرد
* ساختار پروژه را بررسی کرد
* جریان‌های اصلی برنامه را آزمایش کرد
* ورودی‌های نامعتبر و حالت‌های خاص را تست کرد
* مدیریت خطاها را بررسی کرد
* مشکلات امنیتی احتمالی را شناسایی کرد
* عملکرد برنامه را در صورت امکان بررسی کرد
* کیفیت کد را تحلیل کرد
* گزارش حرفه‌ای تست ایجاد کرد

---

## قابلیت‌های اصلی

* بررسی ساختار پروژه
* اجرای تست‌های خودکار
* اعتبارسنجی نتایج
* شناسایی و تأیید باگ
* بررسی امنیتی
* تحلیل عملکرد
* آمار تست‌ها
* گزارش حرفه‌ای
* پشتیبانی از مستندات فارسی و انگلیسی
* وضعیت‌های مشخص برای تست‌ها
* جلوگیری از نتایج ساختگی

---

## پرامپت اصلی

فایل **`PROMPT.md`** شامل پرامپت کامل توسعه TestForge برای Claude است.

### [مشاهده PROMPT.md ←](./PROMPT.md)

این پرامپت به Claude دستور می‌دهد که:

1. پروژه را بررسی کند.
2. برنامه واقعی را بسازد.
3. تست‌های واقعی را اجرا کند.
4. باگ‌ها را تأیید کند.
5. حالت‌های خاص را آزمایش کند.
6. امنیت را بررسی کند.
7. گزارش ایجاد کند.
8. خود TestForge را تست کند.
9. مشکلات تأییدشده را اصلاح کند.
10. گزارش نهایی و وضعیت تأیید را ارائه دهد.

> **نکته مهم:** پرامپت طوری طراحی شده است که از ساخت نتایج آزمایشی و غیرواقعی جلوگیری کند. نتیجه هر تست باید به‌صورت واقعی `PASS`، `FAIL`، `BLOCKED` یا `NOT_TESTED` مشخص شود.

---

## TestForge چگونه کار می‌کند؟

```text
پروژه
  ↓
بررسی اولیه
  ↓
برنامه‌ریزی تست
  ↓
اجرای تست
  ↓
تأیید مشکلات
  ↓
تحلیل
  ↓
گزارش نهایی
```

### ۱. بررسی اولیه

ساختار پروژه، وابستگی‌ها، تنظیمات و فایل‌های مهم بررسی می‌شوند.

### ۲. برنامه‌ریزی

بر اساس قابلیت‌های واقعی پروژه مشخص می‌شود چه قسمت‌هایی باید تست شوند.

### ۳. اجرا

در صورت امکان، تست‌ها روی پروژه واقعی اجرا می‌شوند.

### ۴. تأیید

مشکلات احتمالی دوباره بررسی می‌شوند تا مشخص شود واقعاً مشکل هستند یا خیر.

### ۵. گزارش

نتایج تست، خطاها، محدودیت‌ها و پیشنهادهای اصلاحی در یک گزارش ساختاریافته ارائه می‌شوند.

---

## وضعیت تست‌ها

| وضعیت        | معنی                                           |
| ------------ | ---------------------------------------------- |
| `PASS`       | تست اجرا شده و موفق بوده است                   |
| `FAIL`       | تست اجرا شده و شکست خورده است                  |
| `BLOCKED`    | به دلیل محدودیت محیط امکان تست وجود نداشته است |
| `NOT_TESTED` | تست اجرا نشده است                              |

---

## سطح اهمیت باگ

| سطح        | معنی                                        |
| ---------- | ------------------------------------------- |
| `CRITICAL` | مشکل بسیار شدید یا مشکل مهم امنیتی/اطلاعاتی |
| `HIGH`     | قابلیت مهم پروژه خراب است                   |
| `MEDIUM`   | مشکل قابل توجه با امکان راه‌حل جایگزین      |
| `LOW`      | مشکل جزئی یا حالت خاص                       |
| `INFO`     | نکته یا پیشنهاد بهبود                       |

---

## نحوه استفاده

تست یک پروژه:

```bash
testforge test ./my-project
```

استفاده از فایل تنظیمات:

```bash
testforge test ./my-project --config testforge.json
```

ساخت گزارش:

```bash
testforge report
```

مشاهده راهنمای دستورات:

```bash
testforge --help
```

---

## محدودیت‌ها

TestForge نمی‌تواند تضمین کند که یک پروژه کاملاً بدون باگ است.

نتایج تست ممکن است به موارد زیر وابسته باشند:

* سیستم‌عامل
* محیط اجرا
* وابستگی‌ها
* API Keyها و اطلاعات دسترسی
* اتصال اینترنت
* سرویس‌های خارجی
* پلتفرم‌های پشتیبانی‌شده

اگر تستی قابل اجرا نباشد، TestForge آن را به‌عنوان `BLOCKED` یا `NOT_TESTED` مشخص می‌کند.

---

## توسعه

دریافت پروژه:

```bash
git clone https://github.com/far6od/testforge.git
cd testforge
```

سپس وابستگی‌های مورد نیاز را نصب کنید.

اجرای تست:

```bash
testforge test .
```

---

## مشارکت

مشارکت در توسعه TestForge آزاد است.

قبل از ارسال Pull Request:

1. تغییرات را تست کنید.
2. تست‌های لازم را اضافه یا به‌روزرسانی کنید.
3. قابلیت جدید را مستند کنید.
4. مطمئن شوید تست‌های قبلی همچنان موفق هستند.
5. تغییرات را به‌صورت واضح توضیح دهید.

---

## مجوز

TestForge یک پروژه متن‌باز است.

برای اطلاعات بیشتر به فایل [`LICENSE`](./LICENSE) مراجعه کنید.

---

## Repository Structure

```text
testforge/
├── README.md
├── PROMPT.md
├── LICENSE
└── .gitignore
```

### Important Files

| File         | Purpose                        |
| ------------ | ------------------------------ |
| `README.md`  | Project documentation          |
| `PROMPT.md`  | Main Claude development prompt |
| `LICENSE`    | Project license                |
| `.gitignore` | Files excluded from Git        |

---

## Quick Links

* **[Main Prompt →](./PROMPT.md)**
* **[License →](./LICENSE)**
* **[Issues](../../issues)**
* **[Repository](../../)**

---

**TestForge — Test it. Verify it. Report it.**
