# 🔗 GenQR – QR Code Generator  

🚀 **GenQR** is a sleek and simple QR code generator that helps you create custom QR codes instantly for links, text, emails, and more.  
Fast ⚡ | Lightweight 🎯 | Easy-to-use ✨  

---

## ✨ Features
- 🎨 Generate QR codes for **URLs**
- 📱 Mobile & desktop friendly
- ⚡ Lightning-fast generation
- 🖼️ Download & share with one click
- 🔒 Secure with (no data tracking)

---

## 🛠️ Tech Stack
- 🖥️ **Frontend:** HTML, CSS, JavaScript  
- 🎨 Simple UI with responsive design  

---

## 🚀 Getting Started
Clone the repo and run it locally:
```bash
git clone https://github.com/anirbanbanerjee07/genqr.git
cd genqr
open index.html
``` 

# 📜 1. Redirect Handling Script
Put this inside your `index.html` before the closing `</body>` tag:  

```html
<script type="text/javascript">
  (function (l) {
    if (l.search[1] === "/") {
      var decoded = l.search
        .slice(1)
        .split("&")
        .map(function (s) {
          return s.replace(/~and~/g, "&");
        })
        .join("?");
      window.history.replaceState(
        null,
        null,
        l.pathname.slice(0, -1) + decoded + l.hash
      );
    }
  })(window.location);
</script>
```

# 📜 2. Vercel Config
Create a file named `vercel.json` in your project root:

```json
{
  "rewrites": [{ "source": "/(.*)", "destination": "/" }]
}
```

# 💡 Future Improvements
- 🌈 Add themes & color customization
- 📷 Upload logo inside QR codes
- ☁️ Save QR codes to cloud


# 📸 Preview on window
**Generate QR code**![ss1](https://github.com/user-attachments/assets/6d8c71d4-3726-4237-b271-82db94ddb988)
**Save QR code**![ss2](https://github.com/user-attachments/assets/d49d0cf9-331a-45e9-85a8-e4806f1fa5ec)

# 📸 Preview on mobile
**Select Pixel**![mss1](https://github.com/user-attachments/assets/aec0d9a9-8e1c-4c1c-8107-d2f3237d956c)

**Generate QR code**![mss2](https://github.com/user-attachments/assets/6a5425f0-1996-4631-b0a0-a09b8ab39b60)

**Save QR code**![mss3](https://github.com/user-attachments/assets/8509b638-cb5f-4b09-81ea-2fdce9e50e6c)


## ⚙️ Deployment on Vercel  
Deploy **GenQR** seamlessly on [GenQR Web](https://gen-qr-web.vercel.app/) 🚀.


# 🤝 Contributing
Pull requests are welcome! 🙌
For major changes, please open an issue first.


# 📜 License
MIT License © 2025



💡 “Fast Codes, Faster Connections.” ⚡

Would you like me to make this README **minimal & modern** (short with emojis only) or **detailed & professional** (with badges, sections, and installation steps)?
