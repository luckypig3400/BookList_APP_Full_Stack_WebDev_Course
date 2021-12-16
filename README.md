# BookList_APP_Full_Stack_WebDev_Course
 Book list App tutorial from Full Stack Web Development Course

## Full Course Play list

### [Full Stack Web Development Course](https://youtube.com/playlist?list=PLZlA0Gpn_vH8jbFkBjOuFjhxANC63OmXM)



## Notes for each Video

### 1. [Project Setup - Node.js/Express/MongoDB Course #1](https://www.youtube.com/watch?v=qj2oDkvc4dQ&list=PLZlA0Gpn_vH8jbFkBjOuFjhxANC63OmXM&index=5)

#### 初始化專案
```
npm init -y
```
> -y 代表全部使用預設值(all yes for default)

#### 安裝套件
+ express
+ ejs
+ express-ejs-layouts
```
npm i {以上三種套件 以空白隔開}
```

開發套件nodemmon
此套件會在code有被修改時自動重啟server
```
npm i --save-dev nodemon
```

#### 編輯腳本
可以使用npm run {scriptCommand} 來執行專案設定的除錯腳本
**例如:**於package.json中的scripts內加入,
"devStart": "nodemon server.js"
則可以npm run devStart來執行對應的指令

### 2. 