# 📋 Project Overview — SaaS Pricing Table (Flexbox)

## 🎯 Goal
Build a practical, real-world-looking **pricing table** using CSS Flexbox and a responsive media query. This project mirrors layouts seen on actual product websites like Notion, Vercel, or Stripe.

## 📄 HTML Structure
```html
<div class="pricing-container">     ← Flexbox parent
  <div class="pricing-plan">        ← Card 1: Basic
    <div class="plan-title">Basic</div>
    <div class="plan-price">$11.99/month</div>
    <ul class="plan-features">
      <li>✅ 10GB Storage</li>
      <li>✅ 1 User</li>
      <li>🚫 Support</li>
    </ul>
    <button class="plan-button">Sign Up</button>
  </div>
  <!-- ...Standard and Premium cards same structure -->
</div>
```

## 🧠 Flexbox Breakdown

### Container (`.pricing-container`)
```css
.pricing-container {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 40px;
  height: 100vh;  /* full viewport height */
}
```

### Cards (`.pricing-plan`)
```css
.pricing-plan {
  flex: 1;              /* equal width distribution */
  max-width: 400px;     /* cap the max width */
  padding: 20px;
  background-color: #f2f2f2;
  border-radius: 5%;
  text-align: center;
}
```

### Responsive Stacking — `@media` Query
```css
@media (max-width: 1250px) {
  .pricing-container {
    flex-direction: column;  /* stacks vertically on small screens */
    height: 100%;            /* let it scroll naturally */
  }
}
```

## 🧩 Design Details
| Element | Style |
|---|---|
| Plan price | `font-size: 48px`, bold |
| Feature list | `list-style: none` (removes default bullets) |
| Sign Up button | Orange (`#ff6600`) background, white text |
| Font | Sono (Google Fonts, monospace-like) |

## 📊 Difficulty Level
| Aspect | Rating |
|---|---|
| HTML | ⭐⭐ (repeated card structure) |
| Flexbox | ⭐⭐ (straightforward sizing + gap) |
| Responsive | ⭐⭐ (one media query) |
| Overall | ⭐⭐ Beginner-Friendly |

## 💡 Next Steps
- Highlight the "Standard" plan (most popular) with a border or different color
- Add a toggle for Monthly vs Annual billing
- Animate card hover with `transform: translateY(-5px)` shadow
- Add real sign-up button links
- Make the feature list icons consistent with a library like Font Awesome
