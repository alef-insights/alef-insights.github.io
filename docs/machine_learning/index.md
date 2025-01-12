### Step 1: Install Jupyter Book

If you haven't already, you need to install Jupyter Book. You can do this using pip:

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

Create a new notebook in the `company_name_jupyter_book` directory. You can do this by creating a new file with a `.ipynb` extension. For example, create a file named `example_notebook.ipynb`:

```bash
touch example_notebook.ipynb
```

You can open this notebook using Jupyter Notebook or JupyterLab and add some content to it. For example, you might add a simple code cell that prints "Hello, World!".

### Step 5: Update the Table of Contents

Open the `_toc.yml` file in the `company_name_jupyter_book` directory. This file defines the structure of your book. You can add your example notebook to the table of contents like this:

```yaml
format: jb-book
root: intro
chapters:
  - file: example_notebook
```

Make sure to adjust the `root` entry if you have an introduction file (like `intro.md`).

### Step 6: Configure the Book

Open the `config.yml` file in the `company_name_jupyter_book` directory and ensure it includes the following settings:

```yaml
title: "Company_Name - Machine Learning Consulting"
author: "The Company_Name Team"
```

### Step 7: Build the Jupyter Book

Now that you have set up your Jupyter Book, you can build it using the following command:

```bash
jupyter-book build .
```

This command will generate the HTML files for your book in the `_build/html` directory.

### Step 8: Serve the Jupyter Book Locally

To view your Jupyter Book, you can serve it locally using:

```bash
jupyter-book serve .
```

This will start a local server, and you can view your book in your web browser at `http://localhost:4000`.

### Summary

You have now created a functioning Jupyter Book site in the `company_name_jupyter_book` directory, including an example notebook and an automatically generated table of contents. You can continue to add more content and customize your book as needed!