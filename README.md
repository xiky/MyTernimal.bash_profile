# MyTernimal.bash_profile


```
vim .bash_profile
```

```

# Setting PATH for Python 3.6
# The original version is saved in .bash_profile.pysave
PATH="/Library/Frameworks/Python.framework/Versions/3.6/bin:${PATH}"
export PATH
# 如果你不是通过Android Studio安装的sdk，则其路径可能不同，请自行确定清楚。
export ANDROID_HOME=~/Library/Android/sdk
export LS_OPTIONS='--color=auto' # 如果没有指定，则自动选择颜色
export CLICOLOR='Yes' # 是否输出颜色
export LSCOLORS='fxfxcxdxbxegedabagGxGx' # 指定颜色

# \h:\w \u\$
#export PS1='\[\033[01;33m\]\u@\h\[\033[01;31m\] \w\$\[\033[00m\] '
export PS1='\[\033[01;33m\]\u@\h\[\033[01;31m\] \w\$\[\e[m\] '

# 2个字母一组分别代表[字体颜色]和[背景颜色]
# 22个字母从第1组到第11组分别指定的文件或文件类型为
# directory
# symbolic link
# socket
# pipe
# executable
# block special
# character special
# executable with setuid bit set
# executable with setgid bit set
# directory writable to others, with sticky bit
# directory writable to others, without sticky bit

# a 黑色
# b 红色
# c 绿色
# d 棕色
# e 蓝色
# f 洋红色
# g 青色
# h 浅灰色
# A 黑色粗体
# B 红色粗体
# C 绿色粗体
# D 棕色粗体
# E 蓝色粗体
# F 洋红色粗体
# G 青色粗体
# H 浅灰色粗体
# x 系统默认颜色

export PATH="/usr/local/opt/openssl/bin:$PATH"
export PATH="$HOME/.rbenv/bin:$PATH"
if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi
```
