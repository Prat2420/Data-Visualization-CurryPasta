# Data-Visualization-CurryPasta

*Data Visualization Repository For Team "CurryPasta"*

## Table of Contents

1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
    - [1. Clone the Repository](#1-clone-the-repository)
    - [2. Create and Activate the Virtual Environment](#2-create-and-activate-the-virtual-environment)
        - [Option A: Using `requirements.txt`](#option-a-using-requirementstxt)
    - [3. Verify the Installation](#3-verify-the-installation)
    - [4. Updating Packages in the Environment](#4-updating-packages-in-the-environment)
        - [Example: Adding a New Package](#example-adding-a-new-package)
4. [Usage](#usage)
5. [Additional Help](#additional-help)
    - [Deactivating the Environment](#deactivating-the-environment)
    - [Removing the Environment](#removing-the-environment)
6. [Troubleshooting](#troubleshooting)
7. [Acknowledgments](#acknowledgments)

---

## Introduction

*In this project we develop steps from 1 to 7 from the Data Visualization course.*

---

## Prerequisites

Before diving in, ensure you have the following installed:

- **Python 3.11.5**: [Download here](https://www.python.org/downloads/)
- **Git**: [Download here](https://git-scm.com/downloads)

---

## Installation

Follow these steps to get your environment up and running.

### 1. Clone the Repository

Start by cloning the repository to your local machine:

```bash
git clone https://github.com/Prat2420/Data-Visualization-Team-2.git
cd Data-Visualization-Team-2/
```

---

### 2. Create and Activate the Virtual Environment

#### Option A: Using `requirements.txt`

1. **Create the virtual environment**:

    ```bash
    python3.11 -m venv my_env
    ```

2. **Activate the virtual environment**:

    - On **Windows**:
        ```bash
        my_env\Scripts\activate
        ```

    - On **macOS and Linux**:
        ```bash
        source my_env/bin/activate
        ```

3. **Install dependencies**:

    ```bash
    pip install -r requirements.txt
    ```

---

### 3. Verify the Installation

Ensure that everything is set up properly:

```bash
python your_main_script.py
```

*Replace `your_main_script.py` with the entry point of your application.*

If your project includes tests, run them to confirm all is well:

```bash
pytest
```

---

### 4. Updating Packages in the Environment

As the project evolves, we might need to add new packages to our environment. Below is the process to update the list of packages, ensuring everyone stays in sync.

#### Example: Adding a New Package

Suppose you need to add the package `pydot` to your environment.

**Steps:**

0. **Activate the Environment**

    ```bash
    source my_env/bin/activate
    ```

1. **Add the Package to `requirements.txt`**

    Open the `requirements.txt` file and add:

    ```
    pydot
    ```

2. **Install the New Package**

    Run:

    ```bash
    pip install -r requirements.txt
    ```

3. **Verify the Package is Installed**

    Check that `pydot` is now available in your environment:

    ```bash
    pip list | grep pydot
    ```

    *You should see `pydot` listed among the installed packages.*

4. **Commit the New Version of the Requirements File**

    Ensure the updated `requirements.txt` file is committed to the repository:

    ```bash
    git add requirements.txt
    git commit -m "Updated requirements.txt with new package pydot"
    git push
    ```

---

## Usage

This is a user guide to use the project. This could include:

- Running scripts
- Sample commands
- Expected outputs

**Example**:

```bash
python your_script.py --option value
```

---

## Additional Help

### Deactivating the Environment

When you're done working with the environment, you can deactivate it:

```bash
deactivate
```

### Removing the Environment

To remove the environment entirely, simply delete the directory `my_env`.

---

## Troubleshooting

**Common Issues and Solutions**

- **Issue**: `Environment already exists.`
  - **Solution**: Use a different environment name or remove the existing one.

- **Issue**: `Package conflicts during installation.`
  - **Solution**: Ensure your Python version is up to date and consider creating a fresh environment.

- **Issue**: `New package not found after installation.`
  - **Solution**: Verify that you're in the correct environment and that the installation steps were followed correctly.

---

## Acknowledgments

*List of resources, inspirations, or collaborators.*

---