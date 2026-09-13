# 🌍 CarbonSense: AI-Powered Supply Chain Emissions Intelligence

## The Problem
As ESG regulations tighten globally (like the CSRD in Europe), companies are facing immense pressure to report their **Scope 3 (supply chain) emissions**. However, supply chain data is famously fragmented, messy, and manual. Companies struggle to calculate accurate carbon footprints across multi-tier suppliers, spot anomalies, and identify actionable ways to reduce their impact.

## Our Solution
**CarbonSense** is an intelligent, automated platform that transforms raw, incomplete supplier manifests into verified GHG (Greenhouse Gas) totals, actionable insights, and auditable reports. 

We don't just calculate carbon—we use machine learning to fill in the blanks, flag hidden risks, and actively recommend greener alternatives.

## ✨ Key Features for a Sustainable Future

- 🚀 **Automated Data Ingestion & Imputation** 
  Upload a messy CSV of your suppliers. If data like electricity usage or transport distance is missing, our ML regression models accurately predict and impute the gaps based on peer group analysis.
- 🔬 **Verified Emission Calculations** 
  We use hardcoded, official government emission factors (UK Govt GHG Conversion Factors, EPA GHG Emission Factors Hub) to calculate the precise CO2 impact of energy usage, transport routes, and material processing.
- 🚨 **AI Anomaly Detection (Isolation Forest)** 
  Automatically flag "MegaPolluters" or suppliers whose emissions are way outside the normal distribution for their specific tier and material type.
- 📊 **Supplier Clustering & Intelligence (KMeans)** 
  Group suppliers into distinct pollution-pattern buckets to help procurement teams prioritize which groups need immediate intervention.
- 🔄 **Circular Sourcing Recommendations** 
  Using cosine similarity, the platform proactively suggests similar-but-cleaner suppliers within your network to switch to, lowering your overall carbon footprint effortlessly.
- 📋 **One-Click ESG Auditing** 
  Export full, enriched datasets and beautifully formatted PDF audit reports for immediate compliance reporting.

## 🛠️ How It Works (The Magic Behind the Scenes)
1. **Upload:** Drop in your CSV.
2. **Cleanse & Predict:** Our AI pipeline fills missing data and validates inputs.
3. **Calculate:** Base emissions are calculated using official factors.
4. **Analyze:** Machine learning models (Isolation Forest, KMeans) run over the data to tag anomalies and cluster profiles.
5. **Recommend:** We run a similarity search to find greener supplier swaps.
6. **Visualize:** You get an interactive dashboard with tree views, charts, and downloadable reports.

## 💻 Tech Stack
We built CarbonSense for speed, scale, and intelligence:
- **Frontend:** Next.js, Tailwind CSS, Recharts, Framer Motion (for a stunning, responsive UI)
- **Backend:** FastAPI, Python (optimized for fast data processing)
- **AI & ML Pipeline:** scikit-learn (Regression, Isolation Forest, KMeans), Pandas, Numpy
- **Database:** MongoDB (for flexible, high-performance document storage)
- **Export Engine:** ReportLab for instant PDF generation

## 🎯 Impact
CarbonSense turns an expensive, months-long consulting project into a 10-second automated pipeline. We empower corporate sustainability teams and supply chain managers to stop wrestling with spreadsheets and start making data-driven decisions to save the planet.
