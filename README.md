# Functionpop
資展國際-結訓專題

## 專案重點

此專案為資展國際的結訓專題，由我與其他四個組員共同完成

以下為我負責的部分
* 頁面皆支援RWD功能，最小到iphone12 pro
* 會員專區頁面皆有登入判斷，未登入看不到資訊

1. 會員登入畫面
登入後會運用session記住會員登入的狀態。

2. 會員個人資料更改
運用session功能帶出會員的相關資料(性別、生日、性別...)
可直接更改聯絡電話和地址，按下儲存會再次詢問是否更改。

3. 會員密碼更改
會判對是否有輸入新、舊密碼，如未輸入會跳出相關錯誤訊息(ex:舊密碼不可為空)
都輸入正確會跟資料庫進行比對舊密碼，舊密碼正確會將新密碼以bcrypt技術進行雜湊加密進資料庫儲存。

4. 訂單&退貨
會到資料庫根據使用者名稱撈訂購資料，並把各項購買數量和金額做加總。

5. 檢視訂單資訊
會呈現該筆訂單的詳細資訊，買的品項、數量、金額......。

6. 我的最愛
在商品頁（ [localhost:3005/home/product/Male](http://localhost:3005/home/product/Male) )直接按愛心會呈現紅色愛心表示已加入我的最愛收藏，使用AJAX將資訊傳到後端。
到我的最愛頁面可以看到商品的描述、價格，點擊圖片可以直接到該商品頁；點一致購物車按鈕可以直接選擇商品的尺寸、顏色、數量，按確定會加入購物車；後方的垃圾桶按鈕刪除收藏；右上角有一鍵刪除所有收藏按鈕，右手邊有商品數量小計。

<img src="https://i.imgur.com/UVI7nJ7.png" width="70%" alt="我的最愛-DESKTOP"/><img src="https://i.imgur.com/IFypgvo.png" width="30%" alt="我的最愛-RWD"/>

## 安裝步驟
### 安裝資料庫
使用
* 使用XAMPP + MySQL
1. 建立資料庫
```SQL
create database functionpop;
```
2. 匯入資料表
`複製0718 DB V3.sql`

### 建立執行環境
1. 
```bash
npm i
```
2.
```bash
npm start
```
或
```bash
nodemon app.js
```
到網址列輸入 ([localhost:3005/home](http://localhost:30054/home)) 即可
網址（ [localhost:3005/home/product/Male](http://localhost:3005/home/product/Male) )




  
