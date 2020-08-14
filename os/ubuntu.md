<p align="center">
  <img src="../assets/ubuntu.png" height="100">
</p>

## Essentials

#### Update Packages
```bash
sudo apt -y update
sudo apt -y upgrade
```

#### Install Git

I am using my details.
```bash
sudo apt -y install git
git config --global user.name "Venus Vavadiya"
git config --global user.email "thisisvenusvavadiya@gmail.com"
```

Generate and copy SSH Key.
```bash
cat /dev/zero | ssh-keygen -q -N "" > /dev/null
sudo apt -y install xsel
cat  ~/.ssh/id_rsa.pub | xsel -i -b
```

Add it to GitHub. https://github.com/settings/keys

## Languages

#### Install Node
```bash
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
nvm install node
```

#### Install Python
```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda.sh
bash ~/miniconda.sh -b -p $HOME/miniconda
~/miniconda/bin/conda init
```

---

## Databases

#### Install MongoDB
```bash
sudo apt -y install mongodb
sudo systemctl enable mongodb
```

#### Install MySQL
```bash
sudo apt -y install mysql-server
sudo systemctl enable mysql
sudo apt -y install libmysqlclient-dev
```

---

## Fixes

#### Watchers
```bash
echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p
```
---

#### TODO
- [x] Install MongoDB
- [ ] Install MongoDB Compass
- [x] Install MySQL
- [ ] Install MySQL Workbench
- [ ] Install Visual Studio Code
- [ ] Install Postman
