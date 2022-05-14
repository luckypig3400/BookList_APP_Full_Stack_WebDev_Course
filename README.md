# BookList_APP_Full_Stack_WebDev_Course
 Book list App tutorial from Full Stack Web Development Course

## Full Course Play list

### [Full Stack Web Development Course](https://youtube.com/playlist?list=PLZlA0Gpn_vH8jbFkBjOuFjhxANC63OmXM)

## 目前進度(下方影片9分06秒)
+ https://www.youtube.com/watch?v=esy4nRuShl8&list=PLZlA0Gpn_vH8jbFkBjOuFjhxANC63OmXM

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

#### router設定注意事項
+ 若有多個router建議分開文件寫，放在routes/底下
+ 記得把寫好的router文件export(module.exports = router)
+ 記得引入並使用該router

#### views小筆記
+ 要渲染EJS頁面需使用res.render()而非res.send()
+ 以layout.ejs作為模板並使用<%- %>會把不同route對應的EJS文件內容都引入進來

#### MongoDB
+ 首先安裝MongoDB[(可參考此影片)](https://www.youtube.com/watch?v=wcx3f0eUiAw)
+ 再來安裝套件
```
npm install mongoose
```
+ 設定DB連線參數時會使用到.env檔案 記得新增該檔案與安裝套件
```
npm i --save-dev dotenv
(僅在開發專案時使用，安裝為開發套件)
```

#### 專案初步構建完成 加入git init &設定gitignore
+ 我已經使用github desktop內建的git來追蹤修訂版本
+ git安裝設定與教學可[參考此](https://www.youtube.com/watch?v=IHaTbJPdB-s)

#### 連結Repo並部署至Heroku 這邊紀錄大致操作步驟
+ https://youtu.be/qj2oDkvc4dQ?list=PLZlA0Gpn_vH8jbFkBjOuFjhxANC63OmXM&t=1152
+ Create new app on Heroku
+ Install the Heroku CLI
+ Push git repo to Heroku remote
+ Set-up ENV vairables in Heroku app Settings page
+ 註冊MongoDB Atlas免費的線上資料庫平台
+ 新版的MongoDB Atlas似乎需要先Create Orginization & Create Project
+ 然後進入剛建立的專案後Create Database(或稱為Cluster)接著選免費方案
+ 可以在建立Cluster的頁面更改Cluster Name或是用預設值也可以
+ 進到建立好的Cluster設定頁面建立DB使用者
![](https://i.imgur.com/AuVkIHz.png)
+ 接著到左上角Database頁籤點選Connect並點選Choose a connection method
![](https://i.imgur.com/ZblaGYc.png)
![](https://i.imgur.com/uqtq99K.png)
+ 接著選Connect Your Application 後面的操作介面一樣就著影片操作即可
+ 補充:MongoDB Atlas可能需要設定允許所有IP的連線(較方便)或是特定IP

### 2. 