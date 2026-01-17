# immutable-vs-mutable-python

Article about immutable vs mutable data types in Python (in Uzbek)

## PART 2 (2-qism)

<i>Ushbu maqolaning 1-qismi (Kirish) bu yerda e’lon qilingan</i> →  
<a href="https://www.linkedin.com/feed/update/urn:li:activity:7409309820966834178/">LinkedIn post</a>

Ba’zi tushunchalar ingliz tilida termin sifatida qoldirildi.  
Sababi, ushbu terminlar aynan ingliz tilida ishlatilganda ma’nosini to‘liq va aniq saqlab qoladi.

---

## 1) Immutable data types (O‘zgarmas ma’lumot turlari)

🟢 Python’da **immutable data types** deb, **obyekt sifatida mavjud bo‘lgan** va **qiymati (value) o‘zgarganda mavjud obyektni o‘zgartirmasdan, balki xotirada yangi obyekt yaratadigan** ma’lumot turlariga aytiladi.

Ya’ni, immutable obyekt ustida o‘zgarish amalga oshirilgandek ko‘rinsa ham, aslida:
- eski obyekt o‘zgarishsiz qoladi;
- yangi qiymat uchun **yangi obyekt** yaratiladi.

Buni oddiy kod va chizma orqali tushunish mumkin.

---

<img width="905" height="546" alt="Immutable diagram 1" src="https://github.com/user-attachments/assets/fd4c60a4-b62a-4fb0-a8a6-635b32a0f761" />
<p><b>(1-rasm)</b></p>

<img width="900" height="500" alt="Immutable diagram 2" src="https://github.com/user-attachments/assets/7fbecab1-76b1-413e-be0e-b4dd15eda107" />
<p><b>(2-rasm)</b></p>

Yuqoridagi **1-rasm**da ko‘rib turganingizdek, birinchi holatda `a` o‘zgaruvchisi ma’lum bir qiymatni (`x`) o‘zlashtiradi.  
Keyingi holatda esa `a` ga yangi qiymat (`y`) berilganda, mavjud obyektning qiymati yangilanmaydi, balki **xotirada yangi obyekt yaratiladi**.

### id nima?

Python’da barcha ma’lumot turlari **class** asosida yaratiladi va har bir obyekt xotirada o‘zining **yagona identifikatori (`id`)** ga ega bo‘ladi.

Qiymat o‘zgarganda `id()` funksiyasi orqali obyektning xotira manzili o‘zgarganini ko‘rish mumkin. Bu esa **yangi obyekt yaratilganidan dalolat beradi** (2-rasm).

> **id** — bu obyektga beriladigan yagona (unique) qiymat bo‘lib, u obyektning Python’dagi dinamik xotiradagi joylashuvini ko‘rsatadi.

Immutable ma’lumot turlariga quyidagilar kiradi:

[int, float, complex, NoneType, bool, str, tuple, frozenset, bytes]

---

## 2) Mutable data types (O‘zgaruvchan ma’lumot turlari)

🟢 **Mutable data types** — bu qiymati o‘zgartirilganda yangi obyekt yaratmaydigan, balki mavjud obyektning ichki holatini (state) o‘zgartiradigan ma’lumot turlaridir.

Bu turdagi obyektlarning qiymatini bevosita o‘zgartirish mumkin.

Mutable ma’lumot turlariga quyidagilar misol bo‘la oladi:

[list, set, dict, bytearray]


Quyida buni hammaga tushunarli bo‘lgan `list` ma’lumot turi orqali ko‘rib chiqamiz.

---

<img width="900" height="260" alt="Mutable diagram 1" src="https://github.com/user-attachments/assets/75d0c19f-761e-4e74-a797-c21ecd6bf778" />
<p><b>(3-rasm)</b></p>

<img width="677" height="617" alt="Mutable diagram 2" src="https://github.com/user-attachments/assets/dd3ee260-0b22-404f-8b49-59447db1f656" />
<p><b>(4-rasm)</b></p>

### 3–4-rasmlar tahlili:

- `a` o‘zgaruvchisi `[20, 30, 40]` list obyektiga reference bo‘ldi;
- `a.append(50)` orqali mavjud obyektning qiymati o‘zgartirildi va yangi qiymat `[20, 30, 40, 50]` ga teng bo‘ldi;
- obyektning eski va yangi `id` qiymatlari tengligicha qoldi;
- `id` obyektning yagona (unique) identifikatori bo‘lganligi sababli, bu holatda obyekt o‘zgarmaganini (ya’ni yangi obyekt yaratilmaganini), balki faqat uning qiymati o‘zgartirilganini xulosa qilishimiz mumkin.

Davomi bor…  
3-qismda aynan ushbu ma’lumot turlaridan qaysi holatlarda va qanday foydalanish kerakligini yoritishga harakat qilamiz.
