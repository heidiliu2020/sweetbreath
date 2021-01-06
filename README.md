# Sweetbreath

[Sweetbreath 甜の呼吸 網路甜點工作室](http://sweetbreath.tw/)

![](./img/localhost-index02-20210106.png)

## 專案介紹

本專案為 Sweet Breath 甜の呼吸甜點購物車前端與後端原始碼，主要開發技術為 React Hooks、
styled-components、Express、Sequelize、MySQL。

使用者相關功能

`商品模組`

- 商品分類檢視：商品分類以外，可建立特殊商品分類，例如人氣商品。
- 瀏覽所有商品：依商品分類呈現。
- 瀏覽單一商品：瀏覽商品名稱、商品介紹、商品規格、商品庫存、選擇商品數量加入購物車。

`購物模組`

- 購物車：選擇商品數量加入購物車，顯示訂單摘要。
- 結帳：導向登入頁面，登入後輸入配送資料並檢視輸入格式，確認訂單總額後提交訂單。

`會員模組`

- 會員註冊：必須輸入全名、帳號、電子郵件、密碼，檢視符合輸入格式即可註冊成功。
- 會員登入：必須輸入帳號、密碼，即可登入。登入後依會員權限顯示一般權限選單／管理權限選單。
- 會員專區：會員登入後可瀏覽個人資料、消費紀錄。個人資料可修改全名、電子郵件、生日、地址，為統一修改模式，全名、電子郵件必填，其他未填欄位於送出後清除原本資料。消費紀錄可瀏覽全部訂單，並顯示訂單狀態、訂單明細，點擊商品圖片、商品名稱可瀏覽商品介紹。

`基本模組`

- 首頁：主打活動輪播區、人氣商品。
- 關於我們：瀏覽網站架設理念。
- 最新消息：瀏覽最新消息列表。
- 聯絡我們：瀏覽店家聯絡資料，瀏覽 Google Maps 實體地址、聯絡表單。

管理者相關功能

`商品管理模組`

- 依商品分類瀏覽所有商品。
- 編輯商品：可編輯商品資訊，包括商品名稱、圖片網址、狀態、分類、商品介紹。
- 刪除商品：後端處理為變更商品狀態，仍保留商品資訊。
- 新增商品：可新增商品資訊，包括商品資訊、商品規格，商品規格包括規格名稱、原價、特價、庫存。

`分類管理模組`

- 瀏覽所有商品分類名稱，顯示各類商品數量。
- 編輯／刪除／新增分類。
- 刪除分類：刪除商品：後端處理為變更分類狀態，仍保留分類名稱。

`權限管理模組`

- 瀏覽所有帳號，可依使用者 id 或名稱搜尋特定帳號。
- 分為一般權限、管理權限、停權。
- 停權：後端處理為變更帳號狀態，仍保留帳號資訊。

`訂單管理模組`

- 瀏覽所有訂單明細，依訂單狀態顯示訂單。
- 管理訂單狀態，依付款進度、出貨進度調整訂單狀態，或取消處理中訂單。
- 取消訂單：後端處理為變更訂單狀態，仍保留訂單資訊。

![](./img/userflow-client-v3-20210104.png)

![](./img/userflow-admin-v3-20210104.png)

## 專案後端

[sweetbreath-backend](https://github.com/ivymuchacha/sweetbreath-backend)：主要開發技術為 Express、Sequelize、MySQL。

## 專案執行

`npm install`

安裝專案所需套件。

`npm run dev`

http://localhost:3000 啟動專案。  
http://localhost:5000 啟動專案後端。

`npm build`

資料夾 build 建立專案 production 版本。

`npm deploy`

GitHub Pages 部屬專案網站。

## 專案技術

`前端框架與套件`

- [React Hooks](https://reactjs.org/)
- [Create React App](https://create-react-app.dev/)
- [React DOM](https://www.npmjs.com/package/react-dom)
- [React Router DOM](https://reactrouter.com/)
- [PropTypes](https://www.npmjs.com/package/prop-types)
- [styled-components](https://styled-components.com/)
- [ESLint](https://eslint.org/)
- [Prettier](https://prettier.io/)
- [Google Map React](https://github.com/google-map-react/google-map-react)

`後端框架與套件`

- [Express](https://expressjs.com/)
- [Sequelize](https://sequelize.org/)
- [MySQL](https://www.mysql.com/)

`第三方 API`

- [Google Cloud Platform](https://cloud.google.com/)
- [Imgur](https://imgur.com/)

## 專案展示

### 商品模組

![](./img/)

### 購物模組

![](./img/)

### 會員模組

![](./img/)

### 後臺管理模組

![](./img/)

## 專案授權

[MIT License](https://choosealicense.com/licenses/mit/)
