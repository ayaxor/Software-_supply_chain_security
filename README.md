

<p align="center">
  <img src="https://raw.githubusercontent.com/ayaxor/Software-_supply_chain_security/main/file_00000000473471f5a72bef07c06e5754.png" width="750">
</p>

<h1 align="center">🔐 Software Supply Chain Security  
QuietWire AI Training Program – Phase 2</h1>

<p align="center">
Developed by <b>Eng. Aya Jamal</b>  
Under the supervision of <b>Eng. Ashraf Al-Haj</b> and <b>Chris Blask</b>  
QuietWire AI Training Program
</p>

---

# 🌍 1. Overview (English)

Software Supply Chain Security is the practice of protecting every component, process, and dependency involved in building, packaging, and delivering software.  

Modern software systems rely heavily on:
- Open-source libraries  
- Third-party APIs  
- CI/CD pipelines  
- Cloud infrastructure  
- Automated build tools  

This creates a **large attack surface**, meaning that an attacker doesn’t need to hack your system directly—  
they can simply compromise a dependency you trust.

---

# 💣 2. Why Supply Chain Attacks Are Dangerous

Supply chain attacks are considered **one of the most powerful cyberattacks** because:

### ✔️ They spread through trusted channels  
A simple malicious update can infect thousands of organizations.

### ✔️ They are extremely hard to detect  
Hackers hide inside legitimate processes.

### ✔️ They scale massively  
One compromised package = global impact.

### ✔️ Real incidents shook the world:
- **SolarWinds** (affected U.S. government + 18,000 organizations)  
- **Log4j** (affected millions of systems)  
- **Codecov Bash Uploader breach**  
- **NPM “event-stream” backdoor attack**  

These incidents changed cybersecurity forever.

---

# 🏗️ 3. Anatomy of the Software Supply Chain

A typical software supply chain includes:

### 🔧 **1. Code Development**
- Developers  
- IDEs  
- Source code  
- Version control (GitHub, GitLab)

### 📦 **2. Dependencies**
- NPM packages  
- PyPI libraries  
- Docker containers  
- OS packages (Debian, RPM)

### 🏭 **3. Build Systems**
- Compilers  
- Build servers  
- Automated scripts

### 🚀 **4. CI/CD Pipelines**
- GitHub Actions  
- Jenkins  
- GitLab CI

### ☁️ **5. Deployment**
- Cloud services  
- Kubernetes  
- On-prem servers

Each point is a potential attack vector.

---

# ⚠️ 4. Key Risks in the Software Supply Chain

### 🧨 1. Malicious Dependencies  
Attackers upload trusted-looking but infected packages.

### 🎭 2. Dependency Confusion  
Hackers upload packages with the same name to public registries.

### 🐍 3. Typosquatting  
Example:  
Instead of `requests` → user installs `reqeusts`

### 🛠️ 4. Compromised Build Servers  
If the build system is infected, every release becomes infected.

### 🔑 5. Stolen Developer Credentials  
Hackers publish malicious code through a trusted developer account.

### 🔃 6. Tampered Updates  
Attackers modify packages downloaded during updates.

---

# 🛡️ 5. Core Security Controls

### 🧱 Zero-Trust Development  
Never trust any component by default.

### 📝 SBOM — Software Bill of Materials  
A full list of all dependencies in your software.

### 🔍 Continuous Dependency Scanning  
Tools like:
- Snyk  
- Dependabot  
- Trivy  

### 🔑 Code Signing  
Ensures the code hasn't been altered.

### 🧪 Secure CI/CD Pipelines  
- Secrets protection  
- Build isolation  
- Immutable runners  

### 🔐 Least Privilege Access  
Every developer and service gets only the required permissions.

---

# 🇸🇦 **النسخة العربيـــــة (Arabic Version)**

# 🌍 1. نظرة عامة

أمن سلسلة توريد البرمجيات هو مجال يركّز على حماية **جميع العناصر** التي تدخل في صناعة البرمجيات، مثل:

- المكتبات الخارجية  
- التبعيات  
- أدوات البناء  
- خطوط CI/CD  
- الخدمات السحابية  

أي اختراق لأي جزء منها قد يؤدي إلى **كارثة أمنية**.

---

# 💣 2. لماذا هجمات سلسلة التوريد خطيرة؟

### ✔️ لأنها تنتشر عبر تحديثات موثوقة  
تصيب آلاف الأنظمة مرة واحدة.

### ✔️ لأن اكتشافها صعب  
تندمج مع العمليات الطبيعية للنظام.

### ✔️ لأنها تؤثر عالميًا  
هجوم واحد قد يضرب العالم كله.

### ✔️ أمثلة حقيقية:
- هجوم **SolarWinds**  
- ثغرة **Log4j**  
- اختراق **Codecov**  
- حزمة NPM مزوّرة (**event-stream**)  

---

# 🏗️ 3. مكوّنات سلسلة التوريد

### 1. التطوير  
الكود – الحسابات – المستودعات – GitHub

### 2. التبعيات  
حزم NPM – مكتبات Python – حاويات Docker…

### 3. أنظمة البناء  
المترجمات – خوادم البناء – السكربتات

### 4. خطوط CI/CD  
GitHub Actions – Jenkins…

### 5. النشر  
الخوادم – السحابة – Kubernetes

---

# ⚠️ 4. المخاطر الأساسية

### 🧨 التبعيات الخبيثة  
تحميل مكتبة مصابة دون العلم.

### 🎭 هجوم “الاعتماد المربك”  
رفع مكتبة باسم مشابه للمكتبة الحقيقية.

### 🐍 الأخطاء الإملائية  
تثبيت مكتبة مزيفة بسبب حرف واحد.

### 🔧 خوادم البناء المخترقة  
كل إصدار يصبح مصابًا.

### 🔑 سرقة حسابات المطورين  
رفع كود خبيث من حساب موثوق.

---

# 🛡️ 5. أساليب الحماية الأساسية

### 🧱 مبدأ انعدام الثقة  
عدم الثقة بأي عنصر إلا بعد التحقق منه.

### 📜 إنشاء SBOM  
قائمة تفصيلية بجميع التبعيات.

### 🔍 الفحص المستمر  
Dependabot – Snyk – Trivy

### 🔐 توقيع الكود  
لضمان عدم التلاعب به.

### ⚙️ تأمين خطوط CI/CD  
عزل – حماية الأسرار – مراقبة مستمرة.

### 🚫 أقل قدر من الصلاحيات  
منع الوصول الزائد.

---

# 🏆 Credits
**Developer:** Eng. Aya Jamal  
**Supervisors:** Eng. Ashraf Al-Haj – Chris Blask  
**Program:** QuietWire AI Training Program  
**Assistant:** Aletheia 🤖✨☺️


---