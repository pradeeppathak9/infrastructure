## Steps to setup JupyterHub on Ubuntu

- Install Pip for Python3
```
sudo apt-get install python3-pip
sudo python3 -m pip install -U pip
```

- Install NodeJs 
```
sudo apt-get install -y nodejs npm

```

- Install JupyterHub, JupyterNotebook (Optional), JupyterLab (Optional), IpyWidgets (Optional)
```
sudo python3 -m pip install jupyterhub notebook jupyterlab ipywidgets
sudo npm install -g configurable-http-proxy
```

- Test If JupyterHub is installed properly and working successfully
```
jupyterhub
```



## Setting JupyterHub as a service

- Creare JupyterHub Working Dorectory and Generate JupyterHub Config File
```
sudo mkdir /etc/jupyterhub
cd /etc/jupyterhub
sudo jupyterhub --generate-config
```

- Create JupyterHub Service and add it to systemmd
```
sudo cp jupyterhub.service /etc/systemd/system/.
```
- Enable JupyterHub Service
```
sudo systemctl enable jupyterhub.service 
```

- Service Daemon Reload
```
sudo systemctl daemon-reload
```


- Start JupyterHub Service
```
sudo systemctl start jupyterhub
```

- Check Status of JupyterHub Service
```
sudo systemctl status jupyterhub
```

- Stop JupyterHub Service
```
sudo systemctl stop jupyterhub
```


## Enabling Jupyter Notebook extensions on JupyterHub

- Install Contrib Extension
```
sudo -E pip3 install jupyter_contrib_nbextensions
```

- Enable Extension
```
sudo -E jupyter-contrib-nbextension install --sys-prefix
```
