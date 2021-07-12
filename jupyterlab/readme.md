```
sudo systemctl stop jupyterlab
sudo systemctl disable jupyterlab
sudo cp jupyterlab.service /etc/systemd/system/
sudo systemctl daemon-reload
sudo systemctl enable jupyterlab
sudo systemctl start jupyterlab
sudo systemctl status jupyterlab
```
