## A simple command line tool to convert GBK to UTF-8

```
$ g2u

Usage:
    g2u [file] [-r dirname --file-exts=[ext]]

Options:
    -r|-R             在指定目录解析
    --file-exts       指定特定文件后缀名,多后缀名以'|'分割,例如: --file-exts=js|java
    -v                命令行版本
    -h                用法说明
```

### 转换单个文件

```
$ g2u gbk_file
```

### 转换指定目录下的所有文件（嵌套）

```
// 默认全部转换
$ g2u -r gbk_dir

// 只转换`.java`和`.js`后缀的文件
$ g2u -r gbk_dir --file-exts=java|js
```
