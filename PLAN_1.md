# PLAN_1.md

> الخطة: السنة 1 (أشهر 1–12) — تأسيس صلب، لغات أساسية، مختبر فعّال، ومخرجات قابلة للعرض

## مقدّمة

هذه النسخة من PLAN_1.md تحتوي على خطة شهرية مفصّلة للسنة الأولى بناءً على خريطتك. هدفها أن تمنحك خارطة طريق عملية لتهيئة مختبر آمن، اكتساب مهارات أساسية، وإنتاج مخرجات قابلة للنشر على GitHub/LinkedIn دون التعامل المباشر مع نشر برمجيات خبيثة.

---

## ملاحظات عامة للالتزام

* وقت يومي مستهدف: 6 ساعات عمل فعّالة، 6 أيام في الأسبوع.
* سلامة قانونية: العمل داخل بيئة معزولة فقط. لا تنفيذ أو نشر عينات خبيثة خارج مختبر معزول.
* كل مشروع يجب أن ينتج: GitHub repo (كود/أدوات مشروعة)، تقرير PDF (تحليل/ملاحظات)، وملخص LinkedIn thread.

---

## شهر 1 — إعداد شامل للمختبر + خطة سلامة

**نَتَج:** VirtualBox/VMs (Win10, Ubuntu-REMnux)، snapshots، شبكة داخلية مع NAT فقط.

**أدوات أساسية:** Ghidra, x64dbg, Procmon, Wireshark, Any.Run (استخدام بحذر)، PEStudio, Python.

**مشروع:** وثّق بيئتك (README) وارفَعها على GitHub (config فقط، لا ملفات ISO أو عينات).

**KPI:** مختبر جاهز + snapshot baseline.

---

## شهر 2 — Windows Internals (Processes, Registry, Services)

**أهداف:** فهم عملي CreateProcess, RegSetValueEx, Service Control Manager.

**مشروع:** تقرير عن سلوك برنامج شرعي (مثال: محرر نصوص) وشرح كيف يظهر في Procmon/Reg.

**KPI:** تقرير قصير + diagram.

---

## شهر 3 — Python للأمن (أتمتة، parsing)

**أدوات:** pefile, capstone, yara-python, pandas.

**مشروع:** سكربت يستخرج strings من PE ويولّد CSV/YAML بالـIOCs.

**KPI:** repo + unit tests بسيطة.

---

## شهر 4 — Assembly (x86/x64) وC basics

**أهداف:** قراءة وظائف بسيطة، stack/heap basics، calling conventions.

**مشروع:** اكتب برنامج C بسيط، وبِّن تحليلك للـassembly الناتج.

**KPI:** ملخص 10 وظائف مُفَسَّرة.

---

## شهر 5 — التحليل الثابت (Ghidra)

**أهداف:** تدفق عمل Ghidra، استخراج call graph، استخراج strings وIAT.

**مشروع:** تحليل عينة غير معبّأة ونشر تقرير static 1.

**KPI:** تقرير Markdown + IOCs.

---

## شهر 6 — التحليل الديناميكي الأساسي

**أدوات:** Procmon, Wireshark, API tracing, Process Explorer.

**مشروع:** تشغيل عينة في sandbox (theory/demo فقط) وجمع pcap + procmon log للتمارين.

**KPI:** تقرير behavioral 1 (لا يحتوي على ملفات خبيثة).

---

## شهر 7 — PE Format وIAT

**أهداف:** فهم header, sections, imports, relocations.

**مشروع:** cheat-sheet عملي للـPE internals + مثال تحليل.

**KPI:** cheat-sheet جاهز.

---

## شهر 8 — PowerShell وscript analysis (دفاعي)

**أهداف:** أنماط obfuscation، كيفية الكشف (regex, YARA).

**مشروع:** مجموعة قواعد YARA لكشف أنماط PowerShell obfuscated.

**KPI:** repo + اختبارات ضد عينات benign وسيناريوهات تحريف.

---

## شهر 9 — .NET / C# basics وdeobfuscation

**أدوات:** dnSpy, ILSpy, dotPeek.

**مشروع:** تحليل dropper .NET (مصدر مفتوح/غير خبيث) وتوثيق عمليات decompile.

**KPI:** تقرير .NET sample.

---

## شهر 10 — Packers / UPX / basic unpacking

**أهداف:** فهم كيف تعمل packers، فك UPX.

**مشروع:** أداة صغيرة لأتمتة فك UPX (Python wrapper) + doc.

**KPI:** repo + demo على binary benign.

---

## شهر 11 — شبكات (TCP, DNS, HTTP, TLS)

**أهداف:** توقيع C2 بسيط، تحليل pcap.

**مشروع:** تحليل pcap تم إنشاؤه يدوياً لسيناريو C2 HTTP بسيط، وكتابة Snort-like signatures.

**KPI:** YARA/Snort rules + تقرير.

---

## شهر 12 — تجميع ونشر أول تقرير احترافي + مراجعة سنة 1

**نَتَج:** تجميع 6–8 تقارير/مشروعات في GitHub portfolio.

**KPI:** 1 تقرير احترافي PDF، repo منظم، ملخّص LinkedIn.

---

## امتحانات دولية مقترحة للسنة 1

(مستوى دخول/أساسي — اختبارات لرفع المصداقية قبل الدخول في التخصصات الأعمق)

* CompTIA Security+ — أساسيات الأمن.
* eJPT (eLearnSecurity Junior Penetration Tester) — معرفة عامة بعمليات الاختبار.

> ملاحظة: هذه الشهادات مفيدة لبناء الثقة مع العملاء/جهات التوظيف قبل التخصص في شهادات GIAC.

---