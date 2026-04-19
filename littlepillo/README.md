# Little Pillo Academy — Website

## 📁 Folder Structure

```
littlepillo/
├── vercel.json          ← Vercel config (don't touch)
└── public/
    ├── index.html       ← The website (don't touch)
    ├── logo.png         ← Your logo
    └── products.json    ← ✏️ THIS IS THE ONLY FILE YOU EDIT
```

---

## ✏️ How to Add a New Product

Open `products.json` and add a new entry at the **top** of the list
(so newest products appear first on the website).

Copy and paste this template and fill in your details:

```json
{
  "id": 7,
  "title": "Your Product Title Here",
  "description": "A short description of what's inside the workbook.",
  "price": "$2.99",
  "language": "english",
  "emoji": "🌟",
  "buyLabel": "Get it →",
  "link": "https://payhip.com/b/YOURCODE"
}
```

### Field Guide

| Field       | What to put                                              |
|-------------|----------------------------------------------------------|
| `id`        | Next number in sequence (7, 8, 9...)                    |
| `title`     | Full product name                                        |
| `description` | 1–2 sentences describing the workbook                  |
| `price`     | e.g. `"$2.99"` or `"$4.99"`                            |
| `language`  | Must be exactly: `"english"`, `"spanish"`, or `"bilingual"` |
| `emoji`     | One emoji that represents the workbook                   |
| `buyLabel`  | `"Get it →"` for English, `"Obtener →"` for Spanish    |
| `link`      | The full Payhip URL for that product                    |

### Don't forget:
- Add a **comma** after the `}` of the previous product
- The last product in the list has **no comma** after its `}`
- The `id` should be unique for each product

---

## 🚀 How to Deploy to Vercel

### First time setup (one time only):
1. Go to [github.com](https://github.com) and create a free account
2. Create a new repository called `littlepillo-academy`
3. Upload all files in this folder to that repository
4. Go to [vercel.com](https://vercel.com) and sign in with GitHub
5. Click **Add New Project** → select your `littlepillo-academy` repo
6. Click **Deploy** — your site will be live in ~30 seconds!
7. Vercel gives you a free URL like `littlepillo-academy.vercel.app`

### Every time you add a new product:
1. Edit `products.json` on GitHub (click the file → click the pencil icon)
2. Add your new product entry
3. Click **Commit changes**
4. Vercel automatically re-deploys in ~30 seconds — done! 🎉

---

## 🌐 Custom Domain (optional)

To use `littlepilloacademy.com` instead of the Vercel URL:
1. Buy the domain on [Namecheap](https://namecheap.com) (~$12/year)
2. In Vercel → your project → Settings → Domains
3. Add your domain and follow the DNS instructions

---

## 📧 Email Capture

The "Free Resource" form currently shows a success message but doesn't
actually send emails. To make it functional, sign up for a free
[Mailchimp](https://mailchimp.com) account and replace the `handleFree`
function in `index.html` with your Mailchimp form embed code.

---

## 🆘 Need Help?

Ask Claude! Just say:
> "I need to add a new product to Little Pillo Academy — here are the details: [paste your Payhip link and product info]"

Claude will give you the exact JSON block to copy and paste.
