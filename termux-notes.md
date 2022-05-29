#### 1.Get Storage
```shell
termux-setup-storage
```

#### 2.修改启动问候语
```shell
vim $PREFIX/etc/motd
```

#### 3.自定义快捷栏
```shell
mkdir .termux
cd .termux
vim termux.properties

extra-keys=[ \
    ['ESC','/','`','HOME','UP','END','|'], \
	['TAB','CTRL','F2','LEFT','DOWN','RIGHT','F5'] \
]
```

#### 4.镜像源设置
1. 手动设置
```bash
nvim /data/data/com.termux/files/usr/etc/apt/sources.list
```
- [中国科技大学源](https://mirrors.ustc.edu.cn/termux/)
```list
deb https://mirrors.ustc.edu.cn/termux/apt/termux-main stable main
```
2. 自动设置
```bash
pkg install termux-tools
termux-change-repo
```
#### 5.pkg install
```bash
pkg install git nodejs wget curl ranger neovim zsh fzf
```

#### 6.ln
```bash
cd ~

ln -s /data/data/com.termux/files/home/storage/pictures ./
ln -s /data/data/com.termux/files/home/storage/downloads ./
```


#### 7.python modules
```zsh
pip install Pygments
```


#### 8.termux-style
```bash
git clone https://github.com/adi1090x/termux-style
cd termux-style
chmod +x install
./install

termux-style
```








