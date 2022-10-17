# 用python爬蟲模擬pixiv網站熱門搜尋功能之可行性
## 前言
本專案僅作為本人面試工作時展示作品之用，功能及介面還相當簡陋。
如真的想要使用pixiv的熱門搜尋功能，建議還是直接買個會員比較快。
## 使用方法
打開上方pixiv_get或pixiv_web檔案，並修改最後一行程式碼。  
``` python3 
pixiv_get(keyword, page, rating_count)
```  
有三個參數可以輸入，第一個輸入關鍵字，第二個輸入要爬取頁數(未登入狀態僅能爬取十頁)，第三個輸入只顯示或下載多少收藏數以上的圖片。  
``` python3 
pixiv_get('cyberpunk',10 , 500)
```  
以上示為例，輸出的結果是爬取關鍵字是cyberpunk，前十頁收藏數超過500的圖片，並且由高到低排列。  
pixiv_get 此程式功能為將爬取到的插畫以原圖尺寸下載到download資料夾內。  
* 呈現示意圖:
<img src="img/image_2.PNG" width="50%">
  
***
pixiv_web 此程式功能為將爬取的內容以網站得方式呈現，每張圖點進去都會連結到該圖片的pixiv網站。  
* 呈現示意圖:
<img src="img/image.PNG" width="50%">
  

