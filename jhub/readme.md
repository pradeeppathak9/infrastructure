## - Steps to setup JupyterHub on Ubuntu

##### Install Pip for Python3
sudo apt-get install python3-pip

##### Install NodeJs 
sudo apt-get install -y nodejs

##### Install JupyterHub, JupyterNotebook (Optional), JupyterLab (Optional), IpyWidgets (Optional)

sudo python3 -m pip install jupyterhub notebook jupyterlab ipywidgets
sudo npm install -g configurable-http-proxy

##### Test If JupyterHub is installed properly and working successfully
jupyterhub


## - Setting JupyterHub as a service

##### Creare JupyterHub Working Dorectory and Generate JupyterHub Config File
sudo mkdir /etc/jupyerhub
cd /etc/jupyterhub
sudo jupyterhub --generate-config



