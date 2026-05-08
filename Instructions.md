

## **Step-by-Step Setup and Execution Guide**

### **1. Activate Python Virtual Environment**

virtual environment is named `.venv`:

```bash
# Linux / macOS
source .venv/bin/activate

```

---

### **2. Install Dependencies from `requirements.txt`**

Make sure you're in the project root directory, then run:

```bash
pip install -r requirements.txt
```

---

### **3. Install `wkhtmltopdf` Executable (for `pdfkit`)**

####  Download `wkhtmltopdf`:

* Go to: [https://wkhtmltopdf.org/downloads.html](https://wkhtmltopdf.org/downloads.html)
* Choose the correct version for your OS (Windows, macOS, Linux)

#### After Installation:

* On **Windows**, add the `bin` folder (e.g., `C:\Program Files\wkhtmltopdf\bin`) to your system `PATH`.
* Test it:

```bash
wkhtmltopdf --version
```

If you don’t want to use `PATH`, specify the path in code (you already do this via `pdfconfig`).

---

### **4. Run the CLI Application**

Assuming your entry point is `cli.py`:

```bash
python CLI.py
```

