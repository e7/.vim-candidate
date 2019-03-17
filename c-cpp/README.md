1. 引入YCM插件后需要到插件目录下编译以支持c家族的补全
```
./install.py --clangd-completer
```

2. 用以下内容替换插件目录下的文件.ycm_extra_conf.py
```
# Add your flags to this list.
flags = [
    '-x',
    'c++',
]

def FlagsForFile(filename):
    return {'flags': flags}
```

3. enjoy
