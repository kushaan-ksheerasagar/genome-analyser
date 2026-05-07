# 🧬 Genome Analyser

A professional AI-powered genomic analysis platform. Upload any VCF file and get:

- **Ancestry** — Population composition using 1000 Genomes Phase 3 reference panels (AFR, AMR, EAS, EUR, SAS)
- **80+ Traits** — Nutrition, metabolism, physical traits, athletic profile, neurology, sleep, immune, cardiovascular
- **Pharmacogenomics** — 25+ drug-gene interactions with CPIC Level A/B guidance
- **Polygenic Risk Scores** — Lab-style gauge with percentile and Z-score for 5 conditions
- **AI Reports** — Separate Claude-powered narrative reports for each module

---

## 🚀 Running Locally

### 1. Clone the repo
```bash
git clone https://github.com/YOUR_USERNAME/genome-analyser.git
cd genome-analyser
```

### 2. Install dependencies
```bash
npm install
```

### 3. Start the app
```bash
npm start
```

The app opens at `http://localhost:3000`

---

## 🔑 API Key (for AI Reports)

The VCF analysis (ancestry, traits, PGx, PRS) works **without any API key**.

The AI report generation uses the Claude API. Enter your key in the upload screen.

Get a free key at: [console.anthropic.com](https://console.anthropic.com)

Your key is stored **only in your browser** (localStorage). It never leaves your device.

---

## 📦 Deploying (Free)

### Vercel (recommended — one command)
```bash
npx vercel
```

### Netlify
```bash
npm run build
# Drag the /build folder to netlify.com/drop
```

---

## 🧬 What's Inside

| Module | Details |
|---|---|
| VCF Parser | Full VCF parsing with QC stats (Ts/Tv, heterozygosity, depth, GQ) |
| Ancestry | Naive Bayes likelihood across 26 AIMs from 1000 Genomes Phase 3 |
| Traits | 80+ SNPs across 10 categories, GWAS-referenced |
| Pharmacogenomics | 25+ variants, CPIC Level A/B, star-allele phenotypes |
| PRS | 5 conditions, PGS Catalog IDs, percentile + Z-score + gauge |
| AI Reports | 5 separate Claude-powered reports + 1 integrated report |

---

## ⚠️ Disclaimer

For educational and wellness purposes only. Not a clinical diagnosis. Consult a healthcare professional for any health decisions.
