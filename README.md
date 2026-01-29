# ValorPack Landing Page

**Professional landing page for QR code access to ValorPack - AviWrap™ investor documentation**

[🇫🇷 Version française ci-dessous](#version-française)

---

## 🎯 Purpose

This landing page serves as a mobile-optimized gateway for investors and stakeholders scanning QR codes on:
- Business cards
- Exhibition stands (PNR EXPO 2026)
- Printed materials
- Marketing collateral

It provides instant access to:
- Complete Business Plan (PDF)
- Investor Presentation (PowerPoint)
- Technical specifications
- Direct contact information

---

## ✨ Features

- **📱 Mobile-First Design**: Optimized for smartphone scanning
- **🎨 Brand-Consistent**: ValorPack green color palette
- **⚡ Fast Loading**: Single HTML file, no dependencies
- **📊 Key Metrics Display**: Market size, ROI, investment amount
- **🔗 Direct Downloads**: One-click access to Google Drive files
- **📧 Contact Integration**: Clickable email links
- **🏆 Credibility Badges**: Patent, PNR EXPO 2026, PNR-2021

---

## 🚀 Quick Start

### Option 1: Netlify Drop (Fastest - 2 minutes)

1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag and drop the `valorpack_landing_page.html` file
3. Get your instant URL: `https://your-site-name.netlify.app`
4. Optional: Customize the site name in Netlify dashboard

**No account required!** ⚡

---

### Option 2: GitHub Pages (Most Professional)

1. Create a GitHub account at [github.com](https://github.com)
2. Create a new repository named `valorpack`
3. Upload the HTML file renamed as `index.html`
4. Go to Settings → Pages
5. Select `main` branch and save
6. Your site will be live at: `https://your-username.github.io/valorpack`

**Free forever** | **Custom domain supported** ✅

---

### Option 3: Google Sites (Google Ecosystem)

1. Go to [sites.google.com](https://sites.google.com)
2. Create a new site
3. Use "Embed" component to add the HTML
4. Publish with custom URL
5. Your site: `https://sites.google.com/view/valorpack`

**Integrated with Google Drive** 🔗

---

## ⚙️ Configuration

### Step 1: Get Google Drive Share Links

For each file in your Google Drive:

1. **Right-click** on the file
2. Select **"Get link"** / **"Obtenir le lien"**
3. Change permission to **"Anyone with the link"** / **"Tous ceux qui disposent du lien"**
4. **Copy the link** (format: `https://drive.google.com/file/d/XXXXXXXX/view?usp=sharing`)

### Step 2: Edit the HTML File

Open `valorpack_landing_page.html` in a text editor and replace:

**Line ~260 - Business Plan:**
```html
<a href="VOTRE_LIEN_GOOGLE_DRIVE_BUSINESS_PLAN" class="doc-card" target="_blank">
```
Replace `VOTRE_LIEN_GOOGLE_DRIVE_BUSINESS_PLAN` with your actual Google Drive link.

**Line ~273 - PowerPoint Presentation:**
```html
<a href="VOTRE_LIEN_GOOGLE_DRIVE_PRESENTATION" class="doc-card" target="_blank">
```
Replace `VOTRE_LIEN_GOOGLE_DRIVE_PRESENTATION` with your actual Google Drive link.

**Line ~286 - Technical Sheet (Optional):**
```html
<a href="VOTRE_LIEN_GOOGLE_DRIVE_FICHE_TECHNIQUE" class="doc-card" target="_blank">
```
Replace `VOTRE_LIEN_GOOGLE_DRIVE_FICHE_TECHNIQUE` with your actual link or remove this section if not needed.

To remove the technical sheet section, delete lines ~286-301 or set `style="display: none;"` on the link.

### Step 3: Create QR Code

1. Go to [qr-code-generator.com](https://www.qr-code-generator.com) or [qr.io](https://qr.io)
2. Paste your landing page URL
3. Customize (optional: add logo)
4. Download in **high resolution** (PNG 300 DPI minimum)

---

## 📱 Testing Checklist

Before printing QR codes, test on multiple devices:

- [ ] iPhone (Safari)
- [ ] Android/Samsung (Chrome)
- [ ] Tablet (iPad/Android)
- [ ] Desktop browser

**Verify:**
- ✅ Page loads quickly (< 2 seconds)
- ✅ Download buttons work correctly
- ✅ Files open properly
- ✅ Contact emails are clickable
- ✅ Layout looks good on all screen sizes

---

## 🎨 Customization

### Colors

The page uses ValorPack's brand colors defined in the CSS:

```css
Primary Green (Forest): #2C5F2D
Secondary Green (Light): #81C784
Accent Green: #4CAF50
Dark Green: #1a472a
Very Light Green: #E8F5E9
Gold (Badges): #FFD700
Silver (Patent): #C0C0C0
Text: #333333
```

To change colors, search for these hex codes in the HTML file and replace them.

### Key Statistics

To update the three main statistics (lines ~175-195):

```html
<div class="stat">
    <div class="stat-number">45 Mds</div>
    <div class="stat-label">Marché DA/an</div>
</div>
```

Change the numbers and labels as needed.

### Contact Information

Contact details are located around lines ~300-350. Update:
- Email addresses
- Organization names
- Any additional contact methods

---

## 📊 Analytics (Optional)

To track QR code scans and page visits:

### Option 1: Google Analytics

Add this before `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

Replace `GA_MEASUREMENT_ID` with your actual ID.

### Option 2: Simple Counter (No Account)

Use [Counter.dev](https://counter.dev) - add one line before `</body>`:

```html
<script src="https://cdn.counter.dev/script.js" data-id="YOUR_ID"></script>
```

---

## 🔒 Security & Privacy

- **No tracking**: The page contains no tracking scripts by default
- **No cookies**: No cookies are set
- **HTTPS only**: Always use HTTPS hosting (Netlify/GitHub Pages provide this automatically)
- **Public data only**: Never include sensitive information in the landing page

---

## 📂 File Structure

```
valorpack_landing_page.html
├── Inline CSS (lines ~10-230)
│   ├── Responsive layout
│   ├── Brand colors
│   ├── Card styling
│   └── Mobile optimizations
└── HTML Content (lines ~230-400)
    ├── Header section (logo, title, tagline)
    ├── Product name & badges
    ├── Key statistics
    ├── Document download cards
    ├── Contact section
    └── Footer
```

---

## 🌐 Browser Compatibility

Tested and working on:
- ✅ Chrome 90+
- ✅ Safari 14+
- ✅ Firefox 88+
- ✅ Edge 90+
- ✅ Mobile browsers (iOS Safari, Chrome Android)

**No JavaScript dependencies** - Pure HTML/CSS for maximum compatibility.

---

## 📱 Mobile Optimization

The page is fully responsive with:
- **Flexible layouts**: Adapts to all screen sizes
- **Touch-friendly buttons**: Large tap targets (min 48x48px)
- **Readable fonts**: 14px minimum on mobile
- **No horizontal scrolling**: Content fits viewport
- **Fast loading**: < 100KB total size

---

## 🛠️ Troubleshooting

### Issue: Downloads not working

**Solution**: Verify Google Drive links are set to "Anyone with the link" permission.

### Issue: Page looks broken on mobile

**Solution**: Ensure you have the viewport meta tag (line ~5):
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

### Issue: QR code doesn't scan

**Solutions**:
- Ensure QR code is high resolution (300 DPI minimum)
- Test with multiple QR code apps
- Make sure URL is correct and accessible
- Check if URL is too long (shorten with bit.ly if needed)

### Issue: Emails not clickable

**Solution**: Verify `mailto:` links are properly formatted:
```html
<a href="mailto:email@example.com">email@example.com</a>
```

---

## 📈 Best Practices

1. **Test before printing**: Always test QR codes before mass printing
2. **Use short URLs**: Consider URL shorteners for complex domains
3. **Monitor traffic**: Use analytics to track engagement
4. **Keep updated**: Regular update documents in Google Drive
5. **Mobile-first**: Always test on actual mobile devices
6. **Backup links**: Keep alternative contact methods visible

---

## 🎯 Use Cases

### Business Cards
- Small QR code (2x2 cm minimum)
- "Scan for Business Plan" text
- High contrast printing

### Exhibition Stand
- Large QR code (A4 size) on banner
- "Download Complete Documentation" heading
- Include example screenshots

### Printed Materials
- Medium QR code (5x5 cm)
- Brief description of what users will find
- ValorPack branding around QR code

### Email Signatures
- Small QR code (1.5x1.5 cm)
- Clickable link as backup
- Professional formatting

---

## 📧 Support

For questions or issues:
- **Email**: f_menaceur@essaia.dz
- **Alternative**: valorpackco@gmail.com
- **Organization**: ESSAIA - Université de Tébessa

---

## 📄 License

This landing page is part of the ValorPack project documentation.

**Project**: PNR-2021 Food Security
**Institution**: Université de Tébessa
**Director**: Pr. Fouad Menaceur

---

## 🔄 Updates

**Current Version**: 1.0 (January 2026)

### Changelog

**v1.0 - January 2026**
- Initial release
- Mobile-responsive design
- Google Drive integration
- Contact section
- Key metrics display
- Badge system (Patent, PNR EXPO)

---

## 🌟 Features Roadmap

Future enhancements:
- [ ] Multilingual support (French/English/Arabic)
- [ ] Video presentation embed
- [ ] Live chat integration
- [ ] Form for investor inquiries
- [ ] Newsletter signup
- [ ] Social media links

---

# Version Française

## 🎯 Objectif

Cette page d'accueil sert de passerelle mobile pour les investisseurs et parties prenantes qui scannent les codes QR sur :
- Cartes de visite
- Stand d'exposition (PNR EXPO 2026)
- Supports imprimés
- Matériel marketing

Elle donne accès instantané à :
- Business Plan complet (PDF)
- Présentation investisseurs (PowerPoint)
- Spécifications techniques
- Coordonnées directes

---

## ⚙️ Configuration Rapide

### Étape 1 : Obtenir les Liens Google Drive

Pour chaque fichier dans votre Google Drive :

1. **Clic droit** sur le fichier
2. Sélectionner **"Obtenir le lien"**
3. Changer en **"Tous ceux qui disposent du lien"**
4. **Copier le lien**

### Étape 2 : Modifier le Fichier HTML

Ouvrir `valorpack_landing_page.html` et remplacer :

**Ligne ~260 - Business Plan :**
```html
<a href="VOTRE_LIEN_GOOGLE_DRIVE_BUSINESS_PLAN" class="doc-card">
```

**Ligne ~273 - Présentation :**
```html
<a href="VOTRE_LIEN_GOOGLE_DRIVE_PRESENTATION" class="doc-card">
```

**Ligne ~286 - Fiche Technique (optionnel) :**
```html
<a href="VOTRE_LIEN_GOOGLE_DRIVE_FICHE_TECHNIQUE" class="doc-card">
```

### Étape 3 : Héberger la Page

**Option A : Netlify Drop (Le plus rapide)**
1. Aller sur [app.netlify.com/drop](https://app.netlify.com/drop)
2. Glisser-déposer le fichier HTML
3. Obtenir l'URL instantanément

**Option B : GitHub Pages (Le plus professionnel)**
1. Créer compte sur [github.com](https://github.com)
2. Créer repository `valorpack`
3. Upload le fichier renommé `index.html`
4. Activer Pages dans Settings

### Étape 4 : Créer le QR Code

1. Aller sur [qr-code-generator.com](https://www.qr-code-generator.com)
2. Coller l'URL de votre page
3. Télécharger en haute résolution (PNG 300 DPI)

---

## 📱 Liste de Vérification

Avant d'imprimer les QR codes :

- [ ] Test sur iPhone
- [ ] Test sur Android
- [ ] Test sur tablette
- [ ] Téléchargements fonctionnent
- [ ] Emails cliquables
- [ ] Chargement rapide

---

## 🎨 Personnalisation

### Couleurs ValorPack

```css
Vert primaire : #2C5F2D
Vert clair : #81C784
Accent : #4CAF50
Or : #FFD700
Argent : #C0C0C0
```

Pour modifier les couleurs, recherchez ces codes hexadécimaux dans le fichier HTML.

### Statistiques Clés

Pour mettre à jour les trois statistiques principales (lignes ~175-195) :

```html
<div class="stat-number">45 Mds</div>
<div class="stat-label">Marché DA/an</div>
```

### Informations de Contact

Les coordonnées sont situées lignes ~300-350. Mettre à jour :
- Adresses email
- Noms des organisations
- Méthodes de contact supplémentaires

---

## 🛠️ Dépannage

### Problème : Les téléchargements ne fonctionnent pas

**Solution** : Vérifier que les liens Google Drive sont configurés en "Tous ceux qui disposent du lien".

### Problème : La page semble cassée sur mobile

**Solution** : S'assurer que la balise viewport est présente (ligne ~5).

### Problème : Le QR code ne scanne pas

**Solutions** :
- QR code haute résolution (300 DPI minimum)
- Tester avec plusieurs apps
- Vérifier que l'URL est correcte et accessible

---

## 📧 Support

Pour questions ou problèmes :
- **Email** : f_menaceur@essaia.dz
- **Alternatif** : valorpackco@gmail.com
- **Organisation** : ESSAIA - Université de Tébessa

---

## 📄 Licence

Cette page fait partie de la documentation du projet ValorPack.

**Projet** : PNR-2021 Sécurité Alimentaire
**Institution** : Université de Tébessa
**Directeur** : Pr. Fouad Menaceur

---

## 🚀 Déploiement Rapide (Résumé)

```bash
# 1. Modifier les 3 liens Google Drive dans le HTML
# 2. Héberger sur Netlify Drop (2 minutes)
# 3. Créer QR code avec l'URL obtenue
# 4. Tester sur 3 smartphones différents
# 5. Imprimer et distribuer !
```

---

**Dernière mise à jour** : Janvier 2026
**Version** : 1.0
**Contact** : valorpackco@gmail.com
