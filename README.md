# immutable-vs-mutable-python

Article about immutable vs mutable data types in Python (in Uzbek)  
<i>Ushbu maqolaning bir qismi bu yerda e’lon qilingan</i> →  
<a href="https://www.linkedin.com/feed/update/urn:li:activity:7409309820966834178/">LinkedIn post</a>

Ba’zi tushunchalar ingliz tilida termin sifatida qoldirildi.  
Sababi, ushbu terminlar aynan ingliz tilida ishlatilganda ma’nosini to‘liq va aniq saqlab qoladi.

---

## 1) Immutable data types (O‘zgarmas ma’lumot turlari)

🟢 Python’da **immutable data types** deb, **object sifatida mavjud bo‘lgan** va **qiymati (value) o‘zgarganda mavjud object’ni o‘zgartirmasdan, balki xotirada yangi object yaratadigan** ma’lumot turlariga aytiladi.

Ya’ni, immutable obyekt ustida o‘zgarish amalga oshirilgandek ko‘rinsa ham, aslida:
- eski obyekt o‘zgarishsiz qoladi
- yangi qiymat uchun **yangi obyekt** yaratiladi

Buni oddiy kod va chizma orqali tushunish mumkin.

---

<img width="905" height="546" alt="Immutable diagram 1" src="https://github.com/user-attachments/assets/fd4c60a4-b62a-4fb0-a8a6-635b32a0f761" />
<h5 style="color:green"><b>(1-rasm)</b></h5>

<img width="900" height="500" alt="Immutable diagram 2" src="https://github.com/user-attachments/assets/7fbecab1-76b1-413e-be0e-b4dd15eda107" />
<h5 style="color:green"><b>(2-rasm)</b></h5>

Yuqoridagi **1-rasm**da ko‘rib turganingizdek, birinchi holatda o‘zgaruvchi `x` ma’lum bir qiymatni o‘zlashtiradi.  
Keyingi holatda esa `x` ga yangi qiymat berilganda, mavjud obyektning qiymati yangilanmaydi, balki **xotirada yangi obyekt yaratiladi**.

Buni qanday aniqlash mumkin?

Python’da barcha ma’lumot turlari **class** asosida yaratiladi va har bir obyekt xotirada o‘zining **unique manzili (id)** ga ega bo‘ladi.  
Qiymat o‘zgarganda `id()` funksiyasi orqali obyektning xotira manzili o‘zgarganini ko‘rish mumkin — bu esa yangi obyekt yaratilganidan dalolat beradi.(**2-rasm**)

Immutable ma'lumot turlariga <h4><b>[int,float,bool,str,tuple,frozeset,bytes]</b></h3> kabilar kiradi.
