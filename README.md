### Step 1: Install Jupyter Book

Make sure you have Jupyter Book installed. You can install it using pip:

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

This command will set up the basic structure of your Jupyter Book, including a default table of contents.

### Step 4: Add an Example Notebook

Create a new Jupyter Notebook in the `company_name_jupyter_book` directory. You can do this using Jupyter Notebook or by creating a `.ipynb` file directly. For example, create a file named `example_notebook.ipynb`:

```bash
touch example_notebook.ipynb
```

You can open this notebook in Jupyter Notebook or JupyterLab and add some content. Here’s a simple example of what you might include:

```python
# example_notebook.ipynb
{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Example Notebook\n",
    "\n",
    "This is an example notebook for the Jupyter Book.\n",
    "\n",
    "## Introduction\n",
    "This notebook demonstrates how to create a Jupyter Book."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "print('Hello, Jupyter Book!')"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.8.5"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 4
}
```

### Step 5: Update the Table of Contents

Open the `_toc.yml` file in the `company_name_jupyter_book` directory and add your example notebook to the table of contents. It should look something like this:

```yaml
# _toc.yml
format: jb-book
root: index
chapters:
  - file: example_notebook
```

### Step 6: Build the Jupyter Book

Now that you have your notebook and table of contents set up, you can build your Jupyter Book:

```bash
jupyter-book build .
```

### Step 7: Serve the Jupyter Book Locally

To view your Jupyter Book, you can serve it locally using:

```bash
jupyter-book serve .
```

This will start a local server, and you can view your Jupyter Book in your web browser at `http://localhost:4000`.

### Summary

You have now created a functioning Jupyter Book site in the `company_name_jupyter_book` directory, including an example notebook and an automatically generated table of contents. You can continue to add more content and customize your book as needed!