# SportGear – E-Commerce Frontend Web Application

**SportGear** is an online sports and fitness equipment store frontend web application built strictly to the specifications of the **SportGear Product Requirements Document (PRD)**.

---

## 🚀 Live Demo & How to Run Locally

1. Open a terminal in the project directory:
   ```bash
   cd c:\Users\ACER\OneDrive\Desktop\sport
   ```
2. Start any local web server, for instance using Python:
   ```bash
   python -m http.server 8080
   ```
3. Open your browser and navigate to:
   ```
   http://localhost:8080/index.html
   ```
   *(Or simply double click `index.html` to open directly in Chrome, Firefox, Safari, or Edge).*

---

## 🎨 Design Guidelines & Aesthetics (PRD Section 5)

- **Color Scheme**:
  - **Primary**: Forest Green (`#1A7A4A`) for headers, navigation, badges, and primary accents.
  - **Accent / CTA**: Vibrant Sports Orange (`#F97316`) for call-to-actions ("Add to Cart", "Shop Now", "Place Order", discount ribbons).
  - **Surfaces & Cards**: Crisp White (`#FFFFFF`) with soft slates (`#F8FAFC`).
  - **High Contrast**: WCAG AA accessible contrast for all text elements.
- **Typography**:
  - **Headings & Display**: Google Font `'Oswald'`, heavy athletic uppercase typography.
  - **Body & Navigation**: Google Font `'Poppins'`, modern legible 16px body copy.
- **Icons**: FontAwesome 6 scalable vector sports and interface icons.
- **Responsiveness**: Mobile-first architecture supporting Mobile (<576px), Tablet (576–991px), and Desktop (992px+).

---

## 📄 Complete 9-Page Architecture (PRD Section 6)

| # | Page File | PRD Section | Description |
|---|-----------|-------------|-------------|
| 1 | [index.html](file:///c:/Users/ACER/OneDrive/Desktop/sport/index.html) | 6.1 Home Page | Hero action banner, category cards (Footwear, Apparel, Gym Equipment, Team Sports, Accessories), featured gear grid, deals section, trust badges, athlete testimonials, and newsletter. |
| 2 | [products.html](file:///c:/Users/ACER/OneDrive/Desktop/sport/products.html) | 6.2 Product Listing | Dynamic catalog grid with multi-filter sidebar (category, sport, brand, price slider, sizes), instant search, sorting (popularity, rating, price, newest), and active filter chips. |
| 3 | [product-detail.html](file:///c:/Users/ACER/OneDrive/Desktop/sport/product-detail.html) | 6.3 Product Detail | Multi-image interactive gallery, stock status, size selector, quantity picker, Add to Cart, Buy Now, Add to Wishlist, customer reviews with submission form, and related gear. |
| 4 | [cart.html](file:///c:/Users/ACER/OneDrive/Desktop/sport/cart.html) | 6.4 Shopping Cart | Itemized product table, quantity increase/decrease/remove, live subtotals, free shipping threshold tracker, coupon code discount engine (`SPORT10`, `FIT20`), and empty cart state. |
| 5 | [checkout.html](file:///c:/Users/ACER/OneDrive/Desktop/sport/checkout.html) | 6.5 Checkout Page | Complete shipping destination form with validation, saved address auto-fill, simulated payment methods (Card, UPI, Net Banking, COD), and order confirmation with generated Order ID. |
| 6 | [account.html](file:///c:/Users/ACER/OneDrive/Desktop/sport/account.html) | 6.6 User Account | Auth-guarded athlete dashboard with profile editing, saved address manager, personal wishlist ("Move to Cart" action), and order tracking status timeline (Placed, Packed, Shipped, Out for delivery, Delivered). |
| 7 | [login.html](file:///c:/Users/ACER/OneDrive/Desktop/sport/login.html) | 6.7 Login / Register | Tabbed authentication interface with client-side validation, password matching, "remember me", forgot password modal, and one-click demo login credentials. |
| 8 | [about.html](file:///c:/Users/ACER/OneDrive/Desktop/sport/about.html) | 6.8 About Us | Company founding story, mission and vision, core athletic values, stats counters (50k+ athletes, 15+ years), and leadership team cards. |
| 9 | [contact.html](file:///c:/Users/ACER/OneDrive/Desktop/sport/contact.html) | 6.9 Contact Us | HQ address and showroom hours, contact phone & email, interactive topic-based contact form with validation and ticket generation, location showcase, and FAQs. |

---

## 🧩 Features & Data Model (PRD Section 7, 8 & 9)

### Core Features (F1 – F8)
- **F1 (Category-wise product display)**: Organized across Footwear, Apparel, Gym Equipment, Team Sports, and Accessories.
- **F2 (Product search)**: Live search across name, brand, sport, category, and specifications.
- **F3 (Add to cart)**: Size and quantity selection with instant persistence in browser `localStorage`.
- **F4 (Quantity adjustment)**: Increment, decrement, or remove items directly from the cart.
- **F5 (Price calculation)**: Automatic calculation of subtotal, coupon discounts, conditional shipping fees, and taxes.
- **F6 (Order summary)**: Itemized breakdowns available in both cart and checkout steps.
- **F7 (Checkout process)**: Multi-step checkout with address validation and simulated payment processing.
- **F8 (Simulated Login/Register)**: Client-side session management persisted in `localStorage`.

### Bonus Features (B1 – B7)
- **B1 (Product filters)**: Category, sport (Football, Basketball, Cricket, Tennis, Running, Fitness), brand, price range, and size filters.
- **B2 (Wishlist)**: Quick heart toggle from any card or detail page; view, remove, or "Move to Cart" in user account.
- **B3 (Size selection)**: Interactive size pills with validation enforcing size selection before adding footwear/apparel.
- **B4 (Reviews and ratings)**: Star breakdowns, verified purchaser reviews, and working review submission form.
- **B5 (Related products)**: Contextual suggestions from the matching category and sport.
- **B6 (Order tracking)**: Multi-stage status timeline (Placed ➔ Packed ➔ Shipped ➔ Out for delivery ➔ Delivered).
- **B7 (Payment gateway simulation)**: Mock payment methods with simulated processing state and instant order dispatch.

---

## 🔑 Pre-Configured Demo Account

For rapid portfolio testing, a demo athlete account is pre-loaded:
- **Email**: `alex@sportgear.com`
- **Password**: `password123`
- Includes pre-populated saved addresses, wishlist items, and sample past orders with active tracking timelines.
