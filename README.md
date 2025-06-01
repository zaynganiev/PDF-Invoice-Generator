# PDF Invoice Generator

This is an app that creates PDF invoices from Excel files.

## Features

- Reads Excel files from the `invoices/` directory
- Extracts invoice number and date from the filename
- Generates a styled PDF invoice for each Excel file
- Outputs PDFs to the `PDFs/` directory

## Requirements

- Python 3.7+
- [pandas](https://pandas.pydata.org/)
- [fpdf](https://pyfpdf.github.io/)
- [openpyxl](https://openpyxl.readthedocs.io/) (for reading Excel files)

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/zaynganiev/pdf-template.git
    cd pdf-template
    ```

2. Create and activate a virtual environment (optional but recommended):
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Place your Excel invoice files in the `invoices/` directory.  
   Filenames should be in the format: `invoiceNumber_date.xlsx` (e.g., `1234_2024-06-01.xlsx`).

2. Run the script:
    ```bash
    python main.py
    ```

3. Generated PDF invoices will appear in the `PDFs/` directory.

## File Structure

```
pdf-template/
├── invoices/
│   └── <your Excel files>.xlsx
├── PDFs/
│   └── <generated PDFs>.pdf
├── main.py
├── requirements.txt
└── README.md
```

## License

MIT License