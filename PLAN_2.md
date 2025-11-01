# PLAN_2.md

> الخطة: السنة 2 (أشهر 13–24) — RE متقدم، Memory Forensics، YARA، Go وRust، وبناء سمعة مهنية

## شهر 13 — Shellcode & Exploits (مفاهيم)

**مشروع:** تحليل shellcode تعليمي (non-malicious) وشرح عمليات التحميل.

**KPI:** ورقة صغيرة توضح تقنيات shellcode.

---

## شهر 14 — Memory Forensics (Volatility)

**أدوات:** Volatility 2/3, Rekall.

**مشروع:** استخراج IOCs من memory dump تم توليده في المختبر.

**KPI:** تقرير DFIR memory analysis.

---

## شهر 15 — Dynamic unpacking & import reconstruction

**أدوات:** Scylla, ImpRec, pe-sieve.

**مشروع:** استخراج PE مفكوك من عملية تشغيلية وإعادة بناء import table.

**KPI:** أداة خطوات قابلة لإعادة الاستخدام.

---

## شهر 16 — Threat Intelligence (MITRE ATT&CK mapping)

**مشروع:** ربط 3 تحليلات بـATT&CK وتقسيم المراحل.

**KPI:** ATT&CK mapping sheets.

---

## شهر 17 — Go: أساسيات + تحليل runtime

**أدوات:** go tool, debugging tools, demangle.

**مشروع:** بناء تطبيق Go benign ثم تحليل binary الناتج.

**KPI:** cheat-sheet «How to analyze Go binaries».

---

## شهر 18 — Rust: أساسيات + تحليل

**أدوات:** cargo, rustfilt.

**مشروع:** بناء binary Rust benign ثم دراسة demangling patterns.

**KPI:** مقال عملي عن demangling Rust.

---

## شهر 19 — Advanced RE: Kernel / Drivers (نظري)

**أهداف:** فهم Windows driver model نظريًا، وكيفية تحليل drivers بأمان (لا تنفيذ على host).

**KPI:** cheat-sheet drivers analysis (theory).

---

## شهر 20 — Automation: YARA/Sigma pipeline

**مشروع:** pipeline تلقائي يجمع عينات جديدة، يفحصها بـYARA، ويصدر تقارير تلقائية.

**KPI:** automation repo + CI tasks.

---

## شهر 21 — C2 Protocol analysis (HTTP, DNS tunneling)

**مشروع:** كتابة walkthrough لتحليل C2 يستخدم DNS tunneling (باستخدام pcaps تم إنشاؤها بنفسك).

**KPI:** detection rules + pcap samples (synthetic).

---

## شهر 22 — Mobile malware (Android)

**أدوات:** apktool, jadx, mobSF.

**مشروع:** تحليل APK مفتوح المصدر مع توثيق السلوك.

**KPI:** تقرير mobile 1.

---

## شهر 23 — Supply chain threats & SBOM

**مشروع:** دراسة حالة supply-chain (تحليل compromise لمشروع مفتوح المصدر).

**KPI:** writeup + remediation checklist.


---

## شهر 24 — سنة 2 review + بدء التقديم على وظائف بعيدة

**نَتَج:** 12–18 تحليلًا عامة/متقدمة منشورة.

**KPI:** 1–2 عقود مدفوعة صغيرة + LinkedIn outreach.

---

## امتحانات دولية مقترحة للسنة 2

* GIAC GREM (GIAC Reverse Engineering Malware) — شهادة متخصصة في تحليل البرمجيات الخبيثة.
* GIAC GCTI (GIAC Cyber Threat Intelligence) — متقدمة في الاستخبارات.
* OSCP (Offensive Security Certified Professional) — مفيد جداً لخبرة hands-on حتى لو ليست متخصصة Malware.

> يُنصح بأخذ GREM بعد إتمام 18 شهرًا عندما تكون comfortable مع RE الديناميكي والثابت.

---