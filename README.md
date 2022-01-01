# bash_chinese
与中文终端文件名补全的一些资料收集和想法

# `bash` 是可以自动补全的

打开 `.bashrc` 可以看到

```bash
# enable programmable completion features (you don't need to enable
# this, if it's already enabled in /etc/bash.bashrc and /etc/profile
# sources /etc/bash.bashrc).
if ! shopt -oq posix; then
  if [ -f /usr/share/bash-completion/bash_completion ]; then
    . /usr/share/bash-completion/bash_completion
  elif [ -f /etc/bash_completion ]; then
    . /etc/bash_completion
  fi
fi
```

# 相关

https://github.com/scop/bash-completion

https://www.cnblogs.com/gmpy/p/13202562.html

# 操作方法

## `Tab` 补全
```
# cd
$ cd zhuomian
```

希望可以在按 `Tab` 之后补全出来`桌面`

## `thefuck` 补全
```
$ cd zhuomian
bash: cd: zhuomian: 没有那个文件或目录
$ fuckime!!!
cd 桌面 [Enter/Ctrl+C]
```
## 第三方命令补全

```
$ zhcd zhuomian
```
前两个我都不会做这个我会，但是感觉不优美
