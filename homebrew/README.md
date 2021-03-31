# homebrew

homebrew 為 mac 的套件管理工具, 可以集中管理各式應用程式


## 目錄
- [安裝/卸載](#安裝/卸載)
- [管理套件](#套件管理)
- [參考](#參考)


## 安裝/卸載

### 安裝
```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### 卸載
```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/uninstall.sh)"
```

### 更新
```sh
brew update
```


## 套件管理

### 搜尋套件
```sh
brew search [套件名稱]
```

### 安裝套件
```sh
brew install [套件名稱]
```

### 卸載套件
```sh
brew uninstall [套件名稱]
```

### 更新已安裝套件
```sh
brew upgrade [套件名稱]
```

### 列出已安裝套件清單
```sh
brew list
```

### 清理過期暫存檔
```sh
brew cleanup
```

## 參考
- [官網](https://brew.sh/index_zh-tw)
