<p align="center">
  <img src="../assets/ubuntu.png" width="200">
</p>

## Essentials

#### Update Packages
```bash
sudo apt -y update
sudo apt -y upgrade
```

#### Install Git
```bash
sudo apt -y install git
git config --global user.name "Venus Vavadiya"
git config --global user.email "thisisvenusvavadiya@gmail.com"
```

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
~/miniconda/bin/conda shell.bash
conda init
```

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
```
