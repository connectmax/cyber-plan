# Week 5 — PE File Structure & Metadata Analysis

## 🎯 Objectives
- فهم بنية ملفات PE (Portable Executable) في Windows.
- استخراج المعلومات الأولية قبل التحليل العميق.
- التعرف على أهمية الـ Headers وSections.

## 📚 Learning Modules
1. **PE Format Overview:** DOS Header, NT Header, Section Table.
2. **Sections Breakdown:** .text, .rdata, .data, .rsrc.
3. **Tools:** PEStudio, PEview, CFF Explorer.

## 🧠 Quiz / Self-Test
1. ما وظيفة الـ Import Table في ملف PE؟
2. ما الفرق بين .text و .rdata؟
3. كيف يمكن معرفة الـ Compiler المستخدم من PE headers؟

## ⚔️ Real-World Story
> أثناء تحليل Ransomware “Ryuk”، اكتشف الباحثون أن الـ Import Table يحتوي فقط على دوال محدودة جدًا — إشارة إلى استخدام **Dynamic API Loading**.  
> هذا الاكتشاف غيّر منهج التحليل بالكامل.  
> **الدرس:** لا تهمل الـ Headers، فهي قد تكشف نية المبرمج الخبيث.

## 🧩 To-Do
- [ ] حلّل ملف PE نظيف وآخر مشبوه باستخدام PEStudio.
- [ ] ارسم خريطة الـ Sections في دفتر ملاحظاتك.
- [ ] سجّل مؤشرات مثل Compiler, Timestamp, Entropy.

## 🗓️ Optional Challenge
- حاول تعديل Section Header (قراءة فقط) دون كسر الملف.
