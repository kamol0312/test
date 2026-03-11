# Asosiy funksiyalar

**Oxirgi yangilanish:** May 2022

Keling, JavaScript'dagi asosiy funksiyalar bilan boshlaymiz.

```javascript
function sum(x, y) {
    return x + y;
}
```

Ushbu kod `sum` deb nomlangan funksiyani yaratadi.

Bu shuni anglatadiki, siz endi `sum(1, 3)` deb chaqirishingiz mumkin va u **4** natijani qaytaradi.

Siz funksiyani boshqa qiymatlar bilan ham ishlatishingiz mumkin. Masalan:

```javascript
sum(2, 5)
```

Bu holda funksiya **2 + 5** hisoblab, **7** natijani qaytaradi.

---

## Natijani qaytarish (Returning the result)

JavaScript’da funksiyalar ichidan **return** orqali natija qaytariladi.

Agar siz `return` yozishni unutib qo‘ysangiz, funksiya **undefined** qiymatini qaytaradi.

`return` kalit so‘zi funksiyani **to‘xtatadi (exit qiladi)**.

```javascript
function sum(x, y) {
    return x + y;
    console.log("Hello World"); // bu kod HECH QACHON ishlamaydi
}
```

`return` ishlagan zahoti funksiya tugaydi va natija qaytariladi (`x + y`).  
Shuning uchun undan keyingi kod **ishlamaydi**.
