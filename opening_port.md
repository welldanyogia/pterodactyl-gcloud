```shell
sudo ufw enable
```
```shell
sudo ufw allow mysql && sudo ufw allow OpenSSH && sudo ufw allow ssh && sudo ufw allow 80 && sudo ufw allow 443 && sudo ufw allow 2022 && sudo ufw allow 8080
```
```shell
sudo vi /etc/ssh/sshd_config
```
```shell
Port 22
PermitRootLogin yes
PasswordAuth yes
```
```shell
sudo systemctl restart sshd
```
```shell
bash <(curl -s https://pterodactyl-installer.se)
```
```shell
Do you want to automatically configure UFW (firewall)? (y/N): N
Do you want to automatically configure HTTPS using Let's Encrypt? (y/N): y
I agree that this HTTPS request is performed (y/N): y
Initial configuration completed. Continue with installation? (y/N): y
Enable sending anonymous telemetry data? (yes/no) [yes]:
 > yes
```
