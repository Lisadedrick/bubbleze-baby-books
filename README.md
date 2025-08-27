# Bubbleze Baby Books — GitHub Builder
Generate KDP-ready interiors (DOCX + PDF) **in the cloud** using GitHub Actions — no local installs, no n8n needed.

### Quick Start
1. Create a **new GitHub repo** and upload these files.
2. Repo → Settings → Secrets and variables → Actions → **New repository secret**:
   - `OPENAI_API_KEY` = your key (optional; if absent, uses a soothing template).
3. Edit `catalog/Product_Catalog.csv` or replace with your 25-row file.
4. Actions tab → **Build Digital Products** → **Run workflow**.
5. Download the `build-outputs` artifact (ZIP) with all DOCX + PDFs.

### Canva Pro Bulk Covers
Apps → Bulk Create → upload `catalog/canva_bulk_covers.csv` and bind fields. Export PNGs as `cover_###.png`.
