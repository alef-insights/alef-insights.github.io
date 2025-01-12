### Step 1: Install Jupyter Book

If you haven't already installed Jupyter Book, you can do so using pip. Open your terminal and run:

```bash
pip install jupyter-book
```

### Step 2: Create the Jupyter Book Directory

Create a new directory for your Jupyter Book:

```bash
mkdir company_name_jupyter_book
cd company_name_jupyter_book
```

### Step 3: Initialize the Jupyter Book

Run the following command to create a new Jupyter Book:

```bash
jupyter-book create .
```

This command will set up the basic structure of your Jupyter Book, including the necessary configuration files.

### Step 4: Add an Example Notebook

Create a new Jupyter Notebook in the `company_name_jupyter_book` directory. You can do this using Jupyter Notebook or by creating a `.ipynb` file directly. For example, create a file named `example_notebook.ipynb` with the following content:

```python
# Example Notebook

# This is a simple example notebook to demonstrate Jupyter Book functionality.

import numpy as np
import matplotlib.pyplot as plt

# Create some data
x = np.linspace(0, 10, 100)
y = np.sin(x)

# Plot the data
plt.plot(x, y)
plt.title('Sine Wave')
plt.xlabel('x')
plt.ylabel('sin(x)')
plt.grid()
plt.show()
```

### Step 5: Update the Table of Contents

Open the `_toc.yml` file in the `company_name_jupyter_book` directory and add your example notebook to the table of contents. It should look something like this:

```yaml
format: jb-book
root: index
chapters:
  - file: example_notebook
```

### Step 6: Configure the Book

Make sure your `pyproject.toml` file is correctly set up. It should look like this:

```toml
[tool.jupyter-book]
title = "Company_Name - Machine Learning Consulting"
author = "The Company_Name Team"
```

### Step 7: Build the Jupyter Book

Now, you can build your Jupyter Book by running:

```bash
jupyter-book build .
```

This command will generate the HTML files for your book in the `_build/html` directory.

### Step 8: Serve the Jupyter Book

To view your Jupyter Book, you can serve it using a simple HTTP server. Run the following command in the `_build/html` directory:

```bash
cd _build/html
python -m http.server
```

Now, open your web browser and go to `http://localhost:8000` to view your Jupyter Book.

### Summary

You have successfully created a functioning Jupyter Book site in the `company_name_jupyter_book` directory, including an example notebook and an automatically generated table of contents. You can now add more content and customize your book as needed!