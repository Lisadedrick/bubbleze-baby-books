# Bubbleze Fix Pack
Use these files if your workflow failed.

## What to upload
- `.github/workflows/build.yml`
- `requirements.txt`
- `scripts/generate_books.py`
- Your catalog CSV in `catalog/Product_Catalog.csv` (or set a repo variable `CATALOG_FILE` to another path like `catalog/Product_Catalog_25.csv`).

## Steps
1. In your repo, click **Add file → Upload files** and upload the three files above to the same paths.
2. Ensure your catalog exists at `catalog/Product_Catalog.csv`, or go to **Settings → Secrets and variables → Actions → Variables → New repository variable**:

   - **Name**: `CATALOG_FILE`

   - **Value**: `catalog/Product_Catalog_25.csv` (or whatever your filename is)

3. Go to **Actions → Build Digital Products → Run workflow** (branch: main).
4. After success, download the **build-outputs** artifact.
