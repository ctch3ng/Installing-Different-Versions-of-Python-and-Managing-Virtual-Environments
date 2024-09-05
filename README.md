# Installing-Different-Versions-of-Python-and-Managing-Virtual-Environments
This guide provides a step-by-step process to install different versions of Python and manage them using virtual environments.

## Steps

### 1. Add the Deadsnakes Repository

```
sudo add-apt-repository ppa:deadsnakes/ppa
```
### 2. Update Package Lists

```
sudo apt update
```

### 3. Install Python 3.9 (or other versions)

```
sudo apt install python3.9
```

### 4. Install the `venv` Package for Python 3.9

```
sudo apt install python3.9-venv
```

### 5. Make a (hidden) Folder for Virtual Environments

```
mkdir ~/.venvs
```

### 6. Create a New Virtual Environment `my-venv-name` with Python 3.9

```
python3.9 -m venv ~/.venvs/my-venv-name
```
### 7. Activate the New Virtual Environment `my-venv-name`

```
source ~/.venvs/my-venv-name/bin/activate
```

### 8. Check the Python Version Inside the Virtual Environment

```
python -V
```

### 9. Check the Pip Version Inside the Virtual Environment

```
pip3 --version
```
### 10. Deactivate the Virtual Environment (After finish using the VENV)

```
deactivate
```

