# -Install-without-using-the-Internet
windows 离线安装 python包
# 在有网络的情况下，在终端中执行如下命令，环境中要已经安装好相应的python包
### requirements.txt 中是所需要的安装包，， /tmp/paks/ 是你准备把下载的python 包，放在哪个目录下

pip download  -r requirements.txt  -d  /tmp/paks/

# 把上一步命令执行之后出现的python包，拷贝到想要安装的电脑，执行如下命令

pip install --no-index --find-link="path" -r requirements.txt


path:是你要安装的目录

