# String ichidagi belgiga murojaat qilish (Character Access)

**Oxirgi yangilanish:** October 2025

JavaScript’da string ichidagi ma'lum bir belgiga **kvadrat qavslar `[]`** yordamida murojaat qilish mumkin.

Buning uchun siz **index (pozitsiya)** ni ko‘rsatishingiz kerak. Index **0 dan boshlanadi**.

---

## Misol

Faraz qilaylik `language` nomli o‘zgaruvchi quyidagi qiymatga ega:

```javascript
const language = "JavaScript";
```

Endi uning belgilariga quyidagicha murojaat qilish mumkin:

```javascript
language[0]; // "J" (birinchi belgi)
language[1]; // "a" (ikkinchi belgi)
language[2]; // "v" (uchinchi belgi)
```

---

## Console’da ko‘rish

Agar siz natijani **console’da ko‘rmoqchi bo‘lsangiz**, `console.log()` dan foydalanishingiz mumkin.

```javascript
console.log(language[1]); // "a"
```

---

# `.length` bilan birga ishlatish

Belgiga murojaat qilishni `.length` property bilan ham birlashtirish mumkin.

Masalan, **oxiridan ikkinchi belgini** olish:

```javascript
const language = "JavaScript";

language[language.length - 2]; // "p"
```

Sababi `"JavaScript"` so‘zining oxiridan ikkinchi belgisi **p**.

E’tibor bering:

```javascript
language[language.length];
```

Bu **undefined** qaytaradi.

Chunki index **0 dan boshlanadi**.

Agar string **9 ta belgidan** iborat bo‘lsa:

```
0 1 2 3 4 5 6 7 8
```

**8 — oxirgi belgining pozitsiyasi.**

---

# `.at(index)` metodi

2022-yildan boshlab JavaScript’da `.at()` metodi qo‘shilgan.

Bu metod **berilgan indexdagi belgini qaytaradi** va **manfiy indexlarni ham qo‘llab-quvvatlaydi**.

## Misollar

```javascript
const language = "JavaScript";

language.at(0); // "J"
language.at(1); // "a"
language.at(-1); // "t"
language.at(-2); // "p"
```

---

# Manfiy indexlar

Manfiy index ishlatilganda hisoblash **string oxiridan boshlanadi**.

```
-1 → oxirgi belgi
-2 → oxiridan ikkinchi belgi
-3 → oxiridan uchinchi belgi
```

---

# Muhim eslatma

Kvadrat qavslar `[]` sintaksisini oddiy holatlarda ishlatishingiz mumkin.

Ammo:

```javascript
language[-1]
```

Bu **undefined** qaytaradi.

Shuning uchun **manfiy index ishlatmoqchi bo‘lsangiz `.at()` metodidan foydalanish tavsiya etiladi.**
