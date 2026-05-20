# 🚀 GAPE Website ажиллуулах гарын авлага

Алхам алхмаар явбал **1 цагийн дотор** сайт интернетэд ажиллана.

---

## ⚡ ХАМГИЙН ХУРДАН ЗАМ (5 минут) — Netlify Drag & Drop

Эхэн үе сорихыг хүсэж байвал:

1. **netlify.com** руу орох
2. **"Sign up"** → Google эсвэл GitHub-аар бүртгүүл
3. Login хийсний дараа **"Sites"** хэсэг рүү орох
4. Доод талын **drag & drop хэсэг** рүү:
   - Энэ `gape-website` folder-ийг бүтнээр нь чирээд тавь
5. ⏱️ **30 секундын дараа** сайт ажиллана!

URL жишээ: `https://gape-website-abc123.netlify.app`

**Хязгаарлалт:** Файл шинэчлэхдээ дахин drag & drop хийх хэрэгтэй (GitHub-тай холбохгүй бол).

---

## 🌟 ЗӨВ ЗАМ (1 цаг) — GitHub + Vercel

### АЛХАМ 1: GitHub бүртгэл (15 минут)

1. **github.com** руу орох
2. **"Sign up"** → имэйл, password оруулна
3. Username сонгох (жишээ: `gape-academy`)
4. Имэйл баталгаажуулах

### АЛХАМ 2: Repository үүсгэх (5 минут)

1. GitHub-д орсны дараа баруун дээд буланд **"+"** товч → **"New repository"**
2. **Repository name**: `gape-website`
3. **Description**: "GAPE Academy official website"
4. **Public** сонгох (Private бол хязгаарлалттай)
5. **"Add a README file"** ✓ (хайрцаг)
6. **"Create repository"** дарах

### АЛХАМ 3: Файлуудаа upload хийх (10 минут)

1. Шинэ repo дотроо орох
2. **"Add file"** → **"Upload files"**
3. **Чирээд тавих** эсвэл **"choose your files"**:
   - `index.html`
   - `1plus2.html`
   - `README.md`
   - `DEPLOYMENT_GUIDE.md`
   - `assets/` folder бүхэлд нь (logo.png-тэй хамт)
4. **Commit message**: "Initial website upload"
5. **"Commit changes"** дарах

⚠️ **Анхаар:** `assets` folder upload хийхэд folder structure хадгалагдсан байх ёстой. Хэрэв буруу бол `logo.png` -г үндсэн folder-д орхино.

### АЛХАМ 4: Vercel-д deploy хийх (15 минут)

1. **vercel.com** руу орох
2. **"Sign Up"** → **"Continue with GitHub"** дарах
3. GitHub-аас Vercel-д хандах эрх өгөх
4. Dashboard-д **"Add New..."** → **"Project"**
5. GitHub repo-уудаас **`gape-website`**-г олж **"Import"** дарах
6. Тохиргооны хэсэгт:
   - **Framework Preset**: Other
   - **Build Command**: (хоосон)
   - **Output Directory**: (хоосон)
   - **Install Command**: (хоосон)
7. **"Deploy"** дарах
8. ⏱️ **30-60 секунд** хүлээнэ...
9. 🎉 **Сайт ажиллаж байна!**

URL жишээ: `https://gape-website-username.vercel.app`

### АЛХАМ 5: Domain холбох (15 минут)

`gape.education` domain-аа холбохын тулд:

1. Vercel-д таны project дотор: **"Settings"** → **"Domains"**
2. **"Add"** дарж `gape.education` оруулах
3. Дахин **"Add"** → `www.gape.education` ч мөн нэмэх
4. Vercel өгсөн **DNS records**-ийг тэмдэглэх:
   ```
   Type: A
   Name: @
   Value: 76.76.21.21
   ```
   эсвэл
   ```
   Type: CNAME
   Name: www
   Value: cname.vercel-dns.com
   ```

5. Domain худалдан авсан газартаа (Namecheap, GoDaddy гэх мэт) орох:
   - **DNS settings / DNS Management** руу орох
   - Дээрх records-ыг тэр чигээр оруулах
   - Хуучин зүйлсийг устгах хэрэгтэй болж магадгүй

6. **5-30 минут** хүлээнэ
7. ✅ `www.gape.education` дээр сайт ажиллана!

---

## 📝 Шинэ хуудас нэмэх

CMA эсвэл ACCA хуудас хийгдсэний дараа:

### GitHub-д (web дээрээс):
1. Repository руу орох
2. **"Add file"** → **"Upload files"**
3. Шинэ файлаа хуулах
4. **"Commit changes"**
5. ⏱️ Vercel **автоматаар** 1-2 минутын дотор шинэчилнэ

### Git command-аар (Terminal):
```bash
git clone https://github.com/[username]/gape-website.git
cd gape-website
# Шинэ файл хийсний дараа:
git add .
git commit -m "Add CMA page"
git push
```

---

## 🔗 Бүртгэлийн форм ажиллуулах

Одоогийн "Бүртгүүлэх" товчнууд `href="#"` юм. Үүнийг **жинхэнээр** ажиллуулахын тулд:

### Хамгийн хялбар: Google Forms

1. **forms.google.com** дээр форм үүсгэх
2. Талбарууд: Нэр, Утас, Имэйл, Сонирхож буй хөтөлбөр
3. Send → Link copy
4. HTML-д "Бүртгүүлэх" товч линкийг тэр Google Form-н URL-аар солих:

```html
<a href="https://forms.google.com/abc123" target="_blank" class="btn btn-primary">
  Бүртгүүлэх
</a>
```

### Илүү professional: Formspree

1. **formspree.io** дээр account нээх
2. **New form** → имэйл-аа оруулах
3. Form ID авах (жишээ: `xyzabc123`)
4. HTML-д жинхэнэ форм хийгээд:

```html
<form action="https://formspree.io/f/xyzabc123" method="POST">
  <input name="нэр" required>
  <input name="имэйл" type="email" required>
  <button type="submit">Илгээх</button>
</form>
```

5. Бөглөгдсөн форм info@gape.education рүү ирнэ

---

## 📊 Analytics суулгах (Сайтад хэн орж байгааг харах)

### Google Analytics:

1. **analytics.google.com** дээр property үүсгэх
2. Сайтын URL оруулах
3. **Measurement ID** авах (G-XXXXXXXXX)
4. HTML-н `</head>` дээр доорхийг нэмэх:

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXX');
</script>
```

---

## 🆘 Хэрэв тулгарвал...

### Лого харагдахгүй байна
- `assets/logo.png` зам зөв эсэхийг шалга
- HTML-д `src="assets/logo.png"` бичсэн эсэх

### Сайт хуучнаараа байна (шинэчлэгдээгүй)
- Browser cache цэвэрлэх: **Ctrl+Shift+R** (Mac: Cmd+Shift+R)
- Vercel-д deploy log харах

### Domain ажиллахгүй байна
- 24 цаг хүлээнэ (DNS propagation)
- `https://dnschecker.org` ашиглан DNS-ыг шалгана

### Форм ажиллахгүй байна
- Formspree dashboard-д submissions харагдаж байна уу?
- Spam folder шалга

---

## 📞 Хэрэгтэй холбоосууд

- 🌐 GitHub: https://github.com
- ⚡ Vercel: https://vercel.com
- 🎨 Netlify: https://netlify.com
- 📋 Formspree: https://formspree.io
- 📊 Google Analytics: https://analytics.google.com

---

**Амжилт хүсье! 🚀**
