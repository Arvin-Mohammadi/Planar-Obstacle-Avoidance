# Python Virtual Environment 

This script follows a standard procedure for making a new Python virtual environment in Microsoft Windows OS:

```cmd
# install the virtual environment
python -m pip install --user virtual env

# create the vm
python -m venv my_env_name

# activating the vm
.\my_env_name\scripts\activate
```

In order to install other dependencies you have to go to the file `./my_env_name/pyvenv.cfg` and change the line 
`include-system-site-packages = false` to `include-system-site-packages = true` then run the following commands:

```cmd
# upgrade pip
python -m pip install --upgrade pip

# install new packages
python -m pip install -U --force-reinstall package_name
```

Since you'll likely be using Jupyter Notebook you need to add the vm to the kernel via the following commands:

```cmd
# adds the vm to jupyter notebook
python -m ipykernel install --user --name=my_env_name

# removes the vm from jupyter notebook
python -m jupyter kernelspec uninstall my_env_name
```

