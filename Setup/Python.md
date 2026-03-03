# How to setup Python3  In Kali Linux

## Objective

The objective of this lab is to install the latest version of Python 3 on Kali Linux, verify the installation, and configure a virtual environment with Jupyter Notebook for development and lab experimentation.

<img src="https://github.com/niha-v/Home-Lab/blob/main/Screenshots/JupyterNotebook.png" width="500">

## Environment

- Operating System: Kali Linux
- Privileges: Root (sudo access)
- Browser Used: Firefox

## Step 1: Download Python Source Code

- Open Firefox.
- Navigate to the official Python website.
- Download the latest Python 3 Linux source file (.zip or .tar.xz).

## Step 2: Extract the File

- Navigate to the Downloads directory and extract the file:
```bash
cd ~/Downloads
unzip filename.zip
- OR
tar -xf Python-3.x.x.tar.xz
```
## Step 3: Switch to Root User
```bash
sudo su
```
- This provides administrative privileges for system-wide installation.

## Step 4: Configure and Build Python

- Navigate into the extracted directory:
```bash
cd Python-3.x.x
```
- Run the following commands:
```bash
./configure  → Prepares the system for building Python
make → Compiles the source code
make install  → Installs Python system-wide
```
## Step 5: Verify Installation

- Check the installed version:
```bash
python3 --version
```
- Example output:  Python 3.x.x

- Test Python functionality: python3
```python
print("Hello World")
>>> Hello World
```
Successful output confirms proper installation.

## Step 6: Create a Virtual Environment

- Create a virtual environment to isolate project dependencies: 
```bash
python3 -m venv venv
```
- Activate the virtual environment:
```bash
source venv/bin/activate
```
After activation, the terminal will display (venv) indicating the environment is active.

## Step 7: Install Jupyter Notebook

- Install Jupyter Notebook inside the virtual environment:
```bash
pip install jupyter notebook
```
Launch Jupyter Notebook: 
``` bash
jupyter notebook
```
The Jupyter interface should automatically open in the browser.

<img src="https://github.com/niha-v/Home-Lab/blob/main/Screenshots/Hello.png" width="500">
</br> </br>



</br> </br>
## 📬 Author

Niharika Umrani | *Cybersecurity Analyst* 

---
####  🔐 *This home lab is built strictly for educational and ethical cybersecurity practice.*





