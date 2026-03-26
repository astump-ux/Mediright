# MediRight – Landing Page

Responsive Landingpage für MediRight: KI-gestützter GoÄ-Widerspruchs-Service für Beihilfeberechtigte & Privatversicherte.

## 🗂 Repo-Struktur

```
mediright/
├── index.html      ← Komplette Landingpage (HTML + CSS in einer Datei)
├── vercel.json     ← Vercel Deployment-Konfiguration
└── README.md       ← Diese Datei
```

---

## 🚀 Deployment: GitHub → Vercel (Schritt-für-Schritt)

### Schritt 1 – GitHub Repository anlegen

1. GitHub öffnen → **[+ New repository](https://github.com/new)**
2. Repository-Name: `mediright` (oder beliebig)
3. Sichtbarkeit: **Public** oder **Private** (beides funktioniert mit Vercel)
4. **„Add a README file"** NICHT anhaken (wir pushen eigene Dateien)
5. Klick auf **„Create repository"**

---

### Schritt 2 – Dateien pushen

**Option A – Über die GitHub-Weboberfläche (kein Terminal nötig):**

1. Im neuen Repo auf **„uploading an existing file"** klicken
2. `index.html` und `vercel.json` per Drag & Drop hochladen
3. Commit-Message: `Initial commit: MediRight landing page`
4. Klick auf **„Commit changes"**

**Option B – Per Terminal / Git:**

```bash
# Lokalen Ordner initialisieren
git init
git add index.html vercel.json README.md
git commit -m "Initial commit: MediRight landing page"

# Mit GitHub verbinden (URL aus deinem neuen Repo kopieren)
git remote add origin https://github.com/DEIN-USERNAME/mediright.git
git branch -M main
git push -u origin main
```

---

### Schritt 3 – Vercel mit GitHub verbinden

1. **[vercel.com](https://vercel.com)** öffnen → mit GitHub-Account einloggen
2. Dashboard → **„Add New Project"** klicken
3. Unter **„Import Git Repository"** → dein `mediright`-Repo auswählen
4. Klick auf **„Import"**

---

### Schritt 4 – Projekt konfigurieren

In der Vercel-Konfigurationsmaske:

| Einstellung | Wert |
|---|---|
| **Framework Preset** | `Other` |
| **Root Directory** | `./` (Standard, nichts ändern) |
| **Build Command** | *(leer lassen)* |
| **Output Directory** | *(leer lassen)* |
| **Install Command** | *(leer lassen)* |

→ Klick auf **„Deploy"**

---

### Schritt 5 – Live ✅

Nach ~15–30 Sekunden ist die Seite live unter:
```
https://mediright-XXXXX.vercel.app
```

Vercel zeigt dir die URL direkt im Dashboard an.

---

## 🔄 Updates deployen

Jede Änderung, die du in GitHub pushst (oder per Weboberfläche hochlädst), löst **automatisch ein Re-Deployment** aus. Kein manueller Schritt nötig.

---

## 🌐 Custom Domain (optional)

1. Vercel Dashboard → Dein Projekt → **„Settings"** → **„Domains"**
2. Gewünschte Domain eingeben (z. B. `mediright.de`)
3. DNS-Einträge beim Domain-Anbieter setzen (Vercel zeigt die genauen Werte)

---

## 📋 Technischer Stack

- **HTML5 + CSS3** (keine externen Frameworks)
- **Google Fonts:** DM Serif Display, DM Sans
- **Icons:** FontAwesome 6 (via CDN)
- **Hosting:** Vercel (Static)
- **DSGVO:** Keine Cookies, kein Tracking, keine externen APIs
