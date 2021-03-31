# Yarn

Yarn 是 javascript 套件管理器, 相容於 npm 的工作內容, 並且更為快速, 安全!

yarn 會將使用過的套件在本機 cache 一份, 之後如果有其他專案使用到, 就不需要再次從網路上下載, 減少等待時間!


## 目錄
- [安裝 Yarn](#安裝-Yarn)
- [管理 javascript 套件](#管理-javascript-套件)
- [參考](#參考)


## 安裝 Yarn

### 透過 homebrew 安裝 yarn

- [安裝 homebrew方法](../homebrew/README.md)

- 在終端機輸入
```sh
brew install yarn
```

- 確認 yarn 的版本
```sh
yarn --version
```

## 管理 javascript 套件
專案依賴的套件會安裝在 node_modules 目錄下, 並記錄在 package.json 檔案中, 如此我們可以在上傳專案時, 透過 .gitignore 排除上傳套件, 而他人也可以透過 package.json 知道專案依賴哪些套件, 並安裝

### 建立 package.json 文件
```sh
yarn init
```

### 加入依賴套件
```sh
# 加在 package.json 的 dependencies 欄位
yarn add [套件名稱]

# 加在 package.json 的 devDependencies 欄位
yarn add --dev [套件名稱]
```

### 安裝 package.json 的依賴套件
```sh
yarn
yarn install
```

### 升級套件
```sh
yarn upgrade [套件名稱]
```

### 移除套件
```sh
yarn remove [套件名稱]
```


## 參考
- [官網](https://classic.yarnpkg.com/en/)
- [IT邦幫忙](https://ithelp.ithome.com.tw/articles/10191745)
