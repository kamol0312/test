# JavaScript String (Matn) haqida

JavaScript’da string (matn) yaratish uchun **ikki xil qo‘shtirnoq** ishlatiladi:

- Double quotes `" "`
- Single quotes `' '`

## Misol

```javascript
"Bu matn";
'Bu boshqa bir matn!';
```

Double quotes yoki single quotes ishlatish o‘rtasida **hech qanday farq yo‘q**. Ular bir xil ishlaydi.

Bu turdagi stringlar **interpolation (o‘zgaruvchini string ichida ishlatish)** ni qo‘llab-quvvatlamaydi.  
String interpolation haqida **keyingi darslarda** o‘rganamiz.

---

# String property

`.length` property string uzunligini qaytaradi.

## Misol

```javascript
"Ajoyib!".length;
// 7
```

Agar sizda `text` nomli o‘zgaruvchi bo‘lsa, uning uzunligini quyidagicha olishingiz mumkin:

```javascript
let text = "Hello World";
text.length; // 11
```

---

# Basic String Methods

Quyida stringlar bilan ishlatiladigan ba’zi **asosiy metodlar** keltirilgan.

## .toLowerCase()

Bu metod stringdagi barcha harflarni **kichik harfga** o‘zgartirib yangi string qaytaradi.

```javascript
"ULUgbek".toLowerCase(); // "ulugbek"
```

E’tibor bering:

- `.length` — **property**, shuning uchun **()` kerak emas**
- `.toLowerCase()` — **method**, shuning uchun **()` ishlatiladi**

---

## .toUpperCase()

Bu metod stringdagi barcha harflarni **katta harfga** o‘zgartirib yangi string qaytaradi.

```javascript
"Ulugbek".toUpperCase(); // "ULUGBEK"
```

---

# O‘zgaruvchini yoki ifodani ko‘rish (Visualize)

Masalalarni yechayotganda siz `console.log()` dan foydalanib **o‘zgaruvchi yoki natijani ko‘rishingiz mumkin**.

Natija **browser console** oynasida chiqadi.

## Misol

```javascript
function sum(a, b) {
    console.log(a);
    console.log(a + b);
    return a + b;
}

// Sample usage
sum(1, 3);
```

Yuqoridagi kod ishlaganda console’da quyidagilar chiqadi:

```
1
4
```

Sababi:

- `console.log(a)` → 1 ni chiqaradi
- `console.log(a + b)` → 4 ni chiqaradi

---

# Muhim eslatma

`console.log()` **return o‘rnini bosmaydi**.

Siz `console.log()` ishlatganingizdan keyin ham **return yozishingiz kerak**.

```javascript
return a + b;
```

## Sample Usage

```javascript
getTextLength("Hello world");
makeTextUpper("Laptop");
makeTextLower("Test");
```
