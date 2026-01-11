# QR Code Generator Script

**License:** The license is in `LICENSE.md`. I strongly recommend reading it.

## Description
This script generates QR codes from two input files: `brigadnici.xls` and `config.xlsx`.

- `brigadnici.xls`: Exported from the program CrossChex; contains IDs and time spent at work.
- `config.xlsx`: Contains IDs, names, and, most importantly, IBANs (international bank account numbers). These are required to create QR payments. There is currently no way to calculate IBANs from local account numbers automatically.

The script produces QR codes suitable for payments in the **Czech Republic**.

## Disclaimer
- This script generates QR payments in **Czech format**. Modifications may be required to deploy it in other countries.
- The script **does not calculate taxes** and **does not generate invoices**. Please consult your local laws before using it.
- For licensing inquiries, contact me at **bojanovsky.vit@protonmail.com**.
## Useage
- install Python and then install libs with the `install.sh`
- From CrossChex export the attendance table and save it in the same folder as the script with the name `brigadnici.xls`
- Add a `config.xlsx` that will look like this <img width="515" height="27" alt="image" src="https://github.com/user-attachments/assets/604c5f08-6e32-4ab0-b094-75e726388bf5" /> 
- launch the script with Python
- View the QRCodes in `/QR_Codes` 
  
