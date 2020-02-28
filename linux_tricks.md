## 1.find 
```
find .
find . -name **
find . | grep **
```

## 2. ; && ||
```sh
command1 ; command2;...
command1 && command2 && ...
command1 || command2 ||...
```

## 3.Spectial Virables
```
mkdir ~/dirold ;cd -
$_
!$
$?

```

## 4.Unix/Linux Users and groups
```
sudo passwd

chown -R 'whoami':root /
chown -R 'whoami':root /
chmod u=rwx *

```

### 5.ubuntu source
```
mv /etc/apt/source.list /etc/apt/source.list.d

touch /etc/apt/source.list ; vim $_
# 默认注释了源码镜像以提高 apt update 速度，如有需要可自行取消注释
deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic main restricted universe multiverse
# deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic main restricted universe multiverse
deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-updates main restricted universe multiverse
# deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-updates main restricted universe multiverse
deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-backports main restricted universe multiverse
# deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-backports main restricted universe multiverse
deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-security main restricted universe multiverse
# deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-security main restricted universe multiverse

# 预发布软件源，不建议启用
# deb https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-proposed main restricted universe multiverse
# deb-src https://mirrors.tuna.tsinghua.edu.cn/ubuntu/ bionic-proposed main restricted universe multiverse


```

### 6.rm  ls ll
```
ls -l | grep "^-"
ls -l | grep "^d"
find . -type f | grep "^-" | wc -l
find . -name *.txt | xargs rm -f 
```