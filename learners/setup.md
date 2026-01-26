---
title: Setup
---

In this workshop, you’ll learn how to extract data from websites using Python — a process known as web scraping.

Episode 1 begins with an introduction to how websites are structured using HTML.
You’ll learn how to explore this structure using your browser and how to extract information from it using the `BeautifulSoup` package.

In Episode 2, you’ll learn how to retrieve the HTML of a webpage using the `requests` package and continue practicing how to parse and extract specific content with `BeautifulSoup`.

Toward the end of the workshop, in Episode 3, we’ll explore the difference between static and dynamic webpages, and how to scrape dynamic content using `Selenium`.

This workshop is intended for learners who already have a basic understanding of Python. In particular, you should be comfortable with:

- Install and import packages and modules
- Use lists and dictionaries
- Use conditional statements (`if`, `else`, `elif`)
- Use `for` loops
- Calling functions, understanding parameters/arguments and return values

## Software Setup

To run the code in this workshop, you will need to install:

- **The following Python libraries:** `requests, beautifulsoup4, selenium, webdriver-manager, pandas, tqdm, jupyterlab`.
- **Google Chrome:** Please install the latest version of the Google Chrome web browser, as we'll use its web developer tools. If you already have it, please check for updates by visiting `chrome://settings/help` in Chrome.

If you already have a preferred workflow for managing Python environments (e.g., Conda or venv), you may proceed as you normally do. However, if you are new to this or want a hassle-free setup, we highly recommend using `pixi` instructions below.


### Setting up your environment with `pixi`

As described in their website, `pixi` is a cross-platform, multi-language (including Python and R) package manager and workflow tool built on the foundation of the conda ecosystem. In short, it is a tool that simplifies installing software and managing libraries (packages).

Steps to configure your workshop environment::

1. **Install `pixi`:**Follow the instructions for your operating system here [https://pixi.prefix.dev/latest/installation/](https://pixi.prefix.dev/latest/installation/).

    - Note: Once the installation finishes, restart your Terminal (close it and open it again) to make sure the `pixi` command is recognized.

2. **Navigate to your folder:** In your Terminal, use the `cd` command to move to the folder where you want to keep your workshop files (e.g., `cd Desktop` or `cd Documents`).

3. **Initialize the project:** Run the following command to create a new folder named     `webscraping` with the necessary configuration files

```bash
pixi init webscraping
```

4. **Enter the folder:** Move into the newly created project folder

```bash
cd webscraping
```

5. **Install libraries:** Run this command to install Python and all the required tools (this may take a minute) 

```bash
pixi add python requests beautifulsoup4 selenium webdriver-manager pandas tqdm jupyterlab
```

6. **Start JupyterLab:** Launch the notebook interface by running 

```bash
pixi run jupyter lab
```

7. **Verify your setup:** Inside JupyterLab, create a new Notebook (File > New > Notebook), copy the code below into a cell, and run it by pressing <kbd>Shift</kbd>+<kbd>Enter</kbd>

```python
from selenium import webdriver
driver = webdriver.Chrome()
```

You are now ready for the workshop! Learn more about pixi by reading their [documentation](https://pixi.prefix.dev/latest/).

## Additional resources
- Mitchell, R. (Ryan E. ). (2024). Web scraping with Python : data extraction from the modern web (3rd edition.). O’Reilly Media, Inc.
- Chapagain, A. (2023). Hands-On Web Scraping with Python : Extract Quality Data from the Web Using Effective Python Techniques (Second edition.). Packt Publishing.
