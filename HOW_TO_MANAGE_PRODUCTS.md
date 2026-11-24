# 🛍️ Rang Banjara - Product Management Guide

Yeh guide batata hai ki aap apne real jewellery products kaise add ya edit kar sakte hain.

---

## 1. Product Structure (`index.html`)

`index.html` file ke andar line ~634 par `const products = [...]` array hai.
Har product ka format aisa hota hai:

```javascript
{
    id: 1,                                       // Unique number
    name: "Royal Banjara Oxidized Silver Choker",// Jewellery ka naam
    category: "Necklaces",                       // Category: "Necklaces", "Rings", "Earrings", "Payal"
    price: 3499,                                 // Selling price (₹)
    originalPrice: 4999,                         // MRP / Original price (₹)
    badge: "Best Seller",                        // Badge: "Best Seller", "New Drop", "Trending", "Handcrafted"
    image: "images/choker-1.jpg",                // Image path ya URL
    description: "Hand-forged oxidized silver finish with Kutch tribal motifs."
}
```

---

## 2. Naya Product Kaise Add Karein?
Bas array me ek naya object comma (`,`) ke sath paste kar dijiye:

```javascript
{
    id: 9,
    name: "Aapke Naye Jhumke Ka Naam",
    category: "Earrings",
    price: 1499,
    originalPrice: 1999,
    badge: "New Arrival",
    image: "images/jhumka-1.jpg",
    description: "Authentic oxidized silver jhumkas with ghungroo bells."
}
```

---

## 3. Categories List
Website me filhal yeh 4 main categories supported hain:
- `Necklaces`
- `Rings`
- `Earrings`
- `Payal` (Payal, Kadas & Cuffs)

Aap jab bhi naya product daalein, `category` me inhi 4 me se ek naam likhein taaki filter button sahi kaam kare.
