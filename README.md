![Spend](https://github.com/user-attachments/assets/f0866e70-57ed-4778-acf7-d9fb964dabe2)

# DoD Spend

## Overview
This Python script searches for publicly available **Department of Defense (DoD) spending PDFs** for **FY 2024 and FY 2025** using Google Search. The script extracts direct PDF links and presents them in a structured, color-coded output for easy readability. It also saves the links to a text file (`dod_spending_pdfs.txt`).

## Features
- **Searches for DoD budget spending PDFs** for fiscal years 2024 and 2025.
- **Extracts direct PDF links** from Google search results.
- **Checks web pages for embedded PDFs** if direct links are not found.
- **Displays results in color** for improved readability.
- **Saves PDF links to a text file** (`dod_spending_pdfs.txt`).

## Requirements
Ensure you have Python installed, then install the required dependencies:

```sh
pip install requests googlesearch-python beautifulsoup4 colorama
```

## Usage
Run the script with:

```sh
python3 dod_spending.py
```

The script will:
1. Search for DoD spending PDFs for FY 2024 and FY 2025.
2. Display the found PDF links in a structured and color-coded format.
3. Save the links to `dod_spending_pdfs.txt`.

This is how it should look:

<img width="1321" alt="Screenshot 2025-02-18 at 2 07 58 PM" src="https://github.com/user-attachments/assets/80454e30-5705-409a-a587-4ef42f1f5ddf" />

Below is a MD example of how it would look:

## Output Example
```
🔵 FY 2024 DoD Budget PDFs

[1] https://defense.gov/FY24_Budget.pdf
[2] https://dod.mil/spending/FY24.pdf

🟢 FY 2025 DoD Budget PDFs

[1] https://defense.gov/FY25_Budget.pdf
[2] https://dod.mil/spending/FY25.pdf

✅ Search complete! PDF links saved in 'dod_spending_pdfs.txt'
```

## Customization
- To **search for additional fiscal years**, modify the `queries` dictionary in the script.
- To **increase the number of search results**, adjust `num_results` in the `find_pdf_links()` function.

## Author

_Michael Mendy (c) 2025._
