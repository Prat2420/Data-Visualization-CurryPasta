# Data-Visualization-Team-2

*Data Visualization Repository For Team "CurryPasta"*

## Table of Contents

1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
    - [1. Clone the Repository](#1-clone-the-repository)
    - [2. Create and Activate the Conda Environment](#2-create-and-activate-the-conda-environment)
        - [Option A: Using `environment.yml`](#option-a-using-environmentyml)
        - [Option B: Using `requirements.txt`](#option-b-using-requirementstxt)
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

- **Anaconda or Miniconda**: [Download here](https://docs.conda.io/en/latest/miniconda.html)
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

### 2. Create and Activate the Conda Environment 'data_vis_env'

#### Option A: Using `environment.yml`

This method ensures all dependencies are installed exactly as specified.

1. **Create the environment**:

    ```bash
    conda env create -f environment.yml
    ```

2. **Activate the environment**:

    ```bash
    conda activate data_vis_env
    ```

    *The environment name is defined in the `environment.yml` file. In this project, it's called "data_vis_env"*

#### Option B: Using `requirements.txt`

If you prefer or need to use `pip`, follow these steps:

1. **Create a new environment** (optional but recommended):

    ```bash
    conda create -n data_vis_env python=3.11.5
    conda activate data_vis_env
    ```

2. **Install dependencies**:

    ```bash
    pip install -r requirements.txt
    ```


---

### 3. Verify the Installation
<<<<<<<<<<----to be updated---->>>>>>>>>>>>>>

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
    conda activate data_vis_env
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

3. **Export the Updated Environment**

    Update the `environment.yml` file to reflect the new package:

    ```bash
    conda env export > environment.yml
    ```

4. **Update the Conda Environment**

    Apply the changes to ensure the conda environment matches the `environment.yml`:

    ```bash
    conda env update --file environment.yml --prune
    ```

    *The `--prune` flag removes any packages not listed in the `environment.yml`.*

5. **Verify the Package is Installed**

    Check that `pydot` is now available in your environment:

    ```bash
    pip list | grep pydot
    ```

    *You should see `pydot` listed among the installed packages.*

---

## Usage
<<<<<<<<<<----to be updated---->>>>>>>>>>>>>>
This is a user guide to use the project....

This could include:

- Running scripts
- Sample commands
- Expected outputs

**Example**:

```bash
python your_script.py --option value
```

---

## Additional Help
<<<<<<<<<<----to be updated---->>>>>>>>>>>>>>
### Deactivating the Environment

When you're done working with the environment, you can deactivate it:

```bash
conda deactivate
```

### Removing the Environment

To remove the environment entirely:

```bash
conda remove --name your-env-name --all
```

---

## Troubleshooting
<<<<<<<<<<----to be updated---->>>>>>>>>>>>>>
**Common Issues and Solutions**

- **Issue**: `Environment already exists.`
  - **Solution**: Use a different environment name or remove the existing one.

- **Issue**: `Package conflicts during installation.`
  - **Solution**: Ensure your conda version is up to date and consider creating a fresh environment.

- **Issue**: `New package not found after installation.`
  - **Solution**: Verify that you're in the correct environment and that the installation steps were followed correctly.

---

## Acknowledgments
<<<<<<<<<<----to be updated---->>>>>>>>>>>>>>
*List of resources, inspirations, or collaborators.*

---
