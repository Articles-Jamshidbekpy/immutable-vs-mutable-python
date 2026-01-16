# immutable-vs-mutable-python
Article about immutable vs mutable data types in Python (in Uzbek) <br>
<i>Ushbu maqolaning qismi bu yerda</i> -> <a>(https://www.linkedin.com/feed/update/urn:li:activity:7409309820966834178/)</a> <br><br>
Ba'zi malumotlarni ingiliz tilida termin qildik.Sababi bu ma'lumotlar shunda tushunarli bo'lib o'z ma'nosini saqlab qoladi.
### 1) Immutable data types (O'zgarmas ma'lumot turlari)
  Pythonda immutable data type lar deb object sifatida tushuniladigan hamda value si(qiymati) o'zgarganda, eski objectning qiymatini yangilamaydigan,balki yangi object yaratadigan ma'lumot turlari(data types)ga aytiladi.
  Buni oddiy kod va chizma orqali tushuntirish mumkin:
  
<img width="905" height="546" alt="Screenshot 2026-01-16 at 07 22 59" src="https://github.com/user-attachments/assets/fd4c60a4-b62a-4fb0-a8a6-635b32a0f761" />
(1-rasm)



<img width="900" height="500" alt="Screenshot 2026-01-16 at 07 00 28" src="https://github.com/user-attachments/assets/a1f9743c-8a96-44d3-996a-e25c7a29d6ef" />
(2-rasm)

Yuqorida 1-rasmda ko'rib turganingizdek, 1-holatda o'zgaruvchi x qiymatini o'zlashtirdi va keyingi safar y qiymatini o'zlashtirganda, xotirada yangi object yaratilishiga olib keldi.Buni qanday bilish mumkin?
Umuman olganda, bizning ma'lumot turlarimiz pythonda class sifatida, 
