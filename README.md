# Data-Visualization-CurryPasta

*Data Visualization Repository For Team "CurryPasta"*

## Table of Contents

1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
    - [1. Clone the Repository](#1-clone-the-repository)
    - [2. Create and Activate the Virtual Environment](#2-create-and-activate-the-virtual-environment)
        - [Option A: Using `requirements.txt`](#option-a-using-requirementstxt)
    - [3. Updating Packages in the Environment](#3-updating-packages-in-the-environment)
        - [Example: Adding a New Package](#example-adding-a-new-package)
4. [Usage](#usage)


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
https://github.com/Prat2420/Data-Visualization-CurryPasta.git
cd Data-Visualization-CurryPasta/
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

### 3. Updating Packages in the Environment

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

To use the implemented steps of the project, go to the Notebooks folder and run either individual step notebooks (step_1.ipynb, step_2.ipynb, etc.) or the comprehensive all_in_one_final.ipynb that contains the most up-to-date implementation of all visualization techniques.

