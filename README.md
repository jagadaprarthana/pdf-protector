# PDF Password Protection Tool

## Description

A simple and efficient Python script designed to password-protect PDF files. This tool provides an easy-to-use command-line interface for securing your sensitive documents with encryption.

## Features

  * Encrypts PDF files with a user-provided password.
  * Creates a new password-protected PDF without altering the original.
  * Includes basic error handling for `FileNotFoundError` (if the input PDF doesn't exist) and `PyPDF2.errors.PdfReadError` (if the input file is not a valid PDF).

## Prerequisites

Before you can run this script, ensure you have the following installed:

  * **Python 3.x**: You can download Python from [python.org](https://www.python.org/).
  * **PyPDF2 library**: This is the only external Python library required.

## Installation

 **Clone the repository** (or download the `protection.py` and `requirements.txt` files):

    ```bash
    git clone https://github.com/jagadaprarthana/python-pdf-protector.git
    cd python-pdf-protector
    ```

## Usage

To use the script, run it from your terminal with the input PDF path, the desired output PDF path, and the password as arguments:

```bash
python3 protection.py <input_pdf_path> <output_pdf_path> <password>
```

**Arguments:**

  * `<input_pdf_path>`: The full path to the original PDF file you want to protect.
  * `<output_pdf_path>`: The desired full path and filename for the new password-protected PDF.
  * `<password>`: The password you want to set for the output PDF.

**Example:**

```bash
python3 protection.py 'my_document.pdf' my_document.pdf 1234
```

This will create a new file named `my_document.pdf` in the same directory, secured with the password `1234`.

## Error Handling

The script includes basic error handling for the following scenarios:

  * **`FileNotFoundError`**: If the specified input PDF file does not exist.
  * **`PyPDF2.errors.PdfReadError`**: If the input file is not a valid PDF document or is corrupted.

## Contributing

If you have suggestions for improvements or find a bug, feel free to open an issue or submit a pull request\!

## License

This project is licensed under the [MIT License](https://www.google.com/search?q=LICENSE) - see the `LICENSE` file for details.

