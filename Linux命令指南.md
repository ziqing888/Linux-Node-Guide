# Linux 命令

* [前 50 条命令](https://www.digitalocean.com/community/tutorials/linux-commands)

* [Linux 命令](https://github.com/trinib/Linux-Bash-Commands)

* [101 条 Linux 命令](https://github.com/bobbyiliev/101-linux-commands-ebook)

### ls：列出目录
```console
# 列出目录
ls

# 列出所有目录，包括隐藏目录
ls -a
```
mkdir：创建目录
```console
# 创建文件夹 - 替换 <文件夹名称>
mkdir <文件夹名称>

# 创建两个文件夹
mkdir <文件夹名称1> <文件夹名称2>

# 创建名为 moei 的文件夹
mkdir moei
```
cd：进入目录
```console
# 进入主目录或根目录
cd

# 进入自定义目录，替换 <目录路径>
cd <目录路径>

# 进入 moei 目录
cd moei

# 返回上一级目录
cd ..
```
mv：移动文件和目录
```console
# 移动 <源> 到 <目标>
mv <源> <目标>
```
rm：删除文件
```console
# 删除文件
rm -rf <文件>

# 删除目录中的文件
rm -rf <目录/文件>
```
nano：编辑文件
```console
# 打开文件的编辑菜单 / 如果文件不存在则创建
nano <文件>

# 使用 CTRL + X + Y + ENTER 保存并退出

```
git：版本控制
```console
# 将 GitHub 仓库下载到 Linux
git clone https://github.com/0xmoei/Linux_Node_Guide
```
Screen：后台运行进程
有时需要在退出终端和 VPS 后保持进程在后台运行。
可以打开一个 screen 会话，在其中运行节点命令。
关闭会话后可以稍后返回该会话。
```console

# 安装 Screen
sudo apt install screen

# 打开一个 screen 会话
screen -S <screen-name>

# 关闭会话
CTRL + A + D

# 列出所有会话
screen -ls

# 返回指定会话
screen -r <screen-name>
```
