# محمد منير · Mohammed Moneer

<p align="center">
  <b>أبني أنظمة أمنية بلغة Python — لا سكربتات عابرة.</b><br>
  <sub>تقييم ثغرات تطبيقات الأندرويد · تحليل جنائي رقمي · أدوات أمنية بالذكاء الاصطناعي</sub>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI"/>
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" alt="LangGraph"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript"/>
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js"/>
  <img src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel"/>
  <img src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP"/>
  <img src="https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white" alt="Kali"/>
  <img src="https://img.shields.io/badge/OWASP_MASVS-8B5CF6?style=for-the-badge&logo=owasp&logoColor=white" alt="OWASP MASVS"/>
</p>

---

## 🎯 المشروعان الرئيسيان

<table>
<tr>
<td width="50%" valign="top">

### 🔍 Android Vulnerability Severity MAS

نظام متعدد الوكلاء يقيّم خطورة ثغرات تطبيقات الأندرويد وفق **OWASP MASVS** —
من رفع ملف APK إلى تقريرين جاهزين (فني إنجليزي · تنفيذي عربي).

**الرقم الذي يهم:** معادلة خطورة شفّافة
`final = 0.6·base + 0.2·context + 0.2·evidence`
كل رقم قابل للتتبع إلى سطر في الكود.

- ✅ 331 اختباراً آلياً
- ✅ 42 نقطة نهاية API موثّقة
- ✅ 5 وكلاء في خط أنابيب LangGraph
- ✅ يعمل بلا إنترنت وبلا مفاتيح API

`LangGraph` `FastAPI` `Streamlit` `SQLite` `Docker` `JADX` `MobSF` `Frida`

**[→ المستودع](https://github.com/ko456123mo-jpg/android-vuln-severity-mas)**

</td>
<td width="50%" valign="top">

### 🔎 StegoNexus — Digital Forensics Workbench

منضدة عمل جنائية دفاعية تختصر عشرات الأدوات المتناثرة في واجهة واحدة:
كشف البيانات المخفية، توثيق الأدلة، وإصدار تقرير قابل للتسليم.

**ما يميّزها:** الأصل لا يُمَس أبداً — كل عملية على نسخة، وكل خطوة في سجل تدقيق،
مع سلسلة حفظ وبصمات SHA-256.

- ✅ إخفاء واستخراج في النص والصورة والصوت والفيديو والشبكة
- ✅ 17 وحدة خدمية · 22 واجهة · 8 ملفات اختبار
- ✅ 29 لقطة شاشة من تشغيل حقيقي
- ✅ AES-256-CBC + HMAC + PBKDF2

`PySide6` `scapy` `ExifTool` `Binwalk` `Steghide` `FFmpeg` `TShark`

**[→ المستودع](https://github.com/ko456123mo-jpg/stegonexus-workbench)**

</td>
</tr>
</table>

---

## 🗂 مشاريع أخرى

### [ATHAR — منصة التحقيقات الجنائية الرقمية](https://github.com/ko456123mo-jpg/ATHAR)
منصة كاملة لإدارة التحقيق الجنائي من فتح القضية إلى التقرير القابل للمراجعة:
تخزين خاص للأدلة، بصمات SHA-256، سلسلة حفظ مترابطة هاشياً، ومهام تحليل تُنفَّذ
داخل **CAINE 14.0** معزولة على VirtualBox.

**ما يميّزها:** الـAgent لا يستقبل أمر shell إطلاقاً — قائمة بيضاء صارمة على
`(tool_id, operation_key)` مع `shell=False` ومسار ثنائي ثابت ورفض أي مسار يخرج عن
مجلد الدليل للقراءة فقط.

`Laravel 13` `PHP 8.3` `MySQL` `Redis` `CAINE` `TShark` `Python` · 52 اختباراً · واجهة عربية RTL · CI أخضر

### [SentinelAI — Threat Detection & Response](https://github.com/ko456123mo-jpg/SentinelAI)
منصة كشف واستجابة موحّدة: تصنيف تدفقات الشبكة، كشف شذوذ بلا تصنيف، كشف تصيّد نصي،
تحديد عائلة برمجية خبيثة من صور بايت، وسياسة استجابة معزّزة — مدرَّبة على
CICIDS2017 وMalimg وUCI SMS Spam.
`scikit-learn` `TensorFlow` `CNN` `NLP` `Q-Learning` `Flask`

### [ZERO-X — AI Penetration Testing Platform](https://github.com/ko456123mo-jpg/zero-x-deploy)
واجهة Next.js متكاملة لمنصة اختبار اختراق بوكلاء ذكاء اصطناعي متعددين، مع بيئة
تنفيذ معزولة E2B وتقارير PDF/HTML. **نموذج أولي موثّق الحالة** — الواجهة تعمل،
وطبقة الخلفية سقالة.
`Next.js` `TypeScript` `Convex` `E2B` `OpenAI`

---

## 📊 ما أفعله فعلياً

| المجال | التفصيل |
|---|---|
| **أمن تطبيقات الجوال** | تحليل ساكن وديناميكي · JADX · MobSF · Frida · Objection · OWASP MASVS/MASTG |
| **الجنائيات الرقمية** | سلسلة حفظ · بصمات · استخراج بيانات مخفية · تحليل PCAP · تقارير منزوعة البيانات |
| **وكلاء LLM** | LangGraph · تنسيق متعدد الوكلاء · RAG · حماية من حقن البرومبت |
| **هندسة البرمجيات** | FastAPI · Laravel · عقود Pydantic · SQLAlchemy · MySQL/Redis · Docker · اختبارات آلية · CI · توثيق ثنائي اللغة |
| **تعلّم الآلة التطبيقي** | تصنيف · كشف شذوذ · CNN · NLP · تعلّم معزّز |

---

## 💼 متاح للعمل الحر

| الخدمة | ما تحصل عليه |
|---|---|
| **تقييم أمني لتطبيق أندرويد** | فحص ساكن + ديناميكي · تقييم خطورة لكل ثغرة · تقرير عربي/إنجليزي بمعيار MASVS · جلسة شرح · إعادة اختبار |
| **تحليل جنائي رقمي** | توثيق سلامة الدليل · ميتاداتا · استخراج بيانات مخفية · تقرير PDF/HTML/JSON |
| **أدوات أمنية مخصّصة** | أداة أو نظام كامل بكود نظيف + اختبارات + Docker + توثيق عربي |

📧 **moh123mon456@gmail.com**

---

## 🔐 مبادئ العمل

> - لا أفحص نظاماً بلا **تفويض كتابي** يحدد النطاق والمدة.
> - لا أدّعي شهادة لا أحملها، ولا أقدّم شهادة خبير أمام محكمة.
> - لا أحتفظ ببيانات العميل بعد التسليم.
> - عندما لا أعرف، أقول **«غير معلوم»** بدل أن أخمّن.

---

<p align="center">
  <sub>
    <a href="https://github.com/ko456123mo-jpg?tab=repositories"><b>كل المستودعات</b></a> ·
    <a href="mailto:moh123mon456@gmail.com"><b>البريد</b></a>
  </sub>
</p>
