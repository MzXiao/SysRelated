### 1.Homebrew 
sonshi-style
```sh
cd "$(brew --repo)"
git remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/brew.git

cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://mirrors.tuna.tsinghua.edu.cn/git/homebrew/homebrew-core.git

```

### 2.
```
sudo chown -R `whoami`:admin /usr/local/bin
sudo chown -R `whoami`:admin /usr/local/share
```

### 2.Python
```sh
brew update
brew install python3
echo -e "[global] \nindex-url = https://pypi.tuna.tsinghua.edu.cn/simple" > pip.conf
pip3 install virtualenv


mkdir ~/Documents/VirtualEnvs ; cd  -
virtualenv --no-site-packages venv
cd venv/bin ; ./activate
deativate

```
