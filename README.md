# 🌞 דשבורד פוטנציאל סולארי — רשויות מקומיות בישראל

דשבורד אינטרקטיבי לצפייה בנתוני הפוטנציאל לייצור אנרגיה סולארית לפי רשות מקומית.

**מקור נתונים:** משרד האנרגיה והתשתיות + המרכז למיפוי ישראל (אפריל 2026)

---

## 🚀 העלאה ל-GitHub Pages (5 דקות)

### שלב 1 — צור Repository

1. היכנס ל-[github.com](https://github.com) וצור חשבון אם אין לך
2. לחץ **New repository**
3. תן שם: `solar-dashboard`
4. סמן **Public**
5. לחץ **Create repository**

### שלב 2 — העלה את הקבצים

**אפשרות א' — ממשק אתר (הכי קל):**

1. בדף ה-repository, לחץ **uploading an existing file**
2. גרור את שני הקבצים: `index.html` ו-`data.json`
3. לחץ **Commit changes**

**אפשרות ב' — מ-VS Code (עם Git מותקן):**

```bash
cd solar-dashboard
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/solar-dashboard.git
git push -u origin main
```

### שלב 3 — הפעל GitHub Pages

1. ב-repository, לחץ **Settings**
2. בתפריט השמאלי לחץ **Pages**
3. תחת **Source** בחר: `Deploy from a branch`
4. Branch: `main` / Folder: `/ (root)`
5. לחץ **Save**

### שלב 4 — גישה לאתר

תוך ~2 דקות האתר יהיה זמין בכתובת:
```
https://YOUR_USERNAME.github.io/solar-dashboard/
```

---

## 📁 מבנה הקבצים

```
solar-dashboard/
├── index.html    # הדשבורד
└── data.json     # נתוני כל 259 הרשויות
```

---

## 🔄 עדכון הנתונים בעתיד

כשיצאו נתונים חדשים:
1. החלף את `data.json` בגרסה החדשה
2. דחוף ל-GitHub — האתר יתעדכן אוטומטית

---

## 🖥️ מעבר לשרת עצמי (בעתיד)

אם תרצה לעבור ל-VPS/nginx:
```bash
scp -r solar-dashboard/ user@your-server:/var/www/html/
```
זה הכל — אותם קבצים בדיוק.
