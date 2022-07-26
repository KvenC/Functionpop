# Functionpop
資展國際-結訓專題

## 版權說明
**該專案內的商品圖片皆來自H&M，僅使用在此專案做為練習之用並不會用於任何商業用途**

## 專案重點

此專案為資展國際的結訓專題，由我與其他四個組員共同完成

以下為我負責的部分
   * 頁面皆支援RWD功能，最小到iphone12 pro

<img src="https://i.imgur.com/UVI7nJ7.png" width="60%" height="75%" alt="我的最愛-DESKTOP"/><img src="https://i.imgur.com/IFypgvo.png" width="25%" height="50%" alt="我的最愛-RWD"/>

   * 會員專區頁面皆有登入判斷，未登入看不到資訊

1. 會員登入畫面

   登入後會運用session記住會員登入的狀態，並且會判斷使用者是否此使用者或帳密是否正確。
   <img src="https://github.com/KvenC/Functionpop/blob/main/GIF/網站登入.gif" width="100%" height="75%" alt="網站登入"/>
   
2. 會員個人資料更改

   運用session功能帶出會員的相關資料(性別、生日、性別...)
   可直接更改聯絡電話和地址，按下儲存會再次詢問是否更改。
   <img src="https://github.com/KvenC/Functionpop/blob/main/GIF/更改個人資料.gif" width="100%" height="75%" alt="個人資料更改"/>

3. 會員密碼更改

   會判對是否有輸入新、舊密碼，如未輸入會跳出相關錯誤訊息(ex:舊密碼不可為空)    
   都輸入正確會跟資料庫進行比對舊密碼，舊密碼正確會將新密碼以bcrypt技術進行雜湊加密進資料庫儲存。
   <img src="https://github.com/KvenC/Functionpop/blob/main/GIF/變更密碼判斷.gif" width="100%" height="75%" alt="會員密碼更改"/>

4. 訂單清單和訂單細節

   會到資料庫根據使用者名稱取得訂購資料，並把各項購買數量和金額做加總。
   訂單細節會呈現該筆訂單的詳細資訊，買的品項、數量、金額......。
   <img src="https://github.com/KvenC/Functionpop/blob/main/GIF/訂單詳情.gif" width="100%" height="75%" alt="訂單詳情"/>
 
5. 我的最愛

   * 在商品頁（ [localhost:3005/home/product/Male](http://localhost:3005/home/product/Male) )直接按愛心會呈現紅色愛心表示已加入我的最愛收藏，使用AJAX將資訊傳到後端。
   <img src="https://github.com/KvenC/Functionpop/blob/main/GIF/加入我的最愛.gif" alt="我的最愛-收藏"/>

   * 到我的最愛頁面可以看到商品的描述、價格，點擊圖片可以直接到該商品頁；點移至購物車按鈕可以直接選擇商品的尺寸、顏色、數量，按確定會加入購物車。
   <img src="https://github.com/KvenC/Functionpop/blob/main/GIF/我的最愛加入購物車.gif" width="100%" alt="我的最愛-DESKTOP"/>

   * 後方的垃圾桶按鈕刪除收藏；右上角有一鍵刪除所有收藏按鈕，右手邊有商品數量小計。
   <img src="https://github.com/KvenC/Functionpop/blob/main/GIF/我的最愛-刪除.gif" width="100%" alt="我的最愛-刪除"/>

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
1. 安裝套件
```bash
npm i
```
2. 執行專案
```bash
npm start
```
或
```bash
nodemon app.js
```
3. 到網址列輸入 ([localhost:3005/home](http://localhost:3005/home)) 即可
網址（ [localhost:3005/home/product/Male](http://localhost:3005/home/product/Male) )




  
