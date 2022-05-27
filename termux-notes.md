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
vim .termux/termux.properties

extra-keys[ \
    ['ESC','/','`','HOME','UP','END','|'], \
	['TAB','CTRL','ALT','LEFT','DOWN','RIGHT','F5'] \
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
#### 5.python modules
```zsh
pip install Pygments
```


#### 6.install python modules
- 1.numpy
```zsh
curl -L https://its-pointless.github.io/setup-pointless-repo.sh | sh
pkg install numpy
```

<++>




