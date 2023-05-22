# Python Setup:
------------------------

**Step 1: Install Python**

First, you need to have Python installed on your machine. If you don't have Python installed, you can download it from the official Python website: https://www.python.org/downloads/

**Step 2: Install pip**

Pip is a package manager for Python. It's used to install and manage Python packages. If you installed Python from the official website, pip should have been installed automatically. If not, you can install pip using the following command in your Command Prompt:

For Windows, download `get-pip.py` from https://bootstrap.pypa.io/get-pip.py, then run:

```cmd
python get-pip.py
```

**Step 3: Set up your virtual environment**

Once Python is installed, you'll want to create a virtual environment for this project. Navigate to this project's root folder in your Command Prompt, then run:

```cmd
python -m venv .venv
```

**Step 4: Install required Python packages**

Having completed Step 3, activate the virtual environment from within your project's root folder by running:

```cmd
.venv\Scripts\activate
```

Next install the required Python packages into your virtual environment by running the following from this project's root folder:

```cmd
pip install -r requirements.txt
```

**Step 5: Activating and deactivating your virtual environment**

The virtual environment can be activated in the future by running the following command from your project's root folder:

```cmd
.venv\Scripts\activate
```

and deactivated by running the following command from your project's root folder:

```cmd
deactivate
```

Your command prompt should indicate whether the virtual environment is currently activated by displaying (.venv). Be sure to have the virtual environment activated whenever you want to run the code in this repo.