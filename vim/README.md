# vim

vim 脫胎於 vi, 是大部分系統 (Unix like) 都有內建的文字編輯器, 在某些情境下 (換新電腦, 使用他人的電腦), 不一定會有自己熟悉的 IDE 可以使用, 但通常會有 vim 可以使用!


## 目錄
- [優點](#優點)
- [基本操作](#基本操作)
- [編輯自己的 .vimrc 設定檔](#編輯自己的-.vimrc-設定檔)
- [參考](#參考)

## 優點

### ```通用```
大部分 Unix like 的系統都有內建 vim 文字編輯器

### ```輕巧```
不用額外安裝 IDE 佔電腦的儲存容量

### ```基本功能```
有提供自動縮排, 語法 highlight 等基本的功能, 可以透過設定快速打開


## 基本操作

### 打開檔案
在終端機輸入指令以進入該檔案的普通模式
```sh
vim [檔名]
```

### 進入插入模式
在打開檔案後的普通模式下, 輸入 ```i```

### 回到普通模式
在插入模式下, 按下鍵盤的 ```ESC```

### 儲存改動
在普通模式下輸入
```sh
:w
```

### 返回終端機
在普通模式下輸入
```sh
# 沒有改動, 直接離開
:q

# 儲存改動後離開
:wq

# 放棄改動直接離開
:q!
```


## 編輯自己的 .vimrc 設定檔

### 在終端機下輸入指令
```sh
vim ~/.vimrc
```

### 我的 .vimrc 設定
```sh
set laststatus=2
set number
set cursorline
set cindent
set wrap
set expandtab
set tabstop=4
set shiftwidth=4
syntax on
```

### 設定內容
- 狀態列
```sh
set laststatus=1    # 關
set laststatus=2    # 開
```

- 行號顯示
```sh
set number
set nonumber
```

- 光標底線
```sh
set cursorline
set nocursorline
```

- 自動縮排
```sh
set cindent
set nocindent
```

- 自動換行
```sh
set wrap
set nowrap
```

- tab 轉 space
```sh
set expandtab
set shiftwidth=4
set tabstop=4
set softtabstop=4
```

- 程式碼高亮
```sh
syntax on
syntax off
```

## 參考
- [成大資工Wiki-vimrc設定教學](http://wiki.csie.ncku.edu.tw/vim/vimrc)
