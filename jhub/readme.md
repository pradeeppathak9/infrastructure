# STeps to setup JupyterHub, JupyterLab on Ubuntu

# Install pip for python3
sudo apt-get install python3-pip

# Install nodejs 
sudo apt-get install -y nodejs

# Install jupyterhub, notebook, jupyterlab, ipywidgets

sudo python3 -m pip install jupyterhub notebook jupyterlab ipywidgets
sudo npm install -g configurable-http-proxy

# generate jupyter hub config
sudo mkdir /etc/jupyerhub
cd /etc/jupyterhub
sudo jupyterhub --generate-config



