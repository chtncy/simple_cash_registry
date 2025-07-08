# Cash Register Simulator

A lightweight JavaScript cash register object that lets you:

- Define items for sale  
- Add items to a shopping cart  
- Calculate totals (with automatic 10% discount for orders over $500)  
- Process payments and display change or error messages  

All logic runs in plain ES6 JavaScript—no frameworks or build steps required.

---

## 🌐 Technologies Used

- **JavaScript (ES6+)** – Core language features, array methods, `this` context  
- **Console I/O** – Uses `console.log()` for interactive feedback  

---

## ✨ Features

1. **Item Catalog**  
   - Predefined `itemsForSale` array with `{ name, price }` objects  
2. **Add to Cart**  
   - `addItem(name)` looks up an item by name and pushes it into `shoppingCart`  
   - Graceful “not found” message if the item doesn’t exist  
3. **Total Calculation**  
   - `calculateTotalPrice()` sums up all prices in the cart  
4. **Payment Processing**  
   - `pay(amount)` applies a 10% discount automatically for totals over $500  
   - Logs change owed or an error if funds are insufficient  
   - Clears or retains cart as needed (you control `shoppingCart` directly)
