# **الخطة**

تم الاستعانة بالله ثم ChatGPT.

أنا أعددت هذه الخطة بنفسي لتطوير مهاراتي في الأمن السيبراني والاختراق الأخلاقي خلال **ثلاثة أشهر**. الخطة عملية ومباشرة: **مشاهدة → تطبيق → توثيق**.  
(أعتمد في الدراسة على قائمة التشغيل التي أرسلتها وعلى مسار بايثون من Elzero مع بعض قوائم تشغيل بايثون للأمن).

---

## الروابط الرئيسية التي أتبعها

- **قائمة تشغيل الاختراق (الأساسية التي أمتلكها وأتبعها):** https://www.youtube.com/playlist?list=PLMuAdKgHarVrcZCqzJFdNlTiKz66U19Xk
    
- **دورة بايثون شاملة (Elzero — تعلم بايثون من الصفر)** — المسار الذي أتبعه لأساسيات بايثون: [https://www.youtube.com/playlist?list=PLDoPjvoNmBAyE_gei5d18qkfIe-Z8mocs](https://www.youtube.com/playlist?list=PLDoPjvoNmBAyE_gei5d18qkfIe-Z8mocs). ([YouTube](https://www.youtube.com/playlist?list=PLDoPjvoNmBAyE_gei5d18qkfIe-Z8mocs&utm_source=chatgpt.com "Mastering Python - تعلم بايثون"))
    
- **قوائم تشغيل لبناء أدوات بايثون للاختبار (عربي):**
    
    - برمجة أدوات اختبار الاختراق باستخدام بايثون — Playlist. ([YouTube](https://www.youtube.com/playlist?list=PLeCT3sRYqlE68fcp3J3Q83EqzPtrQoeaa&utm_source=chatgpt.com "برمجة ادوات اختبار الاختراق باستخدام لغة البرمجة بايثون"))
        
- **مورد إنجليزي/عملي مفيد (للفترات المتقدمة):** HackerSploit — Python3 For Pentesting (مادة عملية لبناء scanners/clients). ([Class Central](https://www.classcentral.com/course/youtube-python3-for-penetration-testing-80220?utm_source=chatgpt.com "Python3 for Penetration Testing from HackerSploit"))
    

---

## الهدف

أن أكتسب معرفة عملية في: الشبكات، لينكس، اختبار تطبيقات الويب، أدوات الاختبار (Nmap, Burp, Metasploit)، والبرمجة بـ **Python** موجهة للاختراق الأخلاقي، بحيث أخرج بـ **بورتفوليو عملي** جاهز للتقديم لتدريب أو وظيفة.

---

## مخرجات متوقعة بعد 3 أشهر

- تقرير PenTest كامل واحد (PDF).
    
- 3 سكربتات Python عملية مرفوعة على GitHub (مثال: `PortScanner.py`, `NmapParser.py`, `WebFuzzer.py`).
    
- خبرة عملية على DVWA وMetasploitable2 وأدوات Kali.
    
- ملف LinkedIn محدث + سيرة ذاتية مع روابط المشاريع.
    

---

## الخطة الأسبوعية (12 أسبوع) — مدمج مع مسار بايثون (Elzero)

> **الجدول اليومي:** **3 ساعات يومياً**
> 
> - **ساعتان** لمشاهدة وتطبيق محتوى بلاي ليست الاختراق.
>     
> - **ساعة** لدراسة وتطبيق بايثون (مسار Elzero + قوائم أدوات البايثون).
>     

### الشهر الأول — الأساسيات

**أسبوع 1 — شبكات + إعداد لاب + بايثون أساسيات**

- مشاهدة (ساعتان/يوم): مقاطع الشبكات من بلاي ليست الاختراق.
    
- عملي (ساعتان/يوم): تثبيت VirtualBox + Kali + Metasploitable2 + Ubuntu وتجريب أوامر Linux الأساسية.
    
- بايثون (1 ساعة/يوم): Elzero — أساسيات (variables, loops, functions, files). تمرين: سكربت يقرأ ملف IPs ويطبعه.
    

**أسبوع 2 — Nmap + Wireshark + بايثون شبكات**

- مشاهدة: مقاطع Nmap وWireshark من البلاي ليست.
    
- عملي: مسح Nmap وتحليل حزم Wireshark.
    
- بايثون: `socket` → بناء Port Scanner بسيط وحفظ النتائج.
    

**أسبوع 3 — Burp + HTTP + بايثون أتمتة**

- مشاهدة: Burp Suite basics وHTTP.
    
- عملي: اعتراض طلبات HTTP، تثبيت DVWA وتجربة تسجيل دخول ضعيف.
    
- بايثون: `argparse`, `subprocess` → تشغيل nmap وقراءة نتائج XML/JSON.
    

**أسبوع 4 — OWASP intro + SQLi عملي + بايثون تحليل ويب**

- مشاهدة: OWASP Top10 (SQLi, XSS).
    
- عملي: تجربة SQLi يدوياً وSQLMap على DVWA.
    
- بايثون: `requests` و`re` لتحليل مخرجات HTTP.
    
- تسليم: تقرير صغير عن SQLi.
    

### الشهر الثاني — تعمق Web & أدوات (مع بايثون عملي)

**أسبوع 5 — XSS & CSRF + بايثون Web Fuzzer**

- مشاهدة: XSS, CSRF من البلاي ليست.
    
- عملي: PoC لـ XSS، Burp Repeater.
    
- بايثون: `requests` + `beautifulsoup` → بناء Web Fuzzer بسيط.
    

**أسبوع 6 — File Upload, LFI/RFI, Command Injection**

- مشاهدة: LFI/RFI وFile Upload.
    
- عملي: اختبارات File Upload وLFI على بيئة محمية.
    
- بايثون: أتمتة إرسال payloads واختبار استجابات السيرفر.
    

**أسبوع 7 — Gobuster, Nikto, Dirb + بايثون تجميع نتائج**

- مشاهدة: أدوات الاكتشاف والـ fuzzing.
    
- عملي: تشغيل Gobuster/Nikto، تحليل النتائج.
    
- بايثون: تحويل نتائج الأدوات إلى CSV/JSON وتلخيصها.
    

**أسبوع 8 — Metasploit basics + ربط بايثون بالأدوات**

- مشاهدة: Metasploit basics.
    
- عملي: استغلال Metasploitable2 والحصول على shell.
    
- بايثون: `subprocess` لربط الأدوات وقراءة النتائج تلقائيًا.
    

### الشهر الثالث — PrivEsc, Active Directory، مشروع نهائي (مع بايثون متقدّم)

**أسبوع 9 — Privilege Escalation (LinPEAS/WinPEAS)**

- مشاهدة: طرق PrivEsc، استخدام LinPEAS/WinPEAS.
    
- عملي: تجارب رفع صلاحيات على لاب.
    
- بايثون: سكربت يحلل مخرجات LinPEAS ويستخرج نقاط الضعف الممكنة.
    

**أسبوع 10 — Active Directory — enumeration basics + بايثون Recon**

- مشاهدة: AD enumeration, LDAP, مقدمة BloodHound.
    
- عملي: مختبر AD أو TryHackMe AD lab.
    
- بايثون: سكربت Recon أساسي (DNS/Subdomain enumeration).
    

**أسبوع 11 — هجمات AD متقدمة (Kerberoasting, Pass-the-Hash)**

- مشاهدة: مقاطع عملية عن Kerberoast وPass-the-Hash.
    
- عملي: تنفيذ سيناريوهات داخل مختبر محلي/منظم.
    
- بايثون: أدوات مساعدة بسيطة لجمع/تنسيق البيانات داخل المختبر.
    

**أسبوع 12 — مشروع نهائي + تجميع البورتفوليو**

- نفّذ PenTest متكامل (Recon → Scan → Exploit → PrivEsc → Report).
    
- دمج أدوات البايثون التي طورتها (PortScanner, NmapParser, WebFuzzer) في repo واحد مع README.
    
- سأسلم تقرير PDF احترافي وأرفع الأكواد على GitHub وأحدّث LinkedIn وCV.
    

---

## ملاحظات سريعة

- أطبق كل درس فورًا؛ التعلّم العملي أهم من المشاهدة فقط.
    
- أدوّن كل مشروع مع README واضح (كيفية التشغيل، المتطلبات، النتائج).
    
- أعمل دائمًا في بيئات مختبرية ومصرّح بها فقط.
    
- أنشر تقدمًا مختصرًا على LinkedIn بعد كل مشروع لرفع فرصي.
    

---
