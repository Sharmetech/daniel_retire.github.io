# 復華退休活動

## 測試站
https://4fhtrustretire.isobar.com.tw/preview/

## 前端相關
#### gitlab 使用
- 請開branch，命名沒有規範
- 完成後發issue assign 給 @ammon.lin

#### 頁面切版相關
- 開發請使用vscode的live server
- 檔案請放在 /www/preview/ 下
- 資料夾結構
  ```
	|-css 
	|-js 
	|-image 
	|-*.html
	```
- 背景圖片使用裁切方式呈現
- 字型使用google font 思源黑體為主要字體，加上 sans-serif
- 圖片都請加上此字串 `?v=version`
  ```html
  <img src="images/zzz.jpg?v=version">
  ```
  ```css
  .aaa{
	  background:url('../images/zzz.jpg?v=version');
  }
  ```
- 表單完成後開啟lightbox的接口已經寫好了 \
  `$('.form')` 的部分，可自行替換 
  ```javascript
  	$(function () {
		$('form').leads(function(frm) {
      // this === frm
			//表單按下送出後完成要做的事情
			alert('success');
		});
	});
  ```
  表單目前有的結構請勿自行刪除，但可以增加class
#### FB及LINE分享的方式
1. 開空的頁面 - ex: 真理1分享網址 indexTip1.html
2. 在此頁面下好分享的meta data及轉址 - ex: indexTip1.html 轉址 index.html#indexTip1
3. 頁面上真理1分享網址設定為 indexTip1.html


