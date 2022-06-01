The azure-cli deb package does not support ARM64 architecture, the solution is to install azure-cli from PyPI as a workaround (https://github.com/Azure/azure-cli/issues/20476)

## Install Azure CLI with pip

Azure CLI is built on Python. The supported Python versions are 3.7 ~ 3.10.

Directly running pip install azure-cli installs Azure CLI system-wide and may cause conflicts with other Python libraries. Instead, we recommend installing Azure CLI in a virtual environment.

First make sure python3 and its related packages are installed:

### Ubuntu/Debian 
```sudo apt install python3 python3-venv --yes```

Then continue the installation:

### Create a virtual environment 
```python3 -m venv azure-cli-env```

### Update pip 
```azure-cli-env/bin/python -m pip install --upgrade pip```

### Install azure-cli 
```azure-cli-env/bin/python -m pip install azure-cli```

### Run any Azure CLI commands 
```azure-cli-env/bin/az --version```

## Install arcdata extension

```azure-cli-env/bin/az extension add --name arcdata```
