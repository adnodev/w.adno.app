# ADNO

Adno is a web application for viewing, editing and sharing narratives and pathways on static images and IIIF images.

---

## Getting started

### Use Adno locally

1. Download the latest release from [github.com/adnodev/adno/releases](https://github.com/adnodev/adno/releases)
2. Unzip the archive
3. Start a local web server from the unzipped folder — for example with Python:
   ```bash
   python -m http.server 8080
   ```
4. Open [http://localhost:8080](http://localhost:8080) in your browser

---

### Host Adno on GitHub Pages

1. Download and unzip the latest release
2. Push the contents to a GitHub repository
3. In your repository, go to **Settings → Pages**
4. Select the branch to deploy from and save

Your Adno instance will be live at `https://<your-username>.github.io/<your-repo>`.

---

## IIIF image examples

- [ronallo.com — example manifests](https://ronallo.com/iiif-workshop/presentation/example-manifests.html)
- `https://free.iiifhosting.com/iiif/1c8d49343676a04fffcd92979c02e9394e48bac96f590fffbadffc9133cd06b9/info.json`
- `https://iiif.emf.fr/iiif/3/peutinger.jp2/info.json`
- `https://iiif.emf.fr/iiif/3/saint-savin.jpg/info.json`

---

## For developers

### Setup

```bash
git clone https://github.com/adnodev/adno.git
cd adno
cp .env.example .env   # fill in your values
npm install
npm run dev
```

### Build

```bash
npm run build
```

> If you run into issues, delete `node_modules` and `package-lock.json` then reinstall with `npm install`.

### Customize your instance

Edit your `.env` file with the following variables:

```env
# Analytics (Matomo)
MATOMO_SITE_ID=your-site-id
MATOMO_URL=https://your-matomo-instance.com

# App title
ADNO_TITLE=My Adno Instance

# Footer
ADNO_FOOTER=true
ADNO_FOOTER_TEXT=Your footer text here
```

---

## Licence

See [LICENCE](https://github.com/adnodev/adno/blob/main/LICENCE).
