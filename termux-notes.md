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
pkg install git nodejs wget curl ranger neovim zsh fzf w3m-img neofetch
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
pip install ueberzug
```


#### 8.termux-style
```bash
git clone https://github.com/adi1090x/termux-style
cd termux-style
chmod +x install
./install

termux-style
```

```bash
cd ~/termux-style
./tstyle
F
[19]Source-Code-Pro
```
#### 9.linux systrm
```bash
pkg install proot-distro

# 查看可以安装的发行版
proot-distro list
proot-distro install archlinux

# 进入ubuntu
proot-distro login archlinux
```

# nerd fonts
```bash
git clone https://github.com/lcdse7en/fonts.git
cd fonts/nerdi\ fonts/JetBrainsMono
# mv nerdfont.ttf ~/.termux/font.ttf
mv JetBrains\ Mono\ Bold\ Italic\ Nerd\ Font\ Complete\Mono.ttf ~/termux/font.ttf

pkg install lsd
termux-reload-settings
```

<++>










