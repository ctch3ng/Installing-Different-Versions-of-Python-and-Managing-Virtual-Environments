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
- Note 1: You can change `my-venv-name` to your preferred name.
- Note 2: You can also specify Python versions other than 3.9; however, the latest version is not always the most supported one. Beware!

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

### 11. (Optional) Make the Virtual Environment as an IPython Kernel for Jupyter Notebook

- Active the environment, `my-venv-name`, again

```
source ~/.venvs/my-venv-name/bin/activate
```
- Install `ipython` and `ipykernel`

```
pip install ipython ipykernel
```

- Configure the IPython Kernel for Jupyter Notebook

```
python -m ipykernel install --user --name=my-venv-name --display-name "My First Customised Kernel"
```

