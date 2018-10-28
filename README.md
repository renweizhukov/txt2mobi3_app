# txt2mobi3_app

Create a simple PyQt5 application for converting Chinese txt files into mobi files. It wraps [txt2mobi3](https://github.com/renweizhukov/txt2mobi3). Since it supports Chinese only, the documentation and the code comments are written in Chinese.

## 1. 安装和运行

### 1.1. 从PyPI安装和运行：

```bash
$ pip install txt2mobi3_app
$ txt2mobi3_app
```

### 1.2. 从安装包：

(1) Linux

下面以Ubuntu 16.04LTS为例：

```bash
$ sudo dpkg -i target/txt2mobi3_app.deb
```

(2) MacOS

TODO

(3) Windows

TODO

## 2. 产生安装包

这里我们使用[fbs](https://github.com/mherrmann/fbs-tutorial)来产生Linux、MacOS和Windows上的安装包。

### 2.1. Linux

下面以Ubuntu 16.04LTS为例：

(1) [安装fbm](https://fpm.readthedocs.io/en/latest/installing.html)

```bash
$ sudo apt install ruby ruby-dev rubygems build-essential
$ sudo gem install --no-ri --no-rdoc fpm
```

(2) 产生安装包

```bash
$ python -m fbs installer
```

生成的安装包`txt2mobi3_app.deb`会在`target`目录中。

如果想产生一个可以单独运行的可执行文件，那么就运行下面这个fbs命令。

```bash
$ python -m fbs freeze
```

生成的可执行文件位于`target/txt2mobi3_app`目录中。将`target/txt2mobi3_app`目录复制到别的机器上后就可运行其中的可执行文件。

### 2.2. MacOS

TODO

### 2.3. Windows

TODO

## 3. README.rst

README.rst is generated from README.md via `pandoc`.

```bash
$ pandoc --from=markdown --to=rst --output=README.rst README.md
```
