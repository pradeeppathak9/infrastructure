### - Steps to setup JupyterHub, JupyterLab on Ubuntu

##### Install pip for python3
sudo apt-get install python3-pip

##### Install nodejs 
sudo apt-get install -y nodejs

##### Install Jupyterhub, notebook, Jupyterlab, ipywidgets

sudo python3 -m pip install jupyterhub notebook jupyterlab ipywidgets
sudo npm install -g configurable-http-proxy

##### Test If Jupyterhub is installed properly and working successfully
jupyterhub


### - Setting JupyterHub as a service

##### Creare JupyterHub Working Dorectory and Generate JupyterHub Config File
sudo mkdir /etc/jupyerhub
cd /etc/jupyterhub
sudo jupyterhub --generate-config



