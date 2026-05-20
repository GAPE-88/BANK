# GAPE Academy Website

Олон улсын мэргэжлийн боловсролын төв GAPE Academy-н албан ёсны вэбсайт.

## 📁 Файлын бүтэц

```
gape-website/
├── index.html              # Нүүр хуудас
├── 1plus2.html             # 1+2 Бакалаврын хөтөлбөр
├── assets/
│   └── logo.png            # GAPE лого (transparent)
└── README.md               # Энэ файл
```

## 🚀 Хэрхэн deploy хийх вэ?

### Сонголт 1: Vercel (ХАМГИЙН ХЯЛБАР) ⭐ — 10 минут

1. **GitHub дээр account нээх** — github.com
2. **Шинэ repository үүсгэх**:
   - "New repository" → нэр: `gape-website`
   - Public сонгох
   - "Create repository"
3. **Файлуудаа upload хийх**:
   - "uploading an existing file" дарах
   - Энэ folder-н бүх файлыг drag & drop хийх
   - "Commit changes"
4. **Vercel-д бүртгүүлэх** — vercel.com
   - "Continue with GitHub" дарах
5. **Project үүсгэх**:
   - "Add New Project" → repo-гоо сонгох
   - "Deploy" дарах
   - **30 секундын дотор сайт ажиллана!** 🎉

Vercel өгсөн URL: `https://gape-website.vercel.app`

### Сонголт 2: Netlify Drag & Drop — 5 минут (CODE-гүйгээр)

1. **netlify.com** -д нэвтрэх
2. **Drag & drop** хэсэгт энэ бүхэл folder-ийг чирэх
3. **Шууд ажиллана!** Netlify URL өгнө.

### Сонголт 3: GitHub Pages — Үнэгүй

1. GitHub repo үүсгэж файлуудаа upload хийх
2. Settings → Pages → Source: main branch
3. URL: `https://[username].github.io/gape-website`

---

## 🔗 Domain холбох (gape.education)

### Vercel дээр:

1. **Project Settings → Domains**
2. **Add Domain**: `gape.education`
3. Vercel өгсөн **DNS records** хуулна (А record эсвэл CNAME)
4. **Namecheap/registrar дээр**:
   - Domain settings руу орох
   - DNS records-уудыг тэр Vercel-н утгаар нэмэх
5. **5-30 минут** хүлээнэ → ажиллана

### www subdomain бас холбох:
- `www.gape.education` → `gape.education` руу redirect хийе

---

## 📝 Шинэ хуудас нэмэх

Шинэ хуудас (жишээ нь `cma.html`) нэмэхдээ:

1. Файлаа `gape-website/` folder-д хадгал
2. GitHub-д commit/push хий
3. Vercel өөрөө auto-deploy хийнэ (1-2 минут)

Бусад хуудаснаас холбохдоо:
```html
<a href="cma.html">CMA хөтөлбөр</a>
```

---

## ✅ Хийгдсэн зүйлс

- [x] Нүүр хуудас (`index.html`)
- [x] 1+2 Бакалавр хуудас (`1plus2.html`)
- [x] Logo (transparent PNG)
- [x] SEO meta tags (Open Graph, Twitter Card)
- [x] Favicon
- [x] Cross-page linking
- [x] Mobile-responsive design
- [x] Cyrillic-friendly fonts (Cormorant Garamond + Inter)

## 🔲 Хийх жагсаалт

- [ ] ACCA хуудас (`acca.html`)
- [ ] USCPA хуудас (`uscpa.html`)
- [ ] CMA хуудас (`cma.html`)
- [ ] Англи хэл hub (`english.html`)
- [ ] IELTS/TOEFL/Business English дэлгэрэнгүй
- [ ] Тухай хуудас (`about.html`)
- [ ] Багш нар (`teachers.html`)
- [ ] Блог жагсаалт (`blog.html`) + бие даасан нийтлэлүүд
- [ ] Холбоо барих (`contact.html`)
- [ ] **Бүртгэлийн форм** — Formspree эсвэл Google Forms-аар ажиллах байдалд
- [ ] Social media linkүүдийг бодит хаягаар солих
- [ ] Бодит зураг (hero, blog cards) орлуулах
- [ ] **Google Analytics** суулгах
- [ ] **Google Search Console**-д бүртгүүлэх

## 🛠️ Технологийн стек

- **HTML5** + **CSS3** (vanilla, framework-гүй)
- **Google Fonts** — Cormorant Garamond, Inter, Caveat
- **Inline SVG** icons (Tabler-style)
- **Mobile-first responsive** design
- **No JavaScript** (одоохондоо — static сайт)

## 📞 Холбоо барих

- 📧 info@gape.education
- 📞 976-85457788
- 📍 River Castle, Блок C, 6 давхар, Улаанбаатар

---

© 2026 GAPE Academy · Бүх эрх хуулиар хамгаалагдсан
