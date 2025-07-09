# Premium File Parser

This Python script parses a fixed-width eligibility or premium `.txt` file to extract structured transaction data. It identifies receipt numbers, policy details, transaction types (e.g., refunds, chargebacks), and saves the results in a clean Excel format.

---

## Features
- Parses raw carrier-generated `.txt` files
- Extracts:
  - Policy number
  - Data source
  - Receipt reference number
  - Gross and net premium amounts
  - Refund/chargeback indicators
  - Transaction type classification
- Outputs a structured Excel file with a timestamped filename

---

## Example Use Case
You receive an eligibility or premium file from a vendor/carrier. This script:
1. Scans and extracts core fields
2. Flags potential refunds and chargebacks
3. Prepares a clean, exportable Excel file for auditing or reconciliation

---

## Requirements
- Python 3.7+
- `pandas`
- `openpyxl`

Install via pip:
```bash
pip install pandas openpyxl
```

---

## How to Use
1. Run the script in Google Colab or locally.
2. Upload the `.txt` file when prompted.
3. The script will:
   - Parse all lines
   - Handle basic formatting issues
   - Export results to: `Carrier Billing to Premium Recon (MMM.9.YYYY-MMM.8.YYYY).xlsx`

---

## Sample
A sample file is included:
```
sample_premium_input.txt
```
Use it to test and observe how the parser behaves.

---

## Limitations
- This version focuses on parsing logic only
- Does not yet integrate with billing or payables reconciliation (future scope)

---

## Author
Created by [Tamarl Christie](https://github.com/tamtural) to automate and streamline premium file auditing as part of a larger billing reconciliation pipeline.
