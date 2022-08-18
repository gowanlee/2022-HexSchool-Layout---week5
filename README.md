# 2022-HexSchool-Layout---week5

2022 六角切版直播班 - 第五週

本週學習重點：

<b>1. form標籤</b>
  - action指的是要把表單傳送到後端的哪個網址
  - method指表單傳送的方法
    - 表單一率使用`method="post"`是指把整包資料傳送過去

<b>2. input表單標籤</b>
  - type指輸入格式 例如text、tel、password等
    - `type="submit"`是會把表單送到後端
    - `type="date"`不要用!!!!!!!!
      - 因為瀏覽器輸出的格式不一樣會造成資料大亂
      - 因為每個裝置顯示的樣式不一樣無法更改
      - 可以用jQurey的套件Datepicker解決
  - name指輸入資料名稱
  - 如不希望被點擊可加上disabled
  - 如只供觀看不要修改可加上readonly
    - disabled 用 form傳送的話不會帶值，但readonly會
  - 如是必填可加上required(此提示樣式無法客製化)

<b>3. 表單一定要有`<form></form>`、`<input>`、`<input type="submit">`</b>

<b>4. label標籤</b>
  - 加上這標籤可以增加使用者體驗，點擊label標籤裡的文字就會自動對應到input框框裡
  - for一定要跟input的id相同 
  - 如果label標籤裡包input就不用寫for跟id

<b>5. select & radio 預設樣式無法更改，如果要更改只能自己用js重寫樣式功能</b>
  - [做出客製化select下拉選單](https://codepen.io/mukul6996/pen/pWjBzV)
  - [做出客製化radio](https://codepen.io/bbodine1/pen/DqdMRy)

<b>6. Bootstrap5</b>
  - Bootstrap 的 Reset 是 normalize，不需加入 Meyerweb 的 CSS Reset
  - 正式專案通常都會用本地端不會用cdn的方式
  - list-unstyled可以消除list前面的圓點
  - 彈跳視窗可以用modal
  - class名稱fs只有文字大小，h1-h6有包含文字大小、文字粗細體、行高
  - img-fluid裡包含`max-width:100%`、`height:auto`
  - [BS5參考文件](https://bootstrap5.hexschool.com/docs/5.1/getting-started/introduction/)

<b>7. base全站設定是放html標籤</b>

<b>8. Material icons提供的較基本，Fontawesom提供的樣式較多</b>

<b>9. button、select、option只能用disabled</b>

-------------------------------------
 
下方提供關於作業細節的建議：

<b>整體</b>
1. 圖片可以設定 object-fit: cover; 來防止圖片變形
2. 元素間距要符合設計稿，例如 logo 到 .navbar-nav 的距離應為 32px
<br>
<br>
<br>
<b>導覽列</b>
1. navbar 沒有在格線內，不需要使用 .container
<br>
<br>
<br>
<b>Admin</b>
1. ID 右方綠色箭頭為可點擊的元素，可用 a 標籤包住
2. #viewAdmin 中的 Edit 按鈕點擊後要開啟 #editAdmin
[作法可參考文件](https://bootstrap5.hexschool.com/docs/5.0/components/modal/#toggle-between-modals)
3. Edit Admin 跳窗內的 「Access Level」內容可以使用[Bootstrap 的 form-select 製作](https://bootstrap5.hexschool.com/docs/5.0/forms/select/)
